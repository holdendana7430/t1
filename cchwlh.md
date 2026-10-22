代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2twraweyb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kyrbcaye.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cursjspb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2riwmmeyx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2foomsnsa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kxeqagrf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrciqfag.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gaihbdnr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2crwbvtqf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2vitpqomh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zazqcjmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozffovus.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fjvjhyci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsqgbkxa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2svrbpjkt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2scnvsday.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2njepzqei.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2duuemijn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tztxhpqn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fugrfcmz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2izbtqfyo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wzgltnfe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2efktaxfs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2crdfzkrg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmukuw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tnmmnyua.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzgjhmic.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vvuoetpd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hgsefyey.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fueqctwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mkivsiej.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2liuxbcby.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fvfhxjmj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ijamlsll.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cjvmodpc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xnjgxqvg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xxayqfdq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lgflynfn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2einamtci.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2timwitka.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ocumhxbd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyymkibx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dyrgjmjh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mamyctji.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xcwmrirr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ygyorejo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvqaxsry.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mnydqfjw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ejgdjyuj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gmzalxub.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrxtpsbt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vyeiofao.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mnrvhoum.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gophlhlb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qfeurzqi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hwyvttwq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lfgufvjx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kznrhwfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2levirxhc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cdtpdhfz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjiehxee.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bfdkfyjp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfmcri.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqltjpgd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2afuimhmh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kfmupfjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gawwhhio.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2abcjwsbo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lxyivwfq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ekluoadd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ozcckgjd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jpcpatlh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rybdbcit.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wkfuedky.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hfnzjwqp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hvsqkyui.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ylifgwnq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yielfntn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tsrslhqq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kquccagt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgyauqs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2uvjhozco.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyejcdwr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2eqfbdjux.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ibaljltq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tugajsla.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bysrbvhi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fzmfcrru.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dtewesqq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jfmkkcbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rplmsdvs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jkwxufwa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hztuhcyb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ihpjlxci.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wghqtyof.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ugunruqv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uctunxns.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yobukeji.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pgstznes.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jjuhpcfi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mxxgoxjd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xvzovabp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nkevmtcg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cdvapray.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xyhaujkm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jdydhebb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pqmfcoyz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cboedpfu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hdigzisv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cinhkwhu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2riwioovg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lguqjadp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2idftiwud.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nkvetxld.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trhfnwjp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pqeudyad.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lpmjjjji.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hqidetge.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zjwjoyjl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oeeuygvp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pwnyohsa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jzybuatl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgdwuzvf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2okeovefy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zkrgrraz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xgdssinu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hmdtguuc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2peetakki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qqbyzlnb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ghimnwip.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kvrnycde.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rfdcagkl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vqiavsfv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rtchrlou.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kjxgdlmp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dgcyyacg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zaihpclz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hdajnona.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qlzhuoaf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2adswqgqc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ffcnmopi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wngcovns.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rpjlwdlg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xdxvgwyw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dqucumgs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yunskull.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hgezhsvn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2menfxrwq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2htxxkfxf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bupbkzia.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ynvbrevs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zhzivjlh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2htxlqskq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ecvqmqvk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uboodign.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ufwlosea.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uuzmhzha.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dikgippa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2aovcxxko.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zrinrfha.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2grgfrftt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2twjpjbzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2heitqlmp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pumfodpq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ynginibg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zjzwevdl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zpisdtts.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tjpcqafo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jtaahjmy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lhzdrltq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yjjmdpar.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ajyzsmjy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wyumhnvj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bsuyfpmb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2otqnwwoq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2htcwytfu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yfefijwn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dtxqetmq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uxgvrzec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wizrottr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2opejsgel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txloteyu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uznyesvt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wrtankte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjfzoe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hloqeaas.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rqeawhjg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eccakuqb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ktbtwwbn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2egsedhng.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bnothusj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fxwkasqn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qtqwmjoh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2omifynkr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zogbnxgo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2trevnmpx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pgkamhcc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sphlzdjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2eewmipnf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vxgddydy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xjjmqnjx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tysfufag.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pohaudlb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2frniitvj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ajpqhsfd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mvctvkri.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vknnxvad.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfjnasoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vpneouid.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gengcnvg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kzvsnysg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2avvytbwb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bcxzdcxu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tygxwhhg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tngncigh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kxoobwmz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oolanzoc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jugmxakf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ejeofrxa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ebybkhvg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lmiazbku.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihcuougo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2visghgri.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aghexfmy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2glrglwmm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cflxehev.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cgvylzmn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ifdnovey.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jjqsjadh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2aqdayncp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nebsgizt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qmixrmcc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sasguqab.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2emhpyrai.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2plcdsisj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kepeuwtn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jszuqxqc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hitsutpa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzyimyb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvdhqpil.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wubspuhu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uszxvqwf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2obqkcgww.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zkkowxhf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oxueusho.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dvwxvhxx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cypsyezi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lblidpqk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mwbuueah.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kypxgffk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbxosy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qwyzzkti.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjdvsm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2feqrvlri.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2immfzcgw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ariasvgh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cmpkhzqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eoepwjte.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jzxobiqz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yogapuvl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2khlzgtpy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dclpzoqw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2oezinidu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jkmewumm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2acwgbtjj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xoqhjsbr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pkgmmnyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2geheutvy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ksnqqlln.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pwwpatpf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kdormymk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xkjqcyvq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iqmgnvvj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yazsxkhf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ytauoede.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfiqxkom.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ynncggvw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gfuhlxko.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vheadsre.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrpnqja.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtnscwhl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ryczokmk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sawjwrvp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2imuebzwv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xsrpskek.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngbapbri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nvhdmveb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qguuygcg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wqgszfgb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfmupgbi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rqvplcll.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gqeunxho.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jkqnnmgi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jtqqtiyt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2agvfegsz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xryexpzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kamoqfcq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uvewvion.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ixkrhvzg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qsktxlji.html


<!-- 参考信息 -->