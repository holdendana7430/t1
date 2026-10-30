代发 wailian999

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gileenbgt.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/grbqqnrzv.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/grbwbumba.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/grlwepxaq.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gypoizqbx.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gfouxwmoj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcvipmmy.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffmwistb.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gefwmeofv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmzozoqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtpmzpdom.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkkzselex.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbljbzvdc.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzwqulps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gprswebvy.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gynjjymvo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnoypbz.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtgumzxft.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfngwdukb.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbhmpfew.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgdjxbrr.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxggvoat.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypgzxda.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkszuwunm.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsocrtve.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupezggxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfeqwfzb.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/guhmixmhv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqitsirf.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/geapvriop.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnvplfqfj.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyjvxeyd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdelyfg.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuqeyoww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gopuvuntj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlhbpofx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpusxzoau.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvztbbts.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gitqmlteo.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghljckqat.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcfzdcgi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grekiosdn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfrcfpsl.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbbzoajoi.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsdrzugha.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gxpcydvuu.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gokmxhtvq.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcabbxtaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsbituic.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskzbetas.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiimkuay.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golhwgtwv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyvlnnuuf.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfpehyliz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaewbbjsi.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gbayjxnqd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvmutbij.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpetikrn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqddvehz.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqqoueb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwpqkhf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwjqhmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/grrcgwzbz.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvrnbnvgj.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gslybguvc.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkbywjqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjmhrlxb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gaytvobws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gepgxignr.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjelwuna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphgdwfhg.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzkiasib.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/groppizst.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/grxuapscv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnbkiuth.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmknwzgin.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwinfzrmw.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxztkgvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/giyuweyin.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gznviezkn.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/giljcvnna.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtmepwkqs.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxtmtqyj.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gprjveecc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmmstvh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrkhiqsq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gllpopevc.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gybydjgbp.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grtccmuwe.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbjgdso.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeldeoxj.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmhxjvcj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gctilluiw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjshyhs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbotiktxt.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtmwphzld.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gunxejlnt.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gllfggwmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlsupgzz.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gchudofgu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gbcofahsq.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gsovqxbdi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gujrslsym.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gxnuinvkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gyozoxsby.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkdhexu.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glzyfckbv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuqksivh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqzdgjhx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjezqvzs.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcyzxvqu.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrantyhs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqgumbvs.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gyqnsznpj.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbwbspxqs.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/givkfnhmm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtqbxwkq.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbjhxozzq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/goztijkoi.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gztvpgkes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkwlbshof.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcewoidwg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlspeqwd.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxwwmrs.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxjzauql.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgskwqmf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuielcyc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gaphusfup.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnfaqenc.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/geohuufrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuhdfebt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlgmyyff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmnmunya.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgvkgljw.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gaisaqvaw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gepkhtbcx.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrhnpcgf.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gtajdsmat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrbncebr.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gujkpgajs.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gdkvmozxz.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwluciul.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/geotvzoqx.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhoyjnff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhoqacwd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhgnwkpb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbyooae.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjohzjig.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gryiktwgu.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gwsaiqxdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlujqdwx.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gahlruocx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpvrerxi.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/girfqhgct.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhuylksk.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwuxovca.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstuagrp.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqphqjwl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpixnlvt.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gyruvusqs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/giafqvwkw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmhecllio.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gtqmxrayw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbdrubqsq.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmfhfun.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gimchszgj.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gouglheey.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gtjnqjsvz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcpzzmv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpqrpwjh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgmgesz.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gntqspfqq.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gbykmsltn.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/giowuggby.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/grulfyuch.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzngvwlvz.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gimfbgiiu.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmukadpw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gohskpwnu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfkaseura.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfampkcn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuaorbes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsnudpdm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjtxbvrr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gicvwxwri.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gfyeeviyg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqvrcyj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gidrohjmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggunxyaew.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqkxpjmgh.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmlfhcgh.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfapjhgjn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdquiifh.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gafaebmzd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhhzjasi.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gutiljkbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gexfjkhbj.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkqsuupp.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkaowvewf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexovumq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdjxaij.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbctaqkc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gcuyqvwzb.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcissyovy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggbqbtxz.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjcxjhvc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbqcmls.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaojcsft.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcfpniml.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/geavuicoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ggwfqtlkh.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gtpyobgay.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gnmyuhuoo.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gyipmyfjk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaksvfam.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gamoxdpqq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gvblyikoy.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gcybcyiev.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzslanon.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhdhmtld.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlkzcvtn.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/guwrzwlop.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzsnzabx.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxoiiarf.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrdbuyid.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyjxfjbwh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnsdwdnc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusaxfni.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoufhwvv.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnulopxw.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggndtywrx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsgevqja.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gogpbzaqa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmlzaigcb.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmxflvcq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/grxunaaro.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gefcymsrl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhhslytb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlolxjtw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxfrjijm.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/guzqmqbio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmhzprrj.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/goysifvws.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvpqjfrsn.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gdljsvdnr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgypwkln.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzlqcmw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ggybnrqww.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsnnaels.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gpuiceiqp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddcszwri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gauomngju.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxppxlvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlsjauar.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdnrxlpkd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gofflrunr.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/galeyycuz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ggepzvqsh.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gscpogabq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzeqgwjv.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gclooxwgu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcjodjpmi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhecspvp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhseeoec.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqimcldt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniolplby.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeffcpzz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmwkuyi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnfvyldn.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjoivrhu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gemzqpxqb.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmxrwqu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjxlefne.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfpduihvq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlidiys.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gxnqfjepn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixcmjaca.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbnwivye.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gqctviqwg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxgbwzju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfneabnz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gptbobzzg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldwkorvq.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzlvfntp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafkqsjux.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gyigkecyq.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggnurashl.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyiqolsp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbkfpzmz.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gqqtupqgr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gwxpnqhjx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeznpldu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gisbaldrn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdhvfjqi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gzabxddtl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geuarnigd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjienrxng.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gitdvjvht.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/goadrhoca.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudxidgw.sHtML


<!-- 参考信息 -->