# A Collection of .tfignore Templates

For use with Team Foundation Server||Service

Please feel free to contribute additional templates or modification to existing ones via fork + pull request.

Similar to .gitignore files, the following rules apply to a .tfignore file:

- `#` begins a comment line
- The `*` and `?` wildcards are supported.
- A filespec is recursive unless prefixed by the \ character.
- ! negates a filespec (files that match the pattern are not ignored)

The effects are recursive with .tfignore files in sub directories overriding the parent. Further details available here http://msdn.microsoft.com/en-us/library/ms245454.aspx

If adding or checking in files from within visual studio, add the .tfignore to the project(s). If added as a solution file, visual studio 2012/2013 will not process it. Having the .tfignore file on the solution should work in theory but it does not in practice. Ideally any .tfignore file on the branch should be processed on each check-in, but perhaps that functionality will be added in a future update.
