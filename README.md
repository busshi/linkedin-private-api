# NodeJS LinkedIn API

Forked version of [this API](https://github.com/eilonmore/linkedin-private-api) but with additionnal functionnalities waiting for the author to merge the [pull request](https://github.com/eilonmore/linkedin-private-api/pull/473)


## Installation

```
yarn add @busshi/linkedin-private-api
```

## Examples

```typescript
import { Client } from "@busshi/linkedin-private-api";

const receivedScroller = client.invitation.getReceivedInvitations();
const receivedInvitations = await receivedScroller.scrollNext();

for (const invit of receivedInvitations) {
    const { entityUrn, profile, sharedSecret } = invit;
    const { profileId } = profile;
    const invitationId = entityUrn.split(":")[3];

    await client.invitation.replyInvitation({
        invitationId,
        invitationSharedSecret: sharedSecret,
    });
}  
```

```typescript
const conversation = await client.conversation.markConversationAsRead({
      conversationId,
});
console.log(conversation);
```

## Notes

Made for learning purposes.
