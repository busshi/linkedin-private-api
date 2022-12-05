**[@busshi/linkedin-private-api](../README.md)**

> [Globals](../globals.md) / ["src/repositories/invitation.repository"](../modules/_src_repositories_invitation_repository_.md) / InvitationRepository

# Class: InvitationRepository

## Hierarchy

* **InvitationRepository**

## Index

### Constructors

* [constructor](_src_repositories_invitation_repository_.invitationrepository.md#constructor)

### Methods

* [getReceivedInvitations](_src_repositories_invitation_repository_.invitationrepository.md#getreceivedinvitations)
* [getSentInvitations](_src_repositories_invitation_repository_.invitationrepository.md#getsentinvitations)
* [replyInvitation](_src_repositories_invitation_repository_.invitationrepository.md#replyinvitation)
* [sendInvitation](_src_repositories_invitation_repository_.invitationrepository.md#sendinvitation)

## Constructors

### constructor

\+ **new InvitationRepository**(`__namedParameters`: { client: [Client](_src_core_client_.client.md)  }): [InvitationRepository](_src_repositories_invitation_repository_.invitationrepository.md)

*Defined in [src/repositories/invitation.repository.ts:37](https://github.com/busshi/linkedin-private-api/blob/f1b6b7b/src/repositories/invitation.repository.ts#L37)*

#### Parameters:

Name | Type |
------ | ------ |
`__namedParameters` | { client: [Client](_src_core_client_.client.md)  } |

**Returns:** [InvitationRepository](_src_repositories_invitation_repository_.invitationrepository.md)

## Methods

### getReceivedInvitations

▸ **getReceivedInvitations**(`__namedParameters?`: { limit: number = 100; skip: number = 0 }): [InvitationScroller](_src_scrollers_invitation_scroller_.invitationscroller.md)

*Defined in [src/repositories/invitation.repository.ts:69](https://github.com/busshi/linkedin-private-api/blob/f1b6b7b/src/repositories/invitation.repository.ts#L69)*

#### Parameters:

Name | Type | Default value |
------ | ------ | ------ |
`__namedParameters` | { limit: number = 100; skip: number = 0 } | {} |

**Returns:** [InvitationScroller](_src_scrollers_invitation_scroller_.invitationscroller.md)

___

### getSentInvitations

▸ **getSentInvitations**(`__namedParameters?`: { limit: number = 100; skip: number = 0 }): [InvitationScroller](_src_scrollers_invitation_scroller_.invitationscroller.md)

*Defined in [src/repositories/invitation.repository.ts:61](https://github.com/busshi/linkedin-private-api/blob/f1b6b7b/src/repositories/invitation.repository.ts#L61)*

#### Parameters:

Name | Type | Default value |
------ | ------ | ------ |
`__namedParameters` | { limit: number = 100; skip: number = 0 } | {} |

**Returns:** [InvitationScroller](_src_scrollers_invitation_scroller_.invitationscroller.md)

___

### replyInvitation

▸ **replyInvitation**(`__namedParameters`: { action: string = "accept"; invitationId: string ; invitationSharedSecret: string  }): Promise<void\>

*Defined in [src/repositories/invitation.repository.ts:43](https://github.com/busshi/linkedin-private-api/blob/f1b6b7b/src/repositories/invitation.repository.ts#L43)*

#### Parameters:

Name | Type |
------ | ------ |
`__namedParameters` | { action: string = "accept"; invitationId: string ; invitationSharedSecret: string  } |

**Returns:** Promise<void\>

___

### sendInvitation

▸ **sendInvitation**(`__namedParameters`: { message: undefined \| string ; profileId: string ; trackingId: string  }): Promise<[Invitation](../interfaces/_src_entities_invitation_entity_.invitation.md)\>

*Defined in [src/repositories/invitation.repository.ts:77](https://github.com/busshi/linkedin-private-api/blob/f1b6b7b/src/repositories/invitation.repository.ts#L77)*

#### Parameters:

Name | Type |
------ | ------ |
`__namedParameters` | { message: undefined \| string ; profileId: string ; trackingId: string  } |

**Returns:** Promise<[Invitation](../interfaces/_src_entities_invitation_entity_.invitation.md)\>
