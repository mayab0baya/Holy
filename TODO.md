This will be our nonexhaustive todo list for Holy Unblocker LTS v6.x.x and above.

## Code Cleanup

  - [ ] Remove all current obfuscation in the source code. It needs to be dynamically obfuscated if anything, or not obfuscated at all. This option will be a config option on the server side before rendering with Express for a performance focus. Meta elements will have an additonal attribute indicating if they should be moved. This is to ensure a SEO source can be served by config or a source focused on pure censorship evasion.
  - [ ] Optimize the stylesheets and the HTML layout. Add more proper commenting and redivide the code so that it's less hard on the eyes.
  - [ ] Optimize the JS. This time it won't be in one line and will be somewhat thoroughly commented.
  - [ ] Restructure navigation scripts to ensure updated proxy functionality is sanitized and effective
  - [x] Particles.js automatically adjusting per display size - done
  - [x] Fix routes.mjs throwing with incorrect paths - done
  - [x] Create test script - done
  - [x] XSS and fingerprinting protection (may need updates) - done
  - [ ] Update games navigation JS and page
  - [ ] Ensure all the original submodules get added back to HU-Archive

## Proxy/Site Functionality
  - [x] Ensure Ultraviolet is updated to support bare-mux and wisp - done
  - [x] Add Rammerhead support - done
  - [x] Fix slow Ultraviolet speeds despite being local; something on the backend?? - done
  - [ ] Fix Ultraviolet on Firefox
  - [ ] Adapt Applications page to use either Rammerhead or UV (for Reddit, YouTube, Discord)
  - [ ] libcurl, epoxy and all that fun stuff 
  - [ ] socks5/tor routing option that can be configured (enabled) via either a cookie or pathname as a settings meny option
  - [ ] Update games page content
  - [ ] Update csel.js (after Setting menu redesign) to support custom transports, icon swap, routing
  - [ ] Omnibox autoupdate script (for the Google/Bing style auto suggest feature)

## Site Redesign
  - [x] Add potato (lime reminded me to do this)
  - [x] Landing Page - done
  - [ ] Web Proxies page
  - [ ] Application page
  - [ ] Games Library page
  - [x] Footer Design - done
  - [x] Header Design - done

## Changelog

  - Added wisp support
  - Fixed AD config setting being opt-out; ads are not implemented in the project however
  - Added Rammerhead support (locally)
  - Drastically updated visuals across the service and refactored stylesheets
  - Bumped games page functionality
  - Updated randomization scripts to ES6 syntax and implemented the alternative to RegEx string replacement
  - Helmet for express implemented into backend
  - Improved component handling via templates.mjs along with deletion of obsolete files that previously handled this standard in a poor format
  - Fixed oddly slow speeds with Ultraviolet (as well as a general version bump to support epoxy-tls and bare-mux)
  - Implemented testing scripts for an improved GitHub actions workflow by doing a quick test on proxy + site functionality
  - Greatly optimized client-side scripts across the site with a new standard
  - Changes to server.mjs with path logic and error handling
  - Updated standards for common scripts
  - Ultraviolet made local
