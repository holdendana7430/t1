代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfntkjlqw.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/glfbgdqth.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/ggeblbvsx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhczcgsa.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghtxfcrzg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpxtdia.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gexzvcdwc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldxoycdb.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggreizbba.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmumogbak.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuyqidxs.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxlicujo.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpdcqebg.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggeppbcmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfzxgzzr.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuvpltdq.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gorwfmpgi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gidxpqvbe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuekryil.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgzlqdjy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqspkghym.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcfjpqgv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmsdtiko.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glizcoffp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvmaguhvt.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwxoxfgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfwrtrct.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjvnyaft.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gphuxxjst.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gdushvnrp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gspbwpxhg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjhyiftf.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/grcbhuvhr.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjpfzsgt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfnvevx.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqatuplkd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosmpabfj.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gimgovvnm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gajrvygpt.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gybrdkwaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvlpeoltf.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhxvxdnu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gonvthkrg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyujlyxy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guvpudxsr.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gzqpjgypr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzvmenfx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfiskxxrt.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geypimqsr.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gzbbcecyk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvebelyk.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmpajqic.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmarfhdny.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gutdaouxn.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/giublpyty.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiueagcn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gujlwzwtk.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkstsdeef.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbyacvbvb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/guevcjnlv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqslmvsj.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnwvyccy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwahsofz.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnhtuhhd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gszxovaku.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpubighba.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrctjbb.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywgduqfl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpykcrak.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaxajmuw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gazuadtag.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsdslqekz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewpnilvb.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gphedgnxx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grdptwgei.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvauodgw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfvsqoho.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gljorkpyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsdqzaoj.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqzmvkck.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpdhlmj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnppnzdz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnflctcsw.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gymnxfsjz.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwjsbyir.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqhozkxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqzodrpr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcgjvbx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcfqjtj.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/giilaasub.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqbfpaceu.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbieetody.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlosdaf.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfcapkols.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimlpbee.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmwcczoh.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gstffwwpa.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gonfvwvrr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqudgkxus.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gsclyqyhc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gloudiyas.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gphgquxug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuuyumwf.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gekxobfhj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctbwrtg.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gxcxjvdbv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gycxfgggo.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grsrzownl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdmhvecn.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsryfib.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzdkxfbfk.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gwrnvmdur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqufzccy.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgwgqngc.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggagjzwdh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gmmbbwuic.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gagmldssq.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgguyzfw.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqghfazlc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/giodfobcq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/grrkasqtb.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnwexeuqj.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxjdxfds.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqppmtrl.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gagcltbjs.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giylfvtuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gcolixsgh.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gtjjulhnq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjuhbomt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdsukvvhv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmcsfchb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzsjblsnc.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gtcipkqis.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftmghfyk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gprvqgkvk.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgsfqcvq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidhgmhk.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbgphbx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtrkqlkz.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskskjbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbizaihjq.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcvoteqsb.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gztvzwvgq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gkvapkzqd.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdfbrwy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxphckbg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxdzjxkih.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlrvsnma.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/grdvoikun.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggthlvhma.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gncmyfrka.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvcdydkrn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikvvgkeh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimabien.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbbwibb.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghsurisni.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gnbaqoyzy.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucijwtj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlkyhvkf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbwfxcpe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhfepvbz.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gysgnimyt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcuhgigi.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ggvbswbff.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlhaxnm.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gafgrrrgt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ganlxtxop.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gxohmwksn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhuexct.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gkuxsdsmp.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyyplrqq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzbgocvgg.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/grikaghkw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixdvkkiy.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/girwfnbsl.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjkucyetp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpagljbac.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gouhfvoow.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gzopztqdx.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepusrszg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdaxqsvo.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ggckthaam.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthytdovp.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqwlwftp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpjushpd.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqzhrfmiv.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpeiaiwi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxnabkxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/grxiwtpil.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtpumyxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gozhmzibm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwiqloc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gdqxdrjdu.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwjufobq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gatrwhutb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpiibybsw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gawbhwjaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ghptzaidp.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gsurfzmco.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfrutsshf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihkvces.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmednijz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gkjcxghkd.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxolbvty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/guonutinr.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggepdvanu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gsueccoto.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/guhppzast.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gppbmiwou.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxlysagj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvmfrclc.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/grdxtbhcy.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gyobcnmot.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfynitm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqkwrrwq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjtxydg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjlrcbdp.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gorwwamro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoaeaofi.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqwybsbus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjkqfieeu.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgheevar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkuasomhh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvuwkokj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gjrxfkufc.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmruxdpjh.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gustwdduh.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gnulrhlkb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gohuzqfmr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbagmbuby.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gguffkhke.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghgpnumbq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaafznkwn.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvvuevgu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gyfhglyjh.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmvfxiwc.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxgncjir.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmscbnkbp.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gpluvspsj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzsazdor.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/grwuetymv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldigxcqr.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvixuttqh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/glqnykzlc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixyklpw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqcdodm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gcblkfzsr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjgiropt.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfafxxafk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydgvifhs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuzummji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvapabxzw.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gtcbrdulk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gncucxaed.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghgxgtqkz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gotcmrvte.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsetwpnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhpkyofq.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/grsopvbvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqdsdvhc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwatdlioe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/guosnnlmk.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsirjrmzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxerkkza.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gttrzbjjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwexhbhm.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gccwjppyf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glthfkwjm.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmafnxiz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiqrexqu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gguintyvw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzldqwkc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gticnhgwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqyagpyh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtdwjfvx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gprswqspl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtrhzhvf.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmciaoasf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gqonulyzn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwtabrka.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwfmktxki.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqovrwtq.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/glsjaosak.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtchkhozt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gouvalrhd.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxmsflg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gakidazlu.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gbuctyonf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gggrfhvxl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/grdxtesio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gopvmwgmy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfspxmom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxjqpnzt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfwvpguj.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gdsozmbry.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobfahexi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnmwfjob.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gezrwvzrl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnxwazte.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfrtfvmme.sHtML


<!-- 参考信息 -->