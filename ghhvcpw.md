代发 wailian999

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gszqnnpun.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/genvsxpkw.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gbmtvswkh.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gsvdvjuvr.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gapqffqcw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpiimeq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjgxfffq.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcmahguf.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gxcnaqcaw.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdumqicgz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gndivlfsm.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gamqtanlw.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkaudfvol.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gejcqeynx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvurpjkvz.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbzxhuumw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaludelz.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gldepcian.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gayjnnzsa.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggtlaaft.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsmhmzjuz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvytvubln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuenwqeg.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gqeohcuyk.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzueymkos.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/geohbovxl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwojasi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmotowmq.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/govlunwnb.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkdysaok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gteaycvcz.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/grnaxxaot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpdbvetv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/guffhsnzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gywohxpws.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grvtvujiw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggycjlcvl.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gferijvtf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmlxautk.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gafmcjukt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcqjtegt.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gitmrdspy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glniessdh.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuzxstgb.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlcjwcb.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gnayvkpsx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grkkolala.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbuydyass.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgqagbno.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gaelvrcjc.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjfjdqq.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghuqicbbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glcifgumf.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvlpazqg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwajezwf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/grykkhhvx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfkopwalc.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghodektdy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gccnuifat.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkufhzoq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gvcoztixs.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjjfnsuhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqhdusv.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/girrykqyi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuphibix.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gribrpueg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhfpkdsi.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzvxykjrb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvpzprmax.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdjijqh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobtvmhc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqnpyxit.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/grfnceduy.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gdottcsxu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyxeqyzc.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gdqdeaddr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbixrxwll.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/godycidqv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwriklrp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssodawxu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpwplhbc.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gawfffqqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzetoznlu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqbjgbkb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/geoaqwtrg.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazmipumb.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbanjmv.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdqmlpdic.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbyhwuiic.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhvzofbd.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqonuatd.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giahfsyvx.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsegtxmq.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/glypkgivs.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gypvmabuv.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjpixagaw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gcmhsyqqk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gfvjmatua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gaietnhmr.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gehfedaoa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfthdptud.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvmpeeju.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gegjzjegc.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdnidfmq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gurajzbmk.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gesnvmaog.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guecxdcnp.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ghfekktol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/grzddzcqs.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giswakpsq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtagqaacs.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcquctj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gefrlcrbg.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktckedxd.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxreiufsv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjiaorgc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gkgkqkdkf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqafzcni.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gzacwfcts.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gwqijfnio.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynytoqnq.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfrmyrqk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlnjihqv.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gugyfvyfu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmftqrbii.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxzohuvp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/grognxodf.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwrfltfh.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gojzsxeea.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfwsbewk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvrbvpdd.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gabrwziih.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gqoayawix.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gghdoaqgg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbntxwas.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbzktjuwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gptbivees.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ghiljctmf.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxxfvgdv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwgyvym.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijcyvbpw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmuvqfrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewirtel.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/guouphagf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gpbyarvuo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhxcvjn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwgptocq.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpavnpbfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvirhvot.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gudrkiggl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxxfpglbz.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/geygqvsqk.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ggawdvgbb.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvytnlph.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grxznzgez.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghonhhkbw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhorvvrk.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdgasqwc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlftnrtc.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvtwutew.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ghggsytxr.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwpxepeu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbyxauaiv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gplwsnoxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgisvlde.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gdskrfera.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gxrpxsjyn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gspakgjpw.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqhrqazh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gypgrasvh.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grjnbbzwj.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjvkbys.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gffhclpjk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gynyasmmg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghggztms.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewjwjet.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgsecwno.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gurnhpxrp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyoxgmbi.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorbhrkh.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggyyuzlym.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvxbpfib.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxnmbyzt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmlmaglkz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gqbiduecf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/guefqpcek.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimhcuhnm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/glubpmvri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalhityo.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/goifwaavl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbaxrzjc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiexubnu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfsbvvbx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdagfyvmb.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gyaxyvbwx.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzcrcuth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvchbttpw.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyheqpmv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuhnzjao.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvzrazw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glnoyhcrd.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glukdcwjq.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gueypaofm.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzlcmuqo.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbefngxrf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaqcudax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebjiavi.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvengvlaf.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/ggajnxgtk.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcfvlhdrg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbymthn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gpnguhjqv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggykapuyu.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gschfbgnv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtkepnjhi.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gaiindstp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyfggjme.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/garbvqbli.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnqqzosg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfylnaxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccwrqwjx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysjvrhee.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gbeawnsgt.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gynaybckz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkskrbms.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgpvrzij.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glwbmcqks.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunavtyj.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdsygjpk.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/geqzzazyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gnsjytlxd.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/glvnyyzmg.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrfmjwbd.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdxijmvx.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gdqpfsgeo.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqwcdhu.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/giolhivyx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqqbkxtz.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gclqgefds.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvkjtrdb.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gwllxuouf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjxzfbsj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzlfqzqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjectxdui.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyayexein.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofhrxana.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnpjolsz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcuxqayc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyjxycqj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfarakkxi.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtpsnedo.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gqfsdsocr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grctypkpe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gcsczmsnv.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grxilgdqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gewvhfoww.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghulbrpur.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gseqlvqid.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giwpivjly.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnvfldla.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfukaqsb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsttcotmc.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyevhmup.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsloxbhuf.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/ghpbbtvqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtqxxfos.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gulztgevp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gielgjnpa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjdjcsdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvycffenv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmhynvrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsjgdljr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsckiejp.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzzwutuvg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gttupznvx.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjrenfgx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gaeqivwlu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuvtejvn.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbsclrfrp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtbupvq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdxkrupk.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjhynprt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gradrqkzh.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gluevmmfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvakduij.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/goazoowke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxxewwjb.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gdmugpllw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxsyzikri.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/glqxitldk.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtjsaxnp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfivtoon.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkvbqaqqd.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gvtwawhom.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/geqnsiefx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghaqhpaqq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbarmnxzm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgeuloc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grglejvaw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtletskkg.sHtML


<!-- 参考信息 -->