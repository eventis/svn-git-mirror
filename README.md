 git-svn-mirror - Easily set up and maintain a mirror of a Subversion
    repository

SYNOPSIS
    git-svn-mirror clone [options] URL [destination]
    git-svn-mirror update [options] [directory]
    git-svn-mirror help
    git-svn-mirror man

    This was originally lifted from Kevin Menard's fork of James Coglan's Ruby
    Gem svn2git (http://github.com/nirvdrum/svn2git) and translated into Perl5
    by John Ralls. But the original code wasn't quite right for creating and
    maintaining a Github repository that mirrors a Subversion one in which
    several developers use each, so John Ralls (the present author) has
    reworked it rather extensively. The sharing set up is due to Thomas Feris
    Niclaison's blog articles, the most salient of which is
    http://blog.tfnico.com/2010/11/git-svn-mirror-for-multiple-branches.html.
 
