GithubUsername/Reponame/.github/workflows/rclone-sync.yml

 - No wiki will be provided.
 - The code is only for those who undersand what they are doing  

:::caution Use on own risk

This may **`ban`** your Github account. I am not responsibe for any such doings. 

:::

```
name: rclone-sync
on:
  schedule:
    - cron: 0 */7 * * *
  workflow_dispatch:
jobs:
  rclone-syncProcess:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2.1.0
    - name: Rclone Install
      run: curl https://rclone.org/install.sh | sudo bash
    - name: Inject Rclone config
      run: |
        mkdir -p ~/.config/rclone/
        cat >  ~/.config/rclone/rclone.conf  << EOF
        ${{ secrets.RCLONE_CONF }}
        EOF
    - name: Rclone Sync
      run: |
        rclone sync onedrive: googledrive:
      #  rclone delete cok: --include '*.{html,url,jpg,png,srt,txt,exe,vtt,torrent,json,nfo}' --fast-list -P
```

 - [Author repo](https://github.com/tianmeng-xiu/rclone-sync ) 
