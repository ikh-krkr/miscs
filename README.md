# Description

This is a repository where I experimented with the difference in GitHub's difference visualization when files were moved using the "git mv" command and when they were not.

これは、「git mv」コマンドでファイルを移動した場合とそうでない場合で、GitHubの差分可視化上で、どのような違いが出るのかを実験したリポジトリです。

Specifically, I used the "git mv" command to move a file to a directory and then verified whether it would be recognized as a difference if a change was made.

具体的には、「git mv」コマンドによって、ファイルをディレクトリ移動して、その後に変更をかけた場合に、差分として認識できるのか検証してみました。

## Conclusion

Even if the code was moved using the "git mv" command, if the amount of code changes was large, it could not be recognized as a difference.

「git mv」コマンドを使って移動しても、コード変更量が多い場合は、差分として認識できませんでした。

## Evidence

When moving and editing without using the "git mv" command.

「git mv」コマンドを使わずに移動し、編集した場合

- https://github.com/hikeya/test-pr-diff/pull/1

When moving and editing using the "git mv" command. (commits were made in one)

「git mv」コマンドを使って移動し、編集した場合（コミットは1つにまとめて実施）

- https://github.com/hikeya/test-pr-diff/pull/2

「git mv」コマンドを使って移動し、編集した場合（コミットは分けて実施した）

When moving and editing using the "git mv" command. (commits were performed separately)

- https://github.com/hikeya/test-pr-diff/pull/3
