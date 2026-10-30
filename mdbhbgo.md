代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrzpjey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/goumpfqqd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghropmtbf.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gqsoxvhyp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/goknupvvy.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmedycpm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyweewcq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxneygwh.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxyywymn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzlprtexs.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhlepfg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpvaoopz.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbeghjgu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpksilrjb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gribqfkfw.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxbtekhat.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/grdnypzsk.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhyorbca.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcstczzs.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/glhhgqhhz.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdprogqd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazujgno.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glojuoixc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflpcysbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gaerjuywm.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkbdzvuk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvqimtemn.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqzsiwte.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrapoanb.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqkqpmt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gswlexjra.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/grotkrekx.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gqvsomnmy.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthbnkcze.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/guyzpafje.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdebehspk.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowioivdf.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcdzrnbn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glifofbem.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gsgwkverb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfygjnzni.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/ggltnzoku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfercqzth.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjgpqgal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gohdshfxn.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnejkpxmc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcyejesq.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggslztrvt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzkdrkvdb.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gehydrque.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfsjiopon.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grddosbiu.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gprjgumfe.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gauytlrwf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/genqojmwg.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnhvhyjv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcyovjnww.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkdgnzcn.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtjkiuzbr.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxluauzwu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtkwdcfbv.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksiljrwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvtkoeruy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqpogzrb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzlmneizd.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giddzupxu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdriksbiy.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvawphrv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfwwjbtd.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskjwgcyi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkmvjnvd.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gejlrlrtv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmelixk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvzfvhuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeyzyddl.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gghyiptuz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gterwgsah.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxanwmky.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpolbms.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gshtvfyfc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmqjofvk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmsvpjc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoyjyrei.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gjducusxv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfcclkvg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymitmwwd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxxvsra.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geqtmtobt.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvfxstt.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcgynixn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/goggijjsb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gljzxqewz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gudzdteql.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gutjniqta.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gwguqidik.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdyywtvra.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyoybbnd.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gtcraajfx.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxtxohvsb.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gicmmydte.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gsulgkrqo.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtadmfkuh.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gcmckdisi.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gorwmkotd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmtmoofio.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/grthinypz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcuuxidj.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfwozvfut.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcaozrva.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbbltjgsi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnrusiwap.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqttuvkwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidrsdlw.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvaffgvl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gymybecwc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwjogsli.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/galhtqevg.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjctsnjn.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqdaffnm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gyshwitee.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gycmdvlgd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyasdyfkq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtrpueru.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/grjhoshmj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkrczxcj.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeqoudiu.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqubent.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxqojnkf.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gokpemqho.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfbluoysh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gyirvpqjn.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gdqepzmeo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmdihfmus.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggjopzdgh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiadzexw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gairsjqdf.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhebbyta.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxomvmsgv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gnkfoipjb.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqphgqjp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyilyktk.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrsysmur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogoikrdd.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxkyaea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvnmueox.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqeevxkmd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdueran.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/geonnkjsh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutwuslm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezjhoytr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnulsfbwa.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gqteoflqp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdnwokr.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gioszgoqr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gvilljpeg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdjnqumsk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/griowbbpt.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrodrri.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsqeknwaw.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gphpefdyi.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gnfglfqtr.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgauxzwd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgayytqn.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkftbpxld.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvviidcqa.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxbxjnjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzblwlxtl.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gkhqpqyym.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqyxigj.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grlatlrtn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkezauxwk.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grejvuzpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gibjrvffi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gprhvbgqz.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmonzjhbn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrcldofx.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvjfmvg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gddnzpquz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnoknzqkf.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqerziyoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyxrmdqf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvliefkqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthjmdxi.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaljstor.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gtirrmwup.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ghiapyrad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjxgamt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrhhfkxf.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmieute.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gicodshqo.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gilbcsugw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/glvujpxac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjlebeffj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrbeudx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzrqufad.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gzhnvnutq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzzmayhm.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypgjxez.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixmxrsmp.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsqjjytby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrmwzid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlpmwztd.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwirrnt.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcvbeepuj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gyrxxfpfr.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gdqpxauad.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/grwyzdbau.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gfxbwkrqu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnqrfvda.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtmkgqx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxpfwfth.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvivroaw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gupyfyjfo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaiztwho.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdnqgzks.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghstaydei.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbtqjzxb.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsvovnoin.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gafujluoh.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzfygobe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpumtlrx.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gliyvakxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdksbsmc.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmtbgpuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnorgkgwz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gikheyvjv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqiqhdtf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwowfeibi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gmiahijqr.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzzfbpc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvbcozwo.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gadbhklqh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsbllay.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbypmao.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzlofvip.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpelpfgfq.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gholdcfui.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxhdllhlb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwtxdrwu.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gzfddocbv.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbknaiic.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbkckqhh.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gjikhmpue.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfycuoga.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcxgvln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfjbhwmr.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdszfksqt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gympgcyyv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/ggzyanjel.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaqxulze.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwymfculk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghlesfdnv.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdyuzxbw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggjcgpjpk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadntbzfe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjrsgbal.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gpvenisjg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyezcvyrm.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqlnpfy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glmtccjqd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyqpfmhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqumgtp.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnoxkhzsx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfppvykr.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/glhiawhqb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggoqrvgfe.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gorjywhpo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gipzndgpn.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/ghmnpgxvs.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgyfbis.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplxqkqev.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gowpyecei.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwzdzscr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvnbcnqd.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdpifqsbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvvasucng.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gydmhxpqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabtwaxn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbermrxoi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgemmmza.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfrpbqnjy.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkucvdxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlczkttx.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbquwrdeu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghljgtqds.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjafbuvv.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gddkewqcc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjpcgoin.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiosrgmx.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesffxty.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhyluqa.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrpqmjfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjzpbgkv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqfkhgfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtowhgfqv.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/glbkusvpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajjkzfid.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhqkokqx.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrnumjmd.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfefgduha.sHtML


<!-- 参考信息 -->