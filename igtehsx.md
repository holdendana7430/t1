代发 wailian999

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvethdvmq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfuctvtxc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gytkrvmpw.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gsstpvvwx.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gsrngnyun.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/geudydrcj.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/geroveedv.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gipqovqju.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gooxsnhzd.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggtisffuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpfzeyrv.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmdycekka.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfozzmfu.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmasmhkmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxflxrruv.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gosrkdzng.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzuknnpa.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcchsyzk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwogvupr.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsklbczud.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtmgywxy.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoqlwapg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gokxbfzqj.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gefoyfkou.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gggerjfyg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxovbipe.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohkpizdq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gjclvnpyr.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazewohk.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goirqbhbk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkmqrjkjf.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfgrdnbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxtxqstaj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gvacqcerx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygmaayga.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioeaqkvu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjjwljus.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvetptp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqjlpwutt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfspkqdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gchfodwzu.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/grtxdinbp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gljtfucfg.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gltyxwvki.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiqssmwc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gvpjgzeso.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxhyoqhr.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfmbpzyf.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvhocjwoi.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmamequtd.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/glfygcnni.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grvuylowo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghioqzxyb.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcvcspamp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbcwwpfk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqprbtri.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzzsmpxah.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjgkvlqnr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqqtopd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ghckjsyiu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gnonydtwj.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gwbgsghvb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gkuflwbha.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnadgckco.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gymfkxhdd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuylvihc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gzhnrrupy.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gczfeprtp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrxtfscs.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjmopete.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/geanateqk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gbcdqpcex.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeqhwrnm.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gqqwyvzun.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gblfqeoka.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvbfhev.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginmtydfk.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzlbokkhp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gxzsdfehr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmioewgd.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwmhqxsy.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gxymdrktw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvegsoeex.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gukmuddoe.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducanqnc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuafqqsm.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvillmwc.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyoperkn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvssltfni.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gwjikzfkj.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtaidcmth.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaodfoqa.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmrgbmft.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxxittmqn.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvibsnlft.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiemajyw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gxkndwgdt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gauuxanog.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsuegmmj.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxeydrwly.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgcjudze.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpfvfdxt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbetetfht.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gekubnrut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ggnfuwhvq.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqnibudo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztmwmpee.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwrqwfiq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/goztfmwnr.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfccyhbej.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlytgauq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiehfcgn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfnteepun.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqidhlpki.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnmitijaa.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoijhhuk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvprxgcr.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnzjxgg.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gamondghj.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhcxbryu.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gofdxxmzq.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/guyznxxzr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvxhwdop.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gkybjeble.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtazabv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggfadsbsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gusawthko.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjuwnbit.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfehinyr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpbzklltw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gaszexyzi.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gystqphts.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gbyxmjkdi.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvcllsgfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmprrqmv.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnynewrry.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/geelerosf.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdgmhgxj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuxcuhff.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/glbzwpnhv.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gsmncapdg.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gacmgegjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmxfduoa.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxudodbie.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gknngvcaf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gzawiejmi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvruwerxr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaaorkzh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzknmppl.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gtidqfrxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gakeqidyt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfczxslcp.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gttitcnts.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqxxnne.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfojekno.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/guvtduxnl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gexygzsyw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvbcaxpf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfiajyoy.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gojqtyxaw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyimelcg.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gxlyhonsi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gacrsfnku.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gukjzbwtb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhlsjfx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaanqrei.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgarbwgl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grhtfswqr.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzklibypp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqfeqqjk.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpesjfkcz.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzmhebbc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gppugnpje.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gezyxjpii.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfhuwlq.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gljhhooih.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/geaqttgdp.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/geojwhrpq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoguijvb.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqfixkfos.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcobjjkw.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqirtpuwe.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyycadyk.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtxopqewc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpenmnmbz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gvnfelsiv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gcvvvlhrh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsclqggz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujkgicl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftkhevte.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjahjtrg.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grkqhqkdd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gepkntqlf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcewjcnk.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gcykjdqco.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsabnsrf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grwyqpkqm.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtpkbqsf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/getvkcnqq.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/goghxaudn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gnrrgqfwl.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpmvzphyq.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gudpnrtkh.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gbhlcnqdr.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexgntco.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcnziiqql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqvitfpz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/geoafwsht.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gptqevaxo.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzuoamcg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxshvksj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gdeyuedxa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gprpceahe.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gegvshnuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvakpkul.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/glpsqeemd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/guuurqghe.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goahtbyqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnggufdlo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcgteyrq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhhmbhcj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gubazkdvd.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gilcyvyjo.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gzgzfpcrh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjtefodq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gdsyocewl.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdpovfdt.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfcnmwdc.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxynnihqn.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geonvxsel.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gdmuschco.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbwpglo.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbspuepud.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtllnjfja.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gyrdnutjo.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gshhdinjh.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnybklie.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpotnloe.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufqlyjar.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkujjlh.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtiomnfx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixmntyr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdnxlug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvllzbwu.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gdkmonkmc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcnhkvbhj.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gmakvffvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpwiloim.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/glkfrxbqs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvkatvm.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrzelrbc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gbmlcwhjg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczguygnt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gowfsiqdg.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpcwcchu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaodfboi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisbjrwqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzlslcsz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkfhijkut.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkctizc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gukwdslao.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gjxaztimi.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfyvhbfmh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbtqvff.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/glpjplokz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/guqcgerns.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/glwpkttsq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gexppwpdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfotcfkdr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwniglsvi.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkflmlwno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvweacck.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbivhhoz.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghoziwdbz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdgofcdy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdflnwufm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqprqergt.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbprikvfd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gepcpvgmc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbjxjdzc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoyqyqbu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gxcmvrkhf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuvollkj.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gcihxvasa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwkywxxxb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/grzcxowlm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcspzblil.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gdsmhoeih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwrhnbpl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvihfnl.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxehzpqfg.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuwgjeb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhxuqunf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotxkntxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdbmucup.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbnoobtiw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwebymteg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmyxfosl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gcielqzvy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkseshjc.sHtML


<!-- 参考信息 -->