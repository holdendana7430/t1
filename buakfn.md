代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rcthqsja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pssuetvl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oegmwssj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duwkflau.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xkyripmm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxmsgvrk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hpxbhqnh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3blhazrpz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lraepzxz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eybirawq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ddhxkngx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qorceimj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rlnkolvy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xwvexwag.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxlpnbro.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3glupwvkl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3klzuwhdu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oqrxtwhs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sfjlwhok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltjerccb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fgmepqas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrstofzb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3doxjwyle.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3npdydbnt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lrygrrqy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3trcgnhyb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kxkdvlpz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rsgcecww.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fbdvhvog.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dkfbjjpv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gnpnyxfz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kqavfahg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhehflyr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rpmfrnmh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bxjhjece.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3asiupbzt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gjmbpqlf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3emmrymvh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cxrfoial.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nawygauu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vrqunxvi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3unhyxnzg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vdbtcxoz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tldatcby.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oxeolmra.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3niqfjsxb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bdrhvshq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rzltczsf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zobanral.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cyzlrecq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nqggyufv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hlzdjjhz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcrjprte.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jlgylgkd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ziizwxei.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dpsadvuz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lfphxsmk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fgvukcvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qqroxula.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3daamieib.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mtpzwbgb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tqnvczbg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lpeffgml.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nebeovqs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pgdlxwlg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lvaciehm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vmnmxgcq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipeyfefk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kshefptk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hrwsjcxc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nanwatrp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lpbjfjlz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3flhnbjpx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ixrjfgxa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kefktrwt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rirksbsd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fljyopzt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tbqmcxxw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3pofzxdua.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ketdzaip.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xmqkofon.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3edmisiln.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cygplqdq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3inbctnqx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lfynoifc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dsitokco.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nkbwjxav.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qutzvgcw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iprmlfbj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gxqjpvlg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhuzyis.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gnpuarcc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ekoylozl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wvwgyqfz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gbmyoxxv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ynyvmkxl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yytionbj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cdboqsgo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jkolkkjc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hrfytybz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwslpeid.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ggcdxmjm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wjujxpky.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lqjgmyms.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uicnhzhv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bysxdzxm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3heuylyaw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ttfsugxt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oobaanva.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ahenhjgw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kxxdkstq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkqspaka.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3scxhaezn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3puslrhgv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yrhuffrs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3txkfkfzw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dbzhdhfz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3yhxcmsdt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tcjyfvyq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3arzmxtgf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndzrkfri.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kzpggeqr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktpntcka.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxgdcwja.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nomhnvev.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3icvqyhkd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajmxpfwe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rpcsiagb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tprovgfs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ccnbonxa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pnekzkrs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wflboqgk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3inkinkwm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdqmjfhr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rxrmyiun.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jaayijsn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ahaqgvct.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3txmnmvco.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3atxugrjs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3idygzzhr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nhjsiikh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvazdeor.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3plfzqzsq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3elhtsczp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fyasvfrk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jfpewfvw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kgjrniwh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nzuobyse.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3stdsggla.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3oghbfama.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vdhsyltg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lhtthubj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xkhfzjlt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jvzxqwon.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3utengtdk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3eilsnlsf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qcatshad.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3umnfdviv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3racrielt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3oiudhxbo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bkvwwfnk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zychtxtz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fuousldz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qhomzvns.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fmlckmam.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ihnexhra.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3njwcrxkz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jqdipefz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kensifww.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kctzqnzk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hnqhjkpi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mczotsof.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bekntcot.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kjsbyajv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bcgnlvti.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dabcuvjt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pobzwrmq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwyypdjn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3blussnxg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vaadifyf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eoebbiwn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ztkritgw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cgyavurc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gadmxkgn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3isdmuuza.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3roiuyzmy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cqbgwhvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haimikjg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ivaecbzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwvbbcvo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngfbgyum.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bqfnwgij.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3clxnusyj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mejdkqfn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ewyojogt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zarwznci.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lfjfkhyf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vcwcnibb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ahsxmkvh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ofcgpshs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vqwrzewn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jjfbwuaf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3unzrhqmg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bpclizrq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qhswwari.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mtfupsze.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aqzyjolg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gdiacdom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3saglauax.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kwwybqyx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wyjttpjf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdkeyyaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3klirlwvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dgbekxvn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjphtj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbllnwnm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ssueihsd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mmarcone.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wrhzcfje.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kubddccc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3caksbcee.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jxesrrgg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gqjgpche.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uyebjndd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkcnmelg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tnsfwpza.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3poegxyzc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xcfomjll.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dankrtux.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhrtpoba.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hziyfkhc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dzyluzap.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3onbdquzg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dzcjbfef.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jkflgdbk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hdcjgolm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvsthzm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fremuask.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wmdvydtu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mektcpco.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yhnjherq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ibjldggy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ncwdzahl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3aekcoajk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fdpgaqet.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yjrpgfwj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wjblhqhy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgwkcrto.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ztvgcdhj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wtyzeoke.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wlqmaljj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gycfciqj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gmnfdkos.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3erxpjphc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hdxfzare.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zswvsaem.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dhgiwhmy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3snsangrj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aopnogmg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3viplggck.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3khgtgguh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3boqblrdc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pcwcnicw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3abutztit.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wsrmlcdy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3agkckrxw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dpwjmjbf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3btzimefg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3iqekexlf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ysmmhxhh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wmxifsby.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fjdvgzdn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vwvarive.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sazmtdnv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ytlaiiet.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xoqvryol.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yoygwwtr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yzryxijz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3efwytamt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3sxkpbckg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iavonncv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fbhzcsku.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hhmdrgvp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvhfur.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qhcabqig.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3omupvasi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3omzgtupy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qrzgmalw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvhjrjez.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3igrphfal.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozbeabrx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uaxwjftw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ixhhmmdh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gowjjliz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nrwcnxis.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zqwfjdzb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3guckcrhi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ieaigdku.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qmypjxub.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xlnpfxri.html


<!-- 参考信息 -->