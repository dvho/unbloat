# Unbloat
[_Unbloat_](https://www.npmjs.com/package/unbloat) is a powerful tool designed to help developers manage and clean up their Git repositories by identifying and handling files that were once tracked but are no longer present in the latest commits. It's particularly useful for maintaining a lightweight repo without compromising commit history.

_________________________
## API
```js
npm run unbloat
```
## Features
* **Identifies Removed Files**: Automatically scans your Git repository to find files that were previously tracked but have been removed in the latest commits.
* **User-Friendly**: Provides an interactive prompt to choose between viewing the list of removed files or permanently deleting them from the repository's history.
* **Batch Processing**: Efficiently processes branches in batches to optimize performance and reduce memory usage.
* **Comprehensive Cleanup**: Offers an option to permanently delete removed files from the entire project history, followed by a thorough cleanup of the Git reflog and unreachable objects to ensure optimal repository performance.


## Notes
[_Unbloat_](https://www.npmjs.com/package/unbloat) works by scanning the entire Git repository, including all branches and reflog entries, to compile a comprehensive list of files that have ever been tracked. It then compares this list against the files currently present in the latest commits. This comparison allows the script to accurately identify files that are no longer needed, providing the developer with the option to either view these files or remove them permanently from the repository's history. Once the obsolete files are identified [_Unbloat_](https://www.npmjs.com/package/unbloat) offers a cleanup option that not only removes these files but also purges the Git reflog and unreachable objects, ensuring that the repository is as lean and performant as possible. Given the powerful nature of [_Unbloat_](https://www.npmjs.com/package/unbloat) it is highly recommended that developers experiment with it in a controlled environment before applying changes to the main repository. This can be achieved by running it from a local copy of the repository, carefully reviewing the list of identified files, extensive regression testing, etc. When confident in the repository's unbloated state, ensure collaborators are aware before forcing updates to the remote repository.

## Installation
With [npm](http://npmjs.org) do
```bash
$ npm install unbloat
```

## License
(MIT)

Copyright (c) 2024 David H. &lt;email6@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.