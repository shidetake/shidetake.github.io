Pelican × github pages でのブランチ運用
#######################################

:date: 2015-04-03 22:39
:tags: pelican
:category: pelican
:slug: pelican-guide-line
:author: shidetake
:summary: Short version for index and feeds

.. role:: bash(code)
  :language: bash

- :bash:`ghp-import output` すると勝手にgh-pagesブランチを作ってコミットし始める
- :bash:`git push origin gh-pages:master` するのが基本らしいが、ローカルのmasterブランチどうすんの？という話
  
  - 設定ファイルとかをmasterでコミットする一方で、
    記事を書いてgh-pagesブランチとマージしたらたったこれだけのコミットのログがひどいことに

    .. image:: images/150403_git_la.png
      :alt: images/150403_git_la.png

- blogの場合、そんなブランチ分ける必要もなさそうだし、とりあえずローカルのmasterは無視してgh-pagesをローカルでもリモートでも唯一のブランチとする

