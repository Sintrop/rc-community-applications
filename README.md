# Regeneration Credit — community applications

This repository collects **expressions of interest** from people who want to join
the [Regeneration Credit](https://regenerationcredit.org) as a researcher,
inspector, developer, contributor, activist or regenerator.

Each application is a GitHub issue, created from a form. Existing members of the
community browse the open issues here and, when they choose, issue an **on-chain
invitation** to an applicant. There is no queue and no guaranteed timeline.

## How to apply

Open a new issue and pick the form for the role you are interested in:

- [Apply as a Researcher](../../issues/new?template=researcher.yml)
- [Apply as an Inspector](../../issues/new?template=inspector.yml)
- [Apply as a Developer](../../issues/new?template=developer.yml)
- [Apply as a Contributor](../../issues/new?template=contributor.yml)
- [Apply as an Activist](../../issues/new?template=activist.yml)
- [Apply as a Regenerator](../../issues/new?template=regenerator.yml)

You will be asked for a name or handle, the wallet address that would receive the
invitation, and a short description of how you can contribute.

> **Supporters** do not need an invitation. Anyone can start supporting the
> project directly — see <https://regenerationcredit.org/supporters>.

## Your data is public

**By opening an application you agree that everything in it — including your
wallet address, your name or handle and your description — is public and
permanent.** GitHub issues are visible to anyone and are also mirrored on the
website's public applications page. Do not include anything you are not
comfortable sharing. You may use a pseudonym instead of a real name.

## How the invitation works

1. You open an application issue here.
2. A member of the community reviews it. They may comment with questions.
3. If they decide to invite you, they call `InvitationRules.invite(yourWallet, role)`
   on the Sintrop Impact Blockchain.
4. You then register in the app with your name and identity photo, which checks
   your invitation on-chain.
5. The application issue is closed with a note.

Applications may also be closed if they are spam, duplicated, or inactive for a
long time. Closing an issue is not a rejection of the person — you are welcome to
apply again.

## Labels

| Label | Meaning |
| --- | --- |
| `application` | Every application issue carries this label. |
| `role: <role>` | The role applied for (`role: researcher`, `role: inspector`, …). |
| `invited` | An invitation has been issued on-chain. |
| `spam` | Not a genuine application. |

Labels are defined in [`.github/labels.yml`](.github/labels.yml) and created
automatically by the *Sync labels* workflow. To provision them on a fresh
repository, run that workflow once from the **Actions** tab.

## License

The content of this repository is released under
[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) — public domain.
