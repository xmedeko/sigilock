# `sigilock` - Simple Git Lock

Proof of concept of simple Git locking implemented using Git objects.

Does not prevent to push commits with a locked file by other user - it's jist proof of concept. (Note: that may be implemented in [`pre-push` hook](https://git-scm.com/docs/githooks#_pre_push).)

See also [How to use native git as a key-value store](https://graphite.dev/blog/git-key-value) and [Gerrit NoteDb](https://gerrit-review.googlesource.com/Documentation/note-db.html)

## Usage

Lock file:

```
bin/sigilock.sh lock <file>
```

Unlock file:
```
bin/sigilock.sh unlock <file>
```

See, who has locked the file:
```
bin/sigilock.sh show <file>
```
