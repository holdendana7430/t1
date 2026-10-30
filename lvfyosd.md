代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gokthztcp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gbirwlxbj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/goljiiasw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqwmzdvkq.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gtwclkmle.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxyfchimt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gpwuumfro.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ghmftcaqv.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/glcnkvgir.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/guikjgipc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gpvkdlxpo.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnjnupllc.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/glxwtiqer.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gjfwbvdem.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkxybgh.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/glywkjesz.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gdpqtrjrt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gglnyyoal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnhxknuga.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzgryobxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glyftsgrs.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gyuqqeimu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gkbpnnoiv.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ginfsganu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gsgchcyrn.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gbuqfaneq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glypbhsri.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gtkfvixxl.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gccncchpp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwxclijmq.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gtcdfcyuv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gllysqfrs.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/grbfxwktb.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gcjobsvmf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gqaplhbhj.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gxcbcfhtu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvgzyxkmq.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gvoecvdro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjoxtsaud.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gpyngsjmq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gnxrtedvu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gdsjubxmc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gvgzlutrn.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gjsrmicaj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gttklyuqs.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gcsevisve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gzbrywhuo.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gcnejyjsa.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gtioaupdz.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gkyahxdux.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/glsnikirm.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/ghowjfkhs.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gadrflawl.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqzbxfbyw.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gcvlebodm.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gwibzhtxj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gddncwqyh.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/grqclqcar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gzzaphikq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gasbneylz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gsimqwwbj.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gqmsxfosi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gahbsawvi.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gvxqebrdp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqbgcjoqf.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gxvwarfza.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gafytohua.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtpwbldoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gogolvjqt.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gfgznbtmo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gyuwueaku.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gwsojdxtx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gcvvcunhg.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gxqaklqmv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjswrdhsl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gziqcnrnm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gqywkhlvw.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gapbakvzu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gsvsofjgg.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gjsnjtcmc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gauspweol.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gjnkhcdhb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gbptvxngw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/ggncxsmgi.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gvixqiwul.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gvfhqbwid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gzeiyzkhw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/ghrxitgqg.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gbvpmlaix.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gpasijzcd.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gpznbcjmy.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gwgmgasut.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gptgtpnxh.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/goactxiii.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gximujgfy.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gvmnmvilc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gfixdcetj.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gbawjkoam.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gxzfpyopn.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gtlafwrih.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gkiosjolo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gwvjvntok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gxwpslrah.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gawhxgcyn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gohinmjvw.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gggboeerh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gotziqqej.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gufiwbyth.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gtpmusvqf.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gqqaztnut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjjujcogl.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gklwgmbvg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gtoiuivnp.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gipxonqut.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gdaxgyqpj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/ghiyddsma.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/glypauzfn.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gdmburgxm.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gjrbnslwp.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gzecqbvny.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gqrpkizde.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gekgvzzkj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gehlfqofz.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gkhcebhds.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ghvwrtmea.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gibgsdhoa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gqjreeiry.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gvuhrbvek.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gtkhpmbgv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gzfolkffn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gnlxoxjgs.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gyhkxvoxm.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gpxamwsce.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggvtbqadf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gkxvqmpgc.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gsocyrdpl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gadthiodk.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/glyoglxcd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gyvgibykh.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gslcnuemj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gpxgeizpa.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gofmxyilc.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gvaixnovk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gyjpxkjwi.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gccztoaer.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gwtzbyvvr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gothpquai.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gpjyildfz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gurffseic.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gebvjryyq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/grfrqoeob.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gwymwssbm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gcuoyuucp.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/grohiaxlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gitstvvuk.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzyhppsxn.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gfhetvmhe.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/geaiiyyyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gucbrgivs.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gukxcudyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/geabvkpdi.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvpgcmxoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gkmrczdfx.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gsouypqsi.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gfmsxzony.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gyhwknmrg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gviawxziw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gtbfgyqmr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gyiixhske.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gavhjkwka.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzfcvdvoh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfzcjthqt.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gfwwpxzqd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjvrefxiv.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gucmqdicl.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gvymyqziv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/ggcywezot.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gkhqlrpdk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/glozbodvx.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gagbklwyh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gzgmcydro.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/ghcaxnnhv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gmtpqhaua.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gehuyccbe.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gayuqlmum.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfmdziemm.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gkkybgmvi.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gftrpbxky.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gkuhyqpus.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gocgbuwqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbhpsmo.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gqecdudpr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gujkyqmkn.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gbulbwlwn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ggiwvyczj.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gefhaoisb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gryaucrti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gdmddelbd.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gpgaklpkf.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/goxbmathy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gywkyxsci.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gsvoabtxd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gvyzhfduv.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gkkucbtmm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gxibmslxb.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gpmczotix.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gpowtcsfb.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gifrqrbxc.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzlpykbqt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwdikjy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gdkixfgok.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gndhifgle.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/guvshzfqy.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gnrlmhfqa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqshdkkjn.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gxxkzflsq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmsxyrlzg.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/guopsruas.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gsruutsib.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfmkjzjtd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gngkvnzpq.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grfdaalsp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/goknekaxp.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/grpluhhcb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/guuivdzzn.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gsezdpbgp.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gyngtfipd.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gwcgwotwg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/glmmshkhv.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gvynwyoyy.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/grzzqtssn.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/glkfzlpsb.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/grxqrbmpp.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gqzmtozln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/goypujets.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gcudieegl.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ggokcdeqq.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gvrxlmboj.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gftkabgvn.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gslxezqtc.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gcffnjeiu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gaeijtufb.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gobgtmwpi.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/ggeiqcygh.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gsdobpmky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gwxobghuw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/glnmuggiq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gzmqvlifj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gwjwqptcz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gqjaambwx.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/ggalwfpsy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyvydnkqw.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/ggowgadft.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvzocdugz.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtdnkerhl.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/geclxeewu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gsjbpxkoq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gocixwdoe.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gxrcfcibr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gcjjzsbpx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghcdooxxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gkgwypwrb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/ghcpypdaf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gcetslqwg.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/grmkpvmam.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gfzrmbniq.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gvefqpgvb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gjtuesxcm.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/glivpbsej.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gljifnfyc.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gmcbrnvws.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gdwkmgqjv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/glhpagnha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/glcgbiazv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvecujprp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gjeeulnda.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gmszwqrnr.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gbukceakp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gbmughoee.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gsidpcdhk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbbmvnapb.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gmhgyrzvc.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gtzvcsexx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/godjdjzev.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/grvratcur.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gajlykmes.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gxpxzfiau.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/ghszpnrkq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/giywvaucr.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gphghvdpw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gabjtsamm.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gshpimnrs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnfwhyjv.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gryynjnit.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/guvygwydf.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/ggbcpzjlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gvrportil.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gziluzlkm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gejgaituo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gnsqaauyh.sHtML


<!-- 参考信息 -->