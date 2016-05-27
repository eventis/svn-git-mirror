 git-svn-mirror - Easily set up and maintain a mirror of a Subversion
    repository

SYNOPSIS
    git-svn-mirror clone [options] URL [destination]
    git-svn-mirror update [options] [directory]
    git-svn-mirror help
    git-svn-mirror man
OPTIONS
    --stdlayout: Repository has a standard layout, with subdirectories named
    trunk, branches, and tags
    --branches=path: Colon-separated list of paths, relative to repo, of
    subdirectories containing svn branches
    --tags=path: Colon-separated list of paths, relative to repo, of
    subdirectories containing svn tags
    --trunk=path: Path, relative to repo, of svn trunk
    --rootistrunk: The subversion repository has no tags or branches, and the
    url supplied is the trunk (i.e., there is no "trunk" directory appended to
    the url). This is the default, and the resulting remote branch will be
    called "git-svn".
    --exclude: Perl regular expressions, separated by ':', with which to
    filter paths when fetching.
    --prefix: Insert a prefix directory into remote refs (e.g.,
    refs/remotes/svn/trunk instead of refs/remotes/trunk). This can be helpful
    for disambiguating branches in checkout commands. Default is "svn/". If
    you want no prefix, pass --prefix="".
    --metadata: Include svn metadata in git commit messages
    --authors: path to an authors file
    --verbose: output more progress information
    --git-repo: URL of Bare git repository to push to. Must be initialized
    ahead of time.
    This was originally lifted from Kevin Menard's fork of James Coglan's Ruby
    Gem svn2git (http://github.com/nirvdrum/svn2git) and translated into Perl5
    by John Ralls. But the original code wasn't quite right for creating and
    maintaining a Github repository that mirrors a Subversion one in which
    several developers use each, so John Ralls (the present author) has
    reworked it rather extensively. The sharing set up is due to Thomas Feris
    Niclaison's blog articles, the most salient of which is
    http://blog.tfnico.com/2010/11/git-svn-mirror-for-multiple-branches.html.
 
