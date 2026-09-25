# Contributing to Nephrite

**English** · [Español](CONTRIBUTING.es.md)

Nephrite grows one app at a time, and most of those apps will be themed by people like you. Thanks for being here.

## Ways to help

- **Request a port.** Tell us which app you want next with the [port request form](https://github.com/Nephrite-theme/web/issues/new?template=port-request.yml). If it's already requested, add a 👍 to that issue; we use the votes to prioritize.
- **Build a port.** Theme an app with the Nephrite palette. See below.
- **Report a problem.** A color that clashes, low contrast or a broken install: open an issue in that port's repository, or use the [problem report form](https://github.com/Nephrite-theme/web/issues/new?template=bug-report.yml) for the website.
- **Translate the website.** Copy lives in [`web/messages`](https://github.com/Nephrite-theme/web/tree/main/messages), one JSON file per language.

## Building a port

1. **Check it's free.** Look at [getnephrite.dev/ports](https://getnephrite.dev/ports) and the [open requests](https://github.com/Nephrite-theme/web/issues?q=is%3Aissue+label%3A%22port+request%22). If someone already claimed the app, coordinate in that issue.
2. **Claim it.** Comment on the request (or open one) saying you're building it, so work isn't duplicated.
3. **Start from the template.** Click **Use this template** on [Nephrite-theme/template](https://github.com/Nephrite-theme/template). It comes with the README, folders, a palette sync script and a checklist.
4. **Use the palette by role.** Take the colors from [Nephrite-theme/palette](https://github.com/Nephrite-theme/palette) and follow its [porting guide](https://github.com/Nephrite-theme/palette#building-a-port): which color goes on backgrounds, text, accents, syntax and terminal slots. Don't invent new colors; if the palette is missing something, open an issue in the palette repository.
5. **Cover the flavors.** Ship Forest, Jade and Mint when the app allows several themes. If it only allows one, start with Forest.
6. **Document it.** A README with install steps and one screenshot per flavor. Name the repository `<app>` if it will live in the organization, or `<app>-nephrite` in your own account.
7. **Submit it.** Open a [port submission](https://github.com/Nephrite-theme/web/issues/new?template=port-submission.yml) with the repository link and screenshots.

### What we check

- Colors come from `palette.json` and are used by role.
- Text stays readable: body text at 4.5:1 contrast or more against its background.
- The README explains installation.
- The port is MIT licensed.

### After review

Accepted ports are listed on [getnephrite.dev/ports](https://getnephrite.dev/ports). Your repository stays yours. If you'd like, we can transfer it into the Nephrite-theme organization and keep you as its maintainer, so it's easier to find and keep in sync with palette updates.

## Pull requests

- Keep each pull request focused on one change.
- Describe what changed and add a screenshot for anything visual.
- Commit messages follow [Conventional Commits](https://www.conventionalcommits.org) when possible (`feat:`, `fix:`, `docs:`).

## Be kind

Assume good intent, give feedback on the work and not the person, and help newcomers find their way. Maintainers may remove comments or contributions that don't follow this.
