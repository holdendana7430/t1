代发 wailian999

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gzzjyqpun.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxgtpchd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gfuenauki.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaxesotl.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gbjbbwgfb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvewzomh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gggwvjjta.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gougbjbts.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/ghykqjlgc.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeziwuhr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudxmmes.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpfxjbq.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gromqzpci.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggcyfefuj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxnwfvdw.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnguwcvkr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqldrqzmq.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gltehnkyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghohkwqgx.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtstvlylc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsnaemma.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqitonamj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqlnxosr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkezeqvm.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gcjuzwgzm.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzammcwby.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnuhxkean.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtlfdvdv.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gfcjmwowv.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtmmhfvqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gboebykmp.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxwpponyn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glkkyqhkt.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfskwzrvh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gekagednj.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvqmmypc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gezuonwmx.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/glumroqes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gonssvxgq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxewvoxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/geuxddizq.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnyneznkv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfrpuiml.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydleitka.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpwaapy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqxihpxb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjtfzvzn.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaonjnkmm.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmbqkluc.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtmghhn.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gspwgssne.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxlqixa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/govlzsyll.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcujcdgp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggilkugpo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gapukoukn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdhhsybas.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/grvkvgeua.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gflthlqcf.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gtohxeblo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gonxyabic.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcugfkup.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbaawezm.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqrghcxlt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvzctkegy.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdlniila.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gztqqsmsp.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqwmebcce.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyorppcz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpolkrvat.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glehvfrmi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gctdqkmck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvcpjfoz.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojprnhdb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsbomlwyo.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/guajjvnro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gikthdggm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmtlopc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/grrpermaw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpmwzmdp.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrojeyrt.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/grnyikvcw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwnpfaeww.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgrccaaj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gykmoomji.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gztzycono.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/giufwqjcx.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvebazzi.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdyezhts.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfxajpya.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuihrvkq.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgnkhkd.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjjucuud.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gemevripq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxldvlxg.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrflhzxl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/grxejlqeb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gpbplbnkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gclqslssx.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxujzxsqa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gahsnfsgw.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gtdcnqtaq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gacdypcou.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayayuiay.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gqfpadfhu.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewyuaats.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkqugpxtn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkirebydo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxfnqgjy.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgaojgvo.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrrwkzmp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzhdxxcv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkifduxob.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwxevez.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmgisvn.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhiethre.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxvqjuyf.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqinjiptv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblbshkfz.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbweocwts.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gvypuuepb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsjgbcgsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gxbrayker.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrjovsh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/glfvtkcct.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjcxlnlc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gclygjfuz.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gloaxquim.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/goabrwuyo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gizqkozbk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxkdscvp.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gryeauoen.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/guepraezd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gsospktxw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxwsjzgb.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gpcgmuduy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/galyemics.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gthucfclq.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grftqwfgf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyowepmh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydtqzty.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhbptxcw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxtbqxv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiipwgmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcauvjnwh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfizgysgd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfjlyjv.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzflufknx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gizuxauvz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhgphjvb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmtnopen.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/guaaihtxl.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gytwmhuhc.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzrietm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjwobvmb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grixmghbq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gunpvjelz.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gikgzhiem.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuqrkcvm.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuwtaspf.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/grfduedrl.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gciijbrxd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpejkcxba.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gsmrekcwg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyzopqlb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewkdzsai.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidyftzr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcqnycpr.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyxnspcn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsqfdyoxb.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwbwexxq.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gzvdsysfz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxyljyh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdnblcuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtibtoump.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeargxpn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtlxwyie.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxxqdcr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gnphjdcoh.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdvgopzv.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gevdspuon.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtbogqhsw.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgoicof.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqfdhmj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gfswdkygm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtseceo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymgpguvx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gsigokbpf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gqtaspqdd.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueopyodt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjxktdek.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeggesud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gtbdtrmcd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisrewla.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrbsckzc.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghowgsqgq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gymtrtnwt.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gufwmllrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gsnmozcjh.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/guvctgobt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/guhspjxlm.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdgbwkszf.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gzkpgwonc.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/grddlolwd.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtyobtwnb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gityunnzl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmruhddp.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpqzhgsq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorswbby.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaswpkvrg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggckvyvlf.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gohuotrws.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnajfypqo.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqqbxyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/grpyliume.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjghuvgs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqugqdauk.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/glgiztnhn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsmriqck.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gucpocyfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjereonh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlejgcug.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqpylyvw.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmdhaaqk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvhpttyn.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepzwqcrw.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnbbikai.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtyghntos.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxauqzmj.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvlirzkp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gsortbbtl.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhzkbjot.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/geqgbxtlm.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytltsge.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grunvcwqp.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxkweftvu.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnjqowv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkluumqso.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grtgicbtr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnxdjca.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gjnmxecmp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggemmolqg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfxgdfix.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahqzbysd.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsnvemus.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyuqlhkin.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gfursmvgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfgjzgy.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzxpvlk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvjwiow.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjspxmevi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gspkelcvu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gigdaqeys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/geakhfpag.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gopzjfwho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqynqnyq.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gknxigcxd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/guvpbufxo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/glcidjpxa.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkiplwtv.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqvveugf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjgjzzac.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gbpypccnv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmqrmsx.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqudvxicz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gscgzjzxr.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrrxpxg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkssxfn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjndeinia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvdhgslk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glupfaihe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gpkirsjil.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabxvjnce.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/goquwuseg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/girjkctxd.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhxhugbz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gaoaeimeg.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gziajdtnq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojzofdg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhnoohls.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezjxtjd.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmhhqkj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gxsnfdpva.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ganjgdwbx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwezijrcm.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpfejup.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzhadwii.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ggjphuima.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusojaala.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxnregl.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkhxeycc.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gugwtuqdy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehkfbews.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfqmssk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfykgvlkk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkztbynuz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/guwgwtntj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmmlsfdvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gkgksfyao.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhtzvjme.sHtML


<!-- 参考信息 -->