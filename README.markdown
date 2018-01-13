## gitlab-lensencrypt-hexo
Used to auto renew let's encrypt certificate for gitlab-hosted blogs that built with hexo.This project is modifed from [gitlab-letsencrypt](https://github.com/rolodato/gitlab-letsencrypt).

## prerequisite
You need [hexo-processor-static](https://github.com/lakenen/hexo-processor-static),python and visual c++ 2005 to make `gitlab-letsencrypt-hexo` work.

## install
```
npm install -g gitlab-letsencrypt-hexo
```

## use
```
gitlab-le-hexo \
--email      example@example.com     `# Let's Encrypt email address` \
--domain     example.com             `# Domain that the cert will be issued for` \
--repository gitlab_user/gitlab_repo `# Namespaced repository identifier` \
--token      ...                     `# GitLab personal access token, see https://gitlab.com/profile/personal_access_tokens` \
--path       ...                     `# Path to put the challenge file,default is source/_static/.well-known/acme-challenge/`
```

## useful link
### vcbuild error
[https://zongren.me/2017/03/22/fix-npm-vcbuild-error/](https://zongren.me/2017/03/22/fix-npm-vcbuild-error/)
