<p>test!</p>
<pre class="language-javascript"><code>const octokit = new Octokit({
  auth: 'YOUR-TOKEN'
})

await octokit.request('PUT /repos/{owner}/{repo}/contents/{path}', {
  owner: 'OWNER',
  repo: 'REPO',
  path: 'PATH',
  message: 'my commit message',
  committer: {
    name: 'Monalisa Octocat',
    email: 'octocat@github.com'
  },
  content: 'bXkgbmV3IGZpbGUgY29udGVudHM='
})</code></pre>