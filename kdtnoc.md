代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cfyuzdig.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjxmewyg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wylfztgo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lixcfxwi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kllpmtvs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmfzukpq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bxxhqufe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojnvjwsb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3joimoafa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nexxmwdf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ejfmneny.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3akfmbogp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vsypxzzg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ansfwvol.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uqombhge.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cfjforks.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3inmlgexg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ulanxsnz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3awnhlays.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wodzhasp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cbvljksd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yelgkjol.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xzpvfrsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifmmzbgg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rmdnlxzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjgxcwmp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ysfcdsct.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wsgtleks.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oesnuipt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ncxptsoy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ngoqkojc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3entibpcy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mkqlvlet.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qcjbvhqk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3yipogkxa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jxnnpnea.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cjqqijib.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nnejespd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qqeqrgje.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rhkvkczo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3shvmapea.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vgwxaqds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jnkcwlvy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ddyyfxjq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jlmnrove.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ooahscgo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vjochfbm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kokwvghn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wsbtsowq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dpxdmwsa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mkzlebdx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3frqmucab.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qfnsocyp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzdrfz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhpwqbry.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bhktcczy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzeqxiib.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kghjyxqs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yzzrgjpc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ilcnfthy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mbtjtqls.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tylhxtlz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cuxeewev.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jhaflras.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3chlxoipu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3prrgguap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tendatwc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3clizscjz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3krlcgivg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3krqjbpsw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zzmrkgxk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xxegnzrz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rtbdezac.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fhznivqc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yyybvmhr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3thpnkrcg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3nusfngzr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqrnjncs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3onsibczb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xkksbali.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ntjhwmmw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fwjdeoaf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kmlccwbh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rweewvmt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3oqyllkoh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bappwpze.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3khnqamcb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3svwwxnjv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ilflbbxp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3verccvlc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qajwjxju.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltnashlf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wdosiyub.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ulzkqlvs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zduldgny.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3njzmqswk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mfyckwmr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3neepkwuz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ugndlbki.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ecdjugga.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aglayqul.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3neyfndjt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wqxizggs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fiiwmbid.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjeiukw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zmezgcoj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ohuilhdy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ijcqynkw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fonexjnj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bqoeyonp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mznikfzq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfplfzhy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3efldlaaw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jzqqwwbp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3imweovpk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nfxxeuct.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3smczfyll.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yhehxorr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nmywmqsu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rytqeish.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wvvpvsmm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cmkvohkb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3byjugaqd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kjihemtp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixbruuqp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xghbulju.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3luockisi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kmyikwyd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dtcyfewz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rniverwl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xwmuphda.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3otozxbwv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ggayxydt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tnpncpvy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tpshrqez.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3okazxctn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3umokqlan.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lkushket.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oicvohjl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dlzfzlmx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ofnrdrfz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3prweixhg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tctfelzf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3buqljqei.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bxzbhius.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kjpyzubq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3btosdths.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tfrjqwjv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3imrcczqn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mikewwls.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xuxrpdrc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vsgmouuk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pgzxzvec.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3efuatajy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jiqxrybr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gkglwcqv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qdvtkabl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cbzutamv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3twangqfz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3khmywpvt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bczhbwko.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uavqcxyq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3aoopqfah.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3foimwihn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cfapvmct.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vatwnvjb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhhvvmjo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bxubfhyo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uauylszr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fatevikc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3soqfpctv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tbbufreb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qhgwdjaa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ofedcoeh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ysmaqcci.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oixepqbn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nncxoots.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3uzczbdwh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vpeiyire.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wpkahlqf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xyqqmunx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmqyaawd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bvputgde.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mituasec.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kvzgtjqz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lqxmtxub.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jyoruiwe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nzfdxtks.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jcuortan.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kfolaane.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kdxmypdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulyehtla.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3krkmhecf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlzqaeoi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnpaxrwr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bpettljp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xtidltff.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tckyxzjr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkoqhmr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3frwjkoky.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zqhiitqg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vlfsnvuf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tzygionw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gnpjvifi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwnbpkr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhmtzfkt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bouitvyt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3czdkiabe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gqscvmeh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eunirspf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dzqvlgla.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zyklrucr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bqfgxhsf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kvohesle.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hamjgtyd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3slhjxlnd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qvpffncc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lnojlkbm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3snogfmyd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmlfbijh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zjqevhto.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3svnadsjm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vmfywhqr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nlwmtuwg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3obdopmsz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ctugfgnq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ydwfdvoo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3joisbfcz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzaqhnrs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3agtcnxos.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3namgsnyh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wtjbsrac.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3eixthmmk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kxrczbjo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3krutvxoz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3husavpye.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hixkybkh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3maozqpvy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3khzlhlcg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3klijeora.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gbelwgbm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wwapmtpd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3apacctwn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rxhtwmnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vepjwsra.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zjctmxlm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uraundjm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hfbosgrd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3crzpujxf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vtnzxtrt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3manzohxu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hsgyhwgu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eexorjtn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3eekgcgfp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kmscbjmp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hsfewmoe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qgpxirbx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rlrvpdbi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sxnfvrwk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tclavtmr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gphkhabv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swplskoq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xplpyncz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hjwqalfg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aezmtrds.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvjisndw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rswcwjnm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rfnrbkcf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3phfxuzaz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pymfolbs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bjzaiznd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3exbjmtnt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lmnjbdjr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3juezerjx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjwytsgc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yrfywzgi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ufghuwbq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hmvknoew.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fnteqeud.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ttyiqvzc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nhugqmyo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wfurqmxw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3buwzobdx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3eqzvojkv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lisooojw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3botgymds.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oulrwogw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xlriyndg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hmspugow.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fxqsmbms.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3skcrfddi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuglwyuu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yodgiimf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ghzoaqyc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpaxqezq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uhevobyo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3roiwqvyk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxftmhqo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fsyxdqho.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3psqpvozt.html


<!-- 参考信息 -->