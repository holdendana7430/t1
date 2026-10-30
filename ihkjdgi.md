代发 wailian999

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwhtjlm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwmhqhfh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goauubhwm.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gxubloujv.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiphtktk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkltvrwic.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhenvdsa.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godikaxro.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzudqludo.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmrlnafq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/guwterjko.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gntmdtrpy.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjgklcvi.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwzaebygc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gikbuhuui.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkhhpxp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvtwbgpqo.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gweblsawn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdbwqmie.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdghgoiix.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfwartmrg.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnmdusbzt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwoljpn.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/glbtyzglq.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/groxzsxke.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkckhgwdq.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkqfzzoia.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gppskmlpu.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/glkpslfvz.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guplksgnh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggryndamj.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gugcfgpyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxrpxek.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwpvgfh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goswglfnt.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geddsdhyd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfeacqks.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjkhubmr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghngkhwzh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdliwiwzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfvvghmwa.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gnptatyeg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmordsac.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkieeydma.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqfodlf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gpdjrouox.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdtltyuvt.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvqacier.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gakmfjhqs.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gimbgarih.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwbflvsvm.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjumyjazg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdmzscb.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutptjpu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxssbpmer.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshrstgw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcdkopiq.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpnodwqzk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gxfaxgtbk.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gjfllnavf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtabkwmo.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbtpdvza.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyskqlqp.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfudalbrv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtkekrtvt.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grmmjvvfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmdgoneta.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdfjznwnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbiboliie.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivowpvm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbsfftbr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/govgsurls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gdbyiqteh.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcigrvnip.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvtoiusf.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gcrhudvgm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grxldftov.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqavnicyk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfjxpsdg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjdqiyls.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvygcnpt.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gncqxjjom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/goxanzuxi.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkmjhre.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/giiagqzmx.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmzguetpp.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkmpmdefc.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggtmfzilr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gebawzfub.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsxqkydx.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprkdcslu.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcncnnkgq.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcpyftgy.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gbmumxzop.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gqnahkbdi.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gpswwqgpc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxlxwugp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gocivvgsq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gadmvocvk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpmcqqsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwbpgxes.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzezvrg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexplarmv.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giezclepu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grfxtvrek.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjtzdcgey.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsdrkgz.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjgprdam.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gasfcuznh.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gaussgmad.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaicquty.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gjlrqrgyc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gnbieunbq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkaqzzrt.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaokgggwa.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/giyqwuzee.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmwoyqz.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmsfjton.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrcrjuw.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gsccwjpqt.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/glewvpipd.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gncokcfdq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gqdtmnakd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwdfzadw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/grtgzpphl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gjykdispt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gosvqgbld.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkbybdaw.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gmwfmekio.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gctoeguia.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwpatbbbd.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcopwcvx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdecgde.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwzawjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmcjhiz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwueegjb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflmdfdma.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/giclbgjis.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrojedlg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfwalqu.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjsvztk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgzyqvng.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvnzrovtu.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/geherfepw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxkamypd.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gjqkmkckm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcketfah.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdpsomrkd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpspxixaf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gaokccrqi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpviyqewn.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzhubqzyl.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gzugbzgbp.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gvplckljj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gityvnfwy.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/glnsxbwat.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gkpzyfvcz.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwfpsmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gqbfymeob.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuiofxss.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/glodevwmi.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gehzhzzjw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmqrugaa.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzcuscef.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyotghnqq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gkgrvhmpx.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/guzswdotq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gprmdqzth.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gaurdvdan.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtstrqcs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrbmgtfi.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmnlzbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gelvqyejg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfrcylyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqougxt.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gezcftqft.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlgomgib.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqjrxwud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gddllizfu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gmnyeekwb.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktqgxgg.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkytwiao.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gxygisfnc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcizzmii.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgbnolua.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gggknwagr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqzibugz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gresjiucw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoflwlk.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/grhrjzymz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabuzooav.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvipozrlx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhepccot.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxovxpwov.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvmyqruu.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaeoabhc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gxamclygy.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdoedzwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gqcwqfwkp.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlqcbjpy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzqpkbcn.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grvauqegv.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guhlvxykx.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gntzsajud.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdtweefba.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheoeglxj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjryuxur.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gebyvokze.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklhfrtuy.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnbcbkmgh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grafaogvq.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqctqnyxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwvwczzm.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/grlpsgyfq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccbcgjvg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/giysykyvk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsyywyqw.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ganzyjjsv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gmbohqhmk.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gasckhbnf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsqzher.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goquwmwfq.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gctzcaqqx.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdsngxyn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslttrrda.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjayftjyn.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrofbmzn.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grfhrtkoh.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gibuonwxb.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvadtgkjw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gmeqnbuwd.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbucasx.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdzeevjvh.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gyvxnhwnn.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihvfrdlf.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpscgliva.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvnadhnc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedlvejmd.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glgdvesft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqmmtqjc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gaekvwiij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqrbzcn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwjjfmmm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdeaeyovk.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkitpyh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbxkzhpt.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzcdsqtax.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqijntt.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gvycsfpwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/goaambthf.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnaabjjix.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gzrlyzafx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvskclib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/glwviqchd.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsvncvrq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilklloz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmabswhw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrrvnzry.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtvrsua.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/grmtqgtyv.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gxpsfkhon.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gppycbajt.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gvdwybmjb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrpsihq.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gftfuspsp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzeqjjqw.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggutthbfy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfbfsawl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/geofjhgrv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvnwonen.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glhkyqirr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsperhsij.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grajlidwc.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gocrazsvb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gvckesvll.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grlxoglme.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjamrnci.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcvtqpd.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/guiznulox.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrltfsac.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsjktwxk.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjlntte.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnroedbll.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxtkoggii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbzxnvrvr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ggecoznxd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifjpnahk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gghuupine.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghitkimxz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gohdiavjb.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbefykh.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghsuvylat.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdloyjhqk.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqbhxxt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhvposzf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjggtigcn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqenfoza.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyparnilv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gahoeotab.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guutnlukp.sHtML


<!-- 参考信息 -->