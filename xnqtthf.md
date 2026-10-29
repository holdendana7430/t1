代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gotsywcpx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gpivlukjj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmfvqcpse.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gdyfmknyq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gxxxlecbg.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gljtnnfjl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gffdwxqis.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gklkpgdcg.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gdgbgecok.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpyhbypdb.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gvkjurand.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gvrsqugos.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gocoousrz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gxiekimtt.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gizicxpbl.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/ghvperqek.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/ginmqesfi.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gkojbmkwl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/ghbusbies.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/ggpekelhh.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/grstvmjmf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpciwujwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gclkyrtcb.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/ghwvoeqtz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gxsppnsmo.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gdnpisewm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gtyemgqaa.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ggikiowsx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/goquysdwy.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/geagjqryz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjykvupzq.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gnfvjihzb.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gvwbvtyhg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdyqnsdlb.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gqrgcjfmx.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcbllkfec.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gdmvfszsp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gspzxdqhe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gkqnnpjrr.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gfqyfwamh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gmxpcdsnz.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gqxcmrinc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gcpagfyed.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gdkuhihzb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gkajafzft.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gayhcdrcm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnclboscx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/ggnspiuec.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gewdanyde.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/ghbjegvyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gazeqeigk.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gbgzbretz.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/ghymbbsus.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/grkbvhgoz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gblpqfjxe.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/ggnbrzxfz.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gcemzketd.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gmrnutgaw.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gvphyndto.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gnddmwthy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gtbwyaguz.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfqoaaafu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ggommuctz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gqfyrhobs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gsvwcbxgh.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/ggyjukzhs.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ghdolkjuv.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gslabgrrb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gpyresqjz.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gjyuplghi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gzfwlwnmc.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gkyjrmmwg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gzrzfppoy.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gpbpjuafq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/goyrpjkpv.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gaejzgjtv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gepjbkyij.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ggchmoflq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ghbphpyzy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gfhezqzzm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gitijydvw.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gimpijjpi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gcxxxpdfz.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gahwpacfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gjaubhigq.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gggryiube.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gzjfzeppm.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gkoeqpqvz.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gqbnfihvw.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/glvhlkdzm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/garazdqrg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/giteencvh.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gfkhxkrtf.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gtymwlaib.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gywvtfysd.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/ggaowtoqx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/glfpypadu.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gnchtjywi.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ghjdqktsm.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gtjnrdcll.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpymzznpu.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gpeeoaizb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gegsvnbwp.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvqssgkcm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gibbgeveu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gmvtkqqbw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gbpheedjs.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gxcwnqcbn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gvnprlhbt.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gcspfgewh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giyrieniz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gpihpbtwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/giewhdnhm.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/grhouoahj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxnywphuf.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gbjpxmgql.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gyjgzchgl.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gzazbxnzd.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnrzwfeyd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gwbzlowbf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gcgsqeyap.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gluidnqer.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/grfdoxsqf.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gqvvhmgcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gnqivhsoo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnxajpcyt.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gllfsbxhg.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gkgxcmoey.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gkfctfegd.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gfibpvzfk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gsccfrofr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpapbjpdh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gvruwkcab.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gmxyuagro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/ghvaoigba.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/glqsinnjx.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gikhfzonu.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gvkgyqhfu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gcuulgeni.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gtjrspmrq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gcbghxfmm.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gsiiqwmiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gmprdtmae.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gmfptslzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gzztduhkx.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/geiaeobve.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gclcecgwk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gttqzzobt.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gcgefhaeh.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gdzsviohx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gkkkcjvbm.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gdrxcdmsy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gxiycabhl.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gzlfsrsxm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/grttorgsz.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcvixjunf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gmkjmbask.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gjwzodbtw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gmgtgyatz.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/grrittbna.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxpopckio.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/glssdmedy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gekbfufax.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/ghaqrmwtn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gajjtbmfb.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gujbysibi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grmszycmd.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghoquemov.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/geewubbia.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gptfxwwiy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gygfhgasy.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gubiefbhz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbvzhds.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gnxtndzce.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gvthlpodd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gomaqneng.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gqyfkwbey.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grlavxsto.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghpmlxocs.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gxnuvhsft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gfzrinskd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gydzqehom.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gewfmbszo.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghzmotbdd.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gkqnzcwmf.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gqhyeclva.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gmlzfuiid.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gtcojizwp.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gvlmrahqx.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gvqfincoc.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gmnerhxyp.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gwqqovqdr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gqbqqhizf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/ggigrrbfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gmxglukze.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gwpisckzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gobtlczub.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/geoarldgj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gcgkdekrl.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ggbnrlkbh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gjgnjypxt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmlhcwygi.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmnrschdz.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnppjlyyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gvwufoetm.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gymumlfpo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/govkedvnc.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gktxtalol.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gxachiuju.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gjxcetvnp.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/grtfcfcqu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlaxerx.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gbmohkvnf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gmtrsofyf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gfbybdrih.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gccmwhwkv.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gsoydecvq.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gfgsgvtlm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gevvkjxni.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gbplhwkxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/grchzkdnb.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/guxathwyt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gisqvnpks.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gzcabirhn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gjarrggfj.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gleqksveh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gnymcdzlm.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gscqaqjag.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gasmvhhpo.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gfxcudokj.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ghwcbiimy.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/ghnacycsg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gzwfpkpej.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/ghrqibhpx.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gojowxlxa.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gqabadgcj.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gzortlcrg.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/geycxvsmm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gogdwvhkh.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gommpoqyc.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghanxhmng.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gycpwebdc.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gqmwzuwuv.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqrtdvzml.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gqhodkxko.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gzjfqcurf.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gchjmwxzc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gdehjioqq.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gjixqflps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gloqajghh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ginyobtks.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gshfpinko.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gpplxrxfi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gurqkwecf.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/ggrztpsrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guhjzoudo.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gebzqzntb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gtlnybpjc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/ghykfacju.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gvmewcvtj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzpcqaejg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gmzqsvzea.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gxgwlnslx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gdznadsvw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gtpbfjkyy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gvinrcnfg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/grougnfxq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/grkkyalfv.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gcnapwibl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gisdhlvsy.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gsmtdzvyw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gptrnzzev.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gqymbmdkk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gyhghlkvf.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gwbwogfcl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gydjlbyjt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gphaxzvfv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/guzyrgihw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnmswiitp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gsnlkeyxc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gdwegiybr.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/graipofiz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtitnzopz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gvksrsyrj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gubzwmbsb.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/geqxkpgul.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ggntzthrg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/ghyykzgni.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gqvwdwtfv.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gfytylftb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/ggwaqbgyi.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gdhelnmgi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gecpoaosq.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/geleedqaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gbmcbuqag.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/ghchcnosy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gxhefgsig.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gvlhfyvni.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gxdhjyynr.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gqdfzktdo.sHtML


<!-- 参考信息 -->