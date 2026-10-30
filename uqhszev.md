代发 wailian999

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gquhunxmg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggquszllt.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gefiehwye.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuesmpjk.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqyadmww.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gwkdurbyk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarcgwep.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuvoaru.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gogstwniw.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/glksdbqtp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtayrnqi.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcnppab.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcqkrafus.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoukfsnh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtzfjcej.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gebbucuvb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/genlihvby.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcvjwvkh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geisufmqf.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtolgxqmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdrgnlrfl.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/glwvhvrpg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdofwkdbv.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwvjfilf.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gellevdpx.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzemxjirt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqgdafnq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gojbttkge.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghewnglax.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfjmltzvc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnpbuvo.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gztipfphd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsfgworjf.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gmtinlbds.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqbvozvia.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gopzdotzf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggozojmlf.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdxqcpxqg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqyzmgzs.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gykodgjkf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfmkjheuv.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzfhdnlk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gicfambou.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/grapfpwfw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqcnjjge.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grhjkghsk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzdkrro.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzfomvno.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjbfuzxh.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghftjmqyh.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnuwylzfp.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmvtbskm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggkvnbcms.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/govkcvvie.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxxmdyslz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdmwwxqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/glmvylibq.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaehomkp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gdlvleatw.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfnsbukf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gmkauwope.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoewwkwn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/giejvzufu.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijeiydns.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvdkkqqz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiuwveao.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqhkzavo.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbnlecsxg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwsnvmbu.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmrvpwxgu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbiogmtjq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezpdxfrg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqqycum.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/giswikskf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/getvfpock.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpdsmdnw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glczrkale.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gubquvhfx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxuwqbri.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtknesjzk.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gohytoakr.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/guzognvmi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgudewnu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/grdyhpggb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/giragyknp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzxsoka.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gujvvfvin.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmujbnjy.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gluzdjmng.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gbucxviaf.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftagflps.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnvmftiv.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gipbqnkqi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfvikntk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhbbbqlw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukmbngdg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmzekdh.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gnhecibae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedlvifin.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoaytuyq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gokhesoee.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpphukk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpozuazda.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvsjseso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/greguemxp.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzvjyhqz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfccmsyhm.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ghtcczuuh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyfbocbm.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ggtfkdnjn.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghahxttlv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/goaumwqpb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuldxebg.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcntmcvc.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfmvjmpv.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbpxthdf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgldlgmp.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxzwimck.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjavhzqd.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnthwjbl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytwrwlwd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/golqvujld.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gttwgvowv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gyecrnpnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcglqwz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdcuaapv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gkxbdgbci.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcivvmfwt.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtsfbpn.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/geixuubfn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/giyjifnqf.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqnwpddg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchnexsx.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gepbxswrk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvtqwkvv.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gsnuphpoc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprxwwnto.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gchtmdyrj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzipxcqsj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjntxpn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgjqzpcn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gjuccustt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzdepnzof.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbiaizcf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbctjwqep.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gomvjlemz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gjnhllgeg.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghuotihjj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuukxezo.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/grogguodg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnkjuikyb.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqmeiru.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwovzncv.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gshyxyzhe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goafvrxez.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdbbhemjk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxdevdtq.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcmjrzjni.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmsusbfe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxxwmrnx.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/goehlykfr.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnjjsohtg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gftilxpqn.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gpxlenfpb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjhbwcuyn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnfariq.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjlcxhwi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhhrxzzy.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmbuuudf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpgceemg.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/geyhjqvar.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkuhrknt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdnooqkw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjnridj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmemcvtm.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiscbvke.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grooxqsrh.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gznbopntn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjfyzbtc.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goxxdlvcr.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvciydc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnevdbvgu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghghffflq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxhfmlbm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucawafz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrscnsis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdndtvw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gdwcumihm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvcmwrv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlgfnlon.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gfougrull.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyyyswvl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqwnwjls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibcmowkj.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gghiphxbf.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdpxdpjh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqbzckwb.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghhhzfkld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gczirqatd.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghdoojzrj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtivvjzvg.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnakciwri.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/geowzqcyg.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gupcmgoyn.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkfppwror.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfksqgceq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchtxqgtw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/glifoakac.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/giuwyiktm.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvsqkhfd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjpiqdnj.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/getypnujv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gxisobipk.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbnzidmr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxkeerxd.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqnkffls.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpksupgoz.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplrqgqvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gaikdjgws.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqazznpxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbuqhzov.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gkltnsxpm.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeohzrrz.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gqmqetqtu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvwxscuk.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyybqmas.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gddtltgvn.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxrekwuf.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grwclqswk.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnffciue.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gvglvoqbd.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gcqfmqkzb.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkpzqnfa.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxbhggcp.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzyqizcd.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gokdbzuvz.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/grphkyxxo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxvrvmde.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcakgjrh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvrprxhx.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gttybvmax.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmeyypmr.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/giviwbfae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzefzimni.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlrnuql.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggepwxgoh.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghimodscm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuwipmcd.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvvdyzxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtbxtddi.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaalkjzy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gcsiclolt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmejxscyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxfklmkf.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtuypfhtr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixkctbuv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsegrlnfu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgtawppt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnryueujs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/genrkypue.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gyrljzcjt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvepthmw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ggjopwhow.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gicjkscbb.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjmeegy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyzdyzetg.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyoiqzha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gezzigttx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjmfwnfta.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gawddaklm.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvddyyiht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtidhhzuc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godfuzhte.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gagxrywai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjttilztz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsupjpwmn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwnjhcviy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuhhvmiu.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gobxojskc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gonifygde.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpytxqlf.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgnumktv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdlyursb.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpgadddxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtkkfheg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwmszpme.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/grsdohdwa.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/grlvtfdjt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geloefuvl.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxcbtpdr.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghpqstknc.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdcaxctjt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxjyyfbh.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gzdtukfrs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/ggkwumkik.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvzxwax.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glgbedfqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmspzces.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gznutrwfw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsalloaji.sHtML


<!-- 参考信息 -->