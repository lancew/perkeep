# Use Cases

First, read [the overview](/doc/overview.md).

These are some higher-level roadmap goals. Only the first few are done, but all
are various stages of implementation (as of 2013-06-12).

* **Filesystem backups**: easy initial use case.  Since you can easily put
[files & directories and such](/doc/schema/) in Perkeep with
[pk put](/cmd/pk put), you can use Perkeep for your backups.  Incremental
backups are basically free.

* **Efficient remote filesystem**: should be easy to do an aggressively caching
remote FUSE filesystem.  Read-only is trivial.  Read-write shouldn't be too
painful. Every modification would be snapshotted implicitly, so revision
control would be the default.

* **Decentralized sharing system**: share anything of yours with anybody or
everybody (private is the default).  This is already starting to work.  See
[sharing](/doc/sharing.md).

* **Blog / photo hosting / Document Management CMS:**  I intend to run my
personal blog and photo / gallery hosting (with permissions) off of Perkeep.
I also intend to replace my "scanningcabinet" document management software and
use Perkeep instead.

* **Decentralized social networking**: a lofty but persistent goal. For
example, to implement comments or tagging: One person could use claims to
attach metadata to another person's image blob. The signing lets you verify
identity.  The sharing/syncing semantics of Perkeep let you easily save a
copy of all your friends' pictures.

* **Import/export adapters for hosted web services:**  Don't worry about web
services shutting down or going downhill.  Mirror all your data online in your
private store.  Create it either in Perkeep (using open tools) and export to
hosted services, or create content in hosted services and continually mirror it
back into your private Perkeep.  Relax knowing that your data is yours,
forever.
