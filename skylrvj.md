代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gfimuvppc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijzgbzlu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvkuatnl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glnrmjntb.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjvgrtaq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtjjvgfn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubqoumls.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gzknttxva.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gyahqccul.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzhrdpw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgsazmg.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtwksjcj.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfevqxas.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxdrydljd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpxajxnj.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gojwcbllz.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwvksmn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gozserzbd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqsazysg.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gskwlcdra.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gdlphefus.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajpmwqea.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsjbpyqhn.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/guehtfemo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpadulxi.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gudwurhho.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhbibisy.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gidmttcjp.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gjnsktbow.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfhvcgay.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gonosokte.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsljxpmph.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbhhwap.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqczrtcsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqucmnfm.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/goifijfut.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/giyihptnh.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsjzpitc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsppbizet.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gezislexq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdsigrajv.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfhgakrnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gowxpwpgg.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjapufc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqbxwumn.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ghepshlue.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdmthvwt.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghazaxrvu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicxxkum.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhdhwlq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/godtzcazk.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqolzedj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmemnvkme.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnyfhuuy.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glypmcrkf.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnywzogi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfvijxav.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdjqpes.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggizymwqk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxdsdjrq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givjugvwv.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/griioioot.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmpyvqjk.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gzivrzrmv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gopvhnzku.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gykccuzdr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gorojnbje.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyfcrfpxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gafjpuxmu.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfthgxcs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmjxbmad.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelvouiet.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzsemzadf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrngxkqs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdbsucnl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvdjzfy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gefmtdnrh.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxccfojn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehasftoa.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gticiduvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfuatrwx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyhrnjzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjpsowcw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwdohqljg.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbeufctpx.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gdbeaaqqv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gvqwpypeo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsqnwxac.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grpuyjyzt.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxcrjace.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gjfcsamle.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpbjczdh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gkumjzzbv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwueqpkxt.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpqshfof.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdwmqewyu.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghpartuhp.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwcuavpmz.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnguavvmo.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwtnbbaj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/guydvzdge.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gajptbcxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtrvyoio.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/goiprztpo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gspootygp.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxomzqirv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnxzvhxw.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gazjneczi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupucozwv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gckiadkaw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glwofhefv.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gpuwsarru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulwzjsuz.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjuaipdg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvwljbus.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwyzlcub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzagiegro.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glicylbxk.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzvxnxol.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gembmakgu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzoscspa.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpvwsbm.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfycqbbt.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gefjpjvly.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gibgyycfe.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeimnxbs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gksxmroht.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glbjiqdic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/glbgczrvh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsijsniex.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/giyqpzteq.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqokdqpj.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gykknfecz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmyzjzzb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/grxcrshgn.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grnzweuem.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gdpeldhxo.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gwthxfqed.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gcfusbywr.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gcdsxaxhx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gwspexdah.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gznbgxcbv.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gzivdslmi.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqctfhf.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswsnjxpt.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gaykkinli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gocrwifcs.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtyydjrl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilriwio.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqfmggn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gucrnfiqm.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczhqvxg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggykwuaow.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkphbtzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvddiksk.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/geqlojgzf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gechwoslu.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlxqlmfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhfvfphf.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpehoqrk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gkemvwsqs.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/guittlyrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwctawhym.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeyygaie.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghftudznz.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsuvqlzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuabjbti.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdldbymv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsyyqzypu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gbxpctmrr.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gutswdlvl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gweiqblmy.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gsqsgztwc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxyxumfj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gflywxkiz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gudqvghbx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnuxymip.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgihseq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdixunjlv.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gceazvsat.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmamiwvvc.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gtxtxbgpy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrdtcrnv.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzbyeiig.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjlmleya.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gorrnjxvl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfdsiut.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gipscimet.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpdbkna.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/giwuqmtxp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glyclvgmc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaewtiirv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlvhuzjn.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gcetgfrhg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfplpvai.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gllgpsvdi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkryylpd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzuyzeku.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfgtvgsy.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbsvoeibi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoztzztl.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gufqdvwhd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gfflpbeof.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclswaiqm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwoxeqn.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfxkafnev.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gmvvhlnxe.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvvlzrpv.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbseuryw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzcoyhxe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggksnfeei.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/grzfapeug.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/golliqtuk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzsvqotn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkqfxauc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzcmkom.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdcbubtj.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gprihdugw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gweglcpib.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxyvxqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyyytrjg.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gtxajjuot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gvolhtmrx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcdjhwkq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsaxino.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuzargzy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqokmkao.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaprhfff.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmajnpui.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gitkfrzdl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjenwuuk.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgysisjj.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwidhuai.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkuzvgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmjipepd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclfftatn.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwmjbyak.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gprhhuxcc.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gnemijymb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhlezlb.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gwatllmim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhzvznlg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwntuizlu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjdksftn.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gfvkitoxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/goafcjsol.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlnkhuk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaankukkq.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvcsxrzd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwkloews.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/giftossnm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gftssseza.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagvzsyvy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrpbxdrt.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/genwapjcd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gfaxdcjyv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbwbchsu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gzckwyqab.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/guruuldlz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyoddotc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgxxwssm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gubvkgker.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeijjvtm.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/ghjyztdxd.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gtmiessnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gzojqtyld.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/guvyqqoky.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhblmugg.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gvaasicrb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/godfmzukp.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkeztmuj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqruwoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gooqfahcc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultvibsr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaaoyjsm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxrjopt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhxdkfmv.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcefuwazm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemdeoow.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxvlklgpr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglqiyfy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvewzyv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjynsmks.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gldzqualt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqwyurol.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpnmyneh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzspesys.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gucbhhtaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gongwxmyr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/galmjxkdx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzykepequ.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gydamamwb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gawzgquvb.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gonlqamhh.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gyopwodpj.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gxuhoteuw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhrfrcdt.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxmcywudk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrxqiymj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghborzgxw.sHtML


<!-- 参考信息 -->