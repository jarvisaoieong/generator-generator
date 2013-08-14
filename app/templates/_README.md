# <%= name %>

> <%= description %>

## Getting Started<% if (usingGithub) { %>

```sh
$ npm install -g <%= githubUser %>/<%= githubRepo %>
$ mkdir /path/to/your/project
$ cd $_
$ yo <%= githubRepo.replace(/^generator-/, '') %>
```<% } else { %>
_(Coming soon)_<% } %><% if (usingGithub && licenses && licenses.length) { %>

## License

Copyright (c) <%= new Date().getFullYear() %> <%= author %> 
Licensed under the <%= licenses.join(', ') %> license<%= licenses.length === 1 ? '' : 's' %>.<% } %>
