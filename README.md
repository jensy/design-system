# hpe design-system monorepo
### HPE Design System Site

[![Netlify Status](https://api.netlify.com/api/v1/badges/39e37d4a-4f9f-4946-8aeb-b8328b1821cd/deploy-status)](https://app.netlify.com/sites/keen-mayer-a86c8b/deploys) - https://design-system.hpe.design/  



### Storybook

[![Netlify Status](https://api.netlify.com/api/v1/badges/e4cb8d72-f3c0-4490-a4d7-54273ac277ed/deploy-status)](https://app.netlify.com/sites/thirsty-shockley-2b7675/deploys) - http://storybook.hpe.design/

# Welcome to HPE Design System
Aries is a monorepo built from two modules.

1. aries-core
2. aries-site

The Monorepo is installed using [yarn](https://github.com/yarnpkg/yarn), and relies on [yarn workspaces](https://yarnpkg.com/lang/en/docs/workspaces/).

Packages are automatically linked together, meaning you can do cross-package work within the repo. woot-woot!

### Basic structure and configurations

```
aries/
  aries-*/
    src/js/
      index.js
    package.json         // package-specific deps and scripts
    README.md            // shown in npmjs.com. included in npm artifact

.eslintignore            // eslint (linter) ignored directories/files
.eslintrc                // eslint (linter) configuration based on @hpe/project-scripts
.gitignore               // github's default node gitignore with customizations
.prettierrc.js           // prettier (formatter) configuration based on @hpe/project-scripts
package.json             // common dev deps and workspace-wide scripts WIP
README.md                // workspace-wide information. shown in github
yarn.lock                // the only lock file in the repo. all packages combined
```

## Getting Started

```
yarn install
```

Running 'yarn install' anywhere in the monorepo hierarchy will always install ALL the modules in the workspaces.

Run aries-site in development mode:

```
cd aries-site
yarn start
```

Running in production mode:

```
yarn build
```

## Sprint Schedule 

**1. January 13 - 17**  
- Server app component breakdown
- Finalize Component pages (Design System site) 
- Review site
- Establish research plan

**2. January 20 - 24**  
- Incorperate Design System site feedback 
- HPE XS showcase
- Core component discovery

**3. January 27 - 31**   
- Finalize Design System site
- Reprioritize roadmap 
- Identify simple patterns 
- Remove referances to Aries

**4. February 3 - 7**   
- Publish HPE theme
- Incorporate site testing (discuss approach) 
- Optimize Netlify build process
- Finalize pattern vis approach (inline vs storybook) 
- Designs for: Button, Type, Anchor, Color
- Research kick off email 
- Schedule stakeholder interviews and gather probing questions. (what info is vauluable for us moving forward?) 

**5. February 10 - 14**   
- Dev: Button, Type, Anchor, Color 
- Design: Layout, Navigation, List, Form/input 

**6. February 17 - 21**  
- Dev: Layout, Navigation, List, Form
- Design: Modal/drop, Card 
