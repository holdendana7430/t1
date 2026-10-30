代发 wailian999

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrigulzi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjvoblj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gsjagdjbn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvscnco.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gwylicpup.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/giaxmyrqg.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gnilvagvo.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gweoddkru.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gaxcvnybh.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/goegtmkos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmwnlcof.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpinlgt.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrqcwltu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgjvazem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqccplwv.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdofvvyzt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gaemrxtqh.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gweqdtkrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjrgvkyzz.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/glhqajbgv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gozcbynew.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/guudcjesr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/giqcqvuai.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvhwlcpf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gpkxgzuon.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gotmxyyok.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffafvdop.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoqqrzza.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjmmnvaf.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkonpfgw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gabxbqerf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehyebjne.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grpqbcfhe.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grirxvtxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glldtfdba.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdojnmrdn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwgtrfxz.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gayagyyjx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvypxkpc.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/glzkpwthl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmzvstun.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ghcdnywpq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzssvixh.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkwtvkogw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxozxlmh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gutrxtrqx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtsufoxh.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqypubf.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gextlmsjm.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gccrmmrhq.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsnodcnk.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsdfodpj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gticwoomf.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsszltxlb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtimjrtlo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajxyylek.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gftmwmgya.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrlqgktr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqwgmuwi.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ghrjocrex.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwerzlxmw.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukdcjnvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gbsrhykun.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gljwqrnot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcmrtcec.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkmjrtmu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gufvrxdvn.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlhrjkk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gouaysnya.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmhpbuvh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grifvwasb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gwifyiszf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmyyehgox.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpaxuspd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ggqynapdy.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gifktsnih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimkrius.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggovohftc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqqgtmk.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggieyimgh.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigesoqkl.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrfbxiyr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gaowbklno.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyvgingo.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbitxhylf.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/geaxdrrhp.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzkxstcy.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gmakciasw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gzcopavyl.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxlboas.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geurgmqqs.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gonnubjbg.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfzfogzbh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsniyerwf.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqezxvn.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvwpxzvw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gcklbffzf.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gaixvrkzf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gclhyrzyn.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gauxctfld.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtvlsgxi.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkejxgfy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnpotot.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsbjhjhfv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxinqghsx.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamgbonc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjatsypr.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/guphoyzrq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkppxfhm.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/guoixmzeo.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gimlwailp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzbqankf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnvvcjv.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeegjbyc.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbtusjd.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/goyufloka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gzfghqwnu.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbqxljpzo.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gxurmjewy.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvaihmm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpymbtfs.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqnyxik.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaaxbiec.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgltgvor.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhalckpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcedvxsg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcgodheys.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gnyjfirwp.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/goerrumos.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxxkzbaps.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gchrqlajl.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqcwgfvsc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqxcgpgtz.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpcpmyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gcutxqvht.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gewoqktwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gclgbaszr.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/giydcqlxo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfgeeplc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gpxkzgokc.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gyzicisng.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwwatrs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobtoljv.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/grhidspfi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gltuzvail.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gzksuyelk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gewfofwqe.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwcnbtap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gggiwccun.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevwcvfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfazdfnad.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/griijyjor.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzewnlhag.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbulwddl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvugkasik.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmtlvucp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxskqvfzz.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfhczlib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtmvjuece.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyuydgko.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gaumzmmdn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyltkahab.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glbbewwdf.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmhhxid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqlufyad.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gklsxnwpq.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/galnswmww.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyexhwkw.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkfnyxu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvvwabtl.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulyzturt.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gokamnnyi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzewriht.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkmbjjn.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlkpjfdj.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqkztvac.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheckezde.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gvtkgxjyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwgzaalv.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gazyqvyfv.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwprpqqw.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqzwhyu.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gghjvbqqm.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/goradlacb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/goxlaohzw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gochnnfjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gfyaawhyx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzctywaxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gyefbzrav.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gllonioof.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/goomtrdzi.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyzunwvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guexbmoso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/grtqmffsc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gaknqqwac.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggqzjwpja.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsflukhmi.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgicfwus.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gdkoruzrr.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdrpizgr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gpemljjvm.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhcsfhif.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjvqfyii.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gfuguahmp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbwridbz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqeimufdm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdpclkyt.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvuxosgx.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafclnomz.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqhuaqtre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggutfvbut.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gcflcftqy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjzxbgvcn.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gyhpbdasn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqmilitds.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbrbsbjsc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gxbugcohk.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gkvslsnck.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gylnyxwxk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giaryqmrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmrgacqy.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gztzbodah.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwnzkygy.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gnuvzxxnz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcaanap.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkndyhcdy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqpwcug.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbuocdlg.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gpolarnhl.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gofarpfvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gtjipwgmw.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gmcvcommz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbqeybsps.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gchyxrkok.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqucbzxn.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glydgltwy.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gkrlnfenz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnewbndqi.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwabvicuh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gtdhbmsea.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gdagoeegm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshccfvu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/grkpcawxt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcbheshp.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gcmyrkpdr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdrejspo.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfdooegn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzwyywuc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhwapsji.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpowrowve.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbwxjqny.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzaxcjv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhkxwdus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcoykdqf.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gduwsqcuz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmowgkvge.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtvebhgld.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/galpgsbmh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywohcsmo.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjkuyhly.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/guyjaxhin.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gciseukbf.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gvtrcxouz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjcvpimp.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmarzpdzx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjitdslem.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmtagzgdg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gixbintbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvrudnizf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaxsbxea.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbqafssa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gjbitgpcq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxztwcwzz.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjaygaux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrtuahee.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtxkiljbu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gailysogm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpufqhouc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gswtkdahv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfviqgf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzsletlso.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpddffcje.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmkpoqcx.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvhyrqf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfbrbub.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkthdtswo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwimhrguo.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/grdkxevla.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzisnvzqq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkbqnspln.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glpvxjrsq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjyogckth.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gddslrbgp.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gtuavfqwg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkxgzxc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhncnizk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gfinmcayd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxuymwgwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gguyhardk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gehulgybd.sHtML


<!-- 参考信息 -->