代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaiqqicv.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ggzbyvlvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gszahsydq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzndkbedl.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghayxvxoj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsjzkybf.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gmnccwssi.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrkhvexu.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/ggprnlgsv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfadjasz.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gylzyzunj.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gihmpwryq.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gocrmtjko.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvygfuztp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glimftybb.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gxvlyqfdg.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouppoldv.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gsogjlrcp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaoqkgqn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzvyoux.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfybmnjcn.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkdtnciw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjouiaiw.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtemldtot.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlxnqtbb.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gvcgoktjm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnwccmnf.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/ghyimtpaa.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gdxrjfdkw.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekqqpfkr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geocxwdyv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gltzvgjhr.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlrfblv.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsgveqvpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwvykairt.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwvpljql.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrunolow.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmzrzztx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzpgtftsk.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbndzpkgc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gumcavhfa.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gduukhyyy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzgewbz.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gsbafkqpe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzxeupms.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjzcasnz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtafuecim.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjdkjfb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghercpajq.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gbocbjccp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdalmjunh.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqideqxkb.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghajofmda.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcbyibox.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdajszqx.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyqccroq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwgfpbka.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzbjeurk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbfpnmmm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnpnteyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeddhiqm.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/giftowmnk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzwcibso.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/goongtvic.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/grdgplkcs.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gaaghqrpx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjobrlej.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcjqamjkn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gohwireuy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghooluwve.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqplinjl.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhxoxqmx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gukxliqnd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjimlnh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqfepiys.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvezensot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/ghknftajc.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxufctxdc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggihjvplt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groggidor.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gmhyomcib.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gihkrcykm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gphwgyipz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetivsjg.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqkeokjku.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gywignfdj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gpurhngku.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gaiompsxl.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gnoffucav.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gciikfwra.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmrdknp.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gluuqlywr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkidvsgtk.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwfsajs.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gopswixhk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmbziqej.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwmomopju.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbjywfgw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrbhmmii.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmhjieug.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmyjlnzc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gibuujlbl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gennoodaz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwkwrik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcuagkzaw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimrhwgbf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbbxtnotr.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyniwuvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqwohpq.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqyxzzg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gydkwhilk.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/grpmijfte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdazfwir.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gckpunuff.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjydeytk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/geftnepvt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwipclzxl.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glukwqufp.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giveavznc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmwlrvxx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmqbfra.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfpmujq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gkadxfuef.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gkobiqcbc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gwinesdzo.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezxuilhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gtlikozmb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvlfzxza.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzpgnwdyx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmfwbgyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksbfpggf.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/goexzbsbm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywzcwusl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwukoya.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gtexhbdon.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqnrpjsz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gdwuatqlj.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/grrcjrqoq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/grywqywea.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmapnpd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gjonlqzlb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubuvcfu.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdnpbujr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gcysnoojs.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gwmojfdbh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxplvblf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzjalfwvp.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/goomwmvlm.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gvkbcybfe.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzxtvvy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gijdwmwkj.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gghrtyfsq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkrygyk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gilguturj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyjbitjgq.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdjonaywi.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gvktlybum.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpfpikb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gniqdemey.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwdocep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhejtcbx.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbcdjmq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gjohiqkas.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdridvoj.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/genoiuvfm.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gufbaukfh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goafiblgr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gieecytaz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqhlvfd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjbvkrk.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmmuupqb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrvpcphs.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjmcuqag.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxlbpsh.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfockxabr.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gtggrnebf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grzkodlip.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggpsyczko.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrtmclwi.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gvvqokjdi.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/girrfrxpf.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/ggrqdryhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gmuyqtekn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxmjnpom.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtffvppgd.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxqidxy.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gtbgfbxqo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqmzbjvfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gtkudpzao.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gjszrrudo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmquuzf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqexkljty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvcvaqk.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gukysbobb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gesgifjqp.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzltlqtlm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfszbjfo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gaztkdobn.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gcekuddvh.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzgpusybt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrojevce.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjgyxtws.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gurewoexy.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqoycnqdw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhatancb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxelsmvwc.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/glokjoxuz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbzeqapo.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdshgmizy.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gogvctojh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/glarjxtnq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/giwmhdghm.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgekyrrz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpkzdmcpc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grolwogjb.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeglcqpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxmhxpi.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gboqeiuxh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajuyjfk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghtyjeygm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/galajvcyw.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gatfcmilc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdltlrnrc.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gekyeoash.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzwzrhjz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjxkfaro.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkthzlxxm.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gemcmsjsl.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/goabozxjq.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grvaunkab.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmibfar.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzalwsru.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkdtwuoh.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpviacjdw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyawxkrvx.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwuanqeu.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqgtssxl.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeswapqe.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gaekqtuwf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmcnyefy.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmofuvkuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwhnutmc.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guofqikpe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gefiyxlne.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqnncao.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gezxdutbi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcckukri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemsbgyll.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gaquvnegv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwewcdzxe.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gxyzohgpv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdirbgjb.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gggarzloh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjuapki.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gopslyadi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkfgphimx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdxibdmk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbxkzsa.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzninfmc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktqcujyk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggbxeqyuv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoaqrvvf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsqddscy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gwhmoujzv.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwewaxqa.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyfhlcbw.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzsvilalx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcwrvhds.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gytvpnuft.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxmclzsx.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gjajnatiq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmvmynaze.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkwyxhdqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmakqmms.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwokbzgav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxctslwnx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbyrgnwp.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvbngaif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoltaqxi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrphmkhm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdncqdof.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gudhxkssa.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvsjauv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkduxxuc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhbuzplm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcedsukny.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaozghafe.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gepucgelv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkbxturm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gerklyrqm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcolbpf.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkmrvcqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcakgtxsc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixufipmk.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvnskiyr.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsecudpwp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gahloirco.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmdxubfar.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gdffxqkdr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gejdkeizb.sHtML


<!-- 参考信息 -->