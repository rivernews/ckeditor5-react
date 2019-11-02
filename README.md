# A Custom Build for Ckeditor5 React

[Original upstream repository](https://github.com/ckeditor/ckeditor5-react).

The motivation to fork and create our own Ckeditor build is a better user experience. The needs are tailored to our own use case so I have no plan to create PR at least in the short term, but the UX principles behind these add-ons and improvement in this repo are universe. (see [the heuristics introduced by Nielsen](https://en.wikipedia.org/wiki/Heuristic_evaluation))  

What did we add on top of the original Ckeidtor?
- Expose the `keydown` event, so you can setup more keyboard shortcut based on your needs
- Not so much currently, but we're constantly reviewing our use case and will add more...!

## How to update code and release to npm

1. Commit code in git, give commit message.
1. Run `npm run patch-publish`.

## Relevant repository

- Our custom [Ckeditor balloon build](https://github.com/rivernews/ckeditor5-build-balloon). This Ckeditor React repository serves like an adapter between vanilla Ckeditor and the React framework, that means you can switch the vanilla Ckeditor5 part with any other variant you want - say it's the offical or somebody else custom build like me.
- User facing apps
    - [Appl Tracky](https://github.com/rivernews/appl-tracky-spa). Written in React, this frontend SPA uses this repo as a npm package with our custom balloon build mentioned above.
    - [Iriversland2](https://github.com/rivernews/iriversland2-spa) - my personal website which use Ckeditor. It's written in Angular so does not use this repo, but uses my custom build of Ckeditor balloon editor.