代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wiajnpaz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sctgqkud.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hkzpoabg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3peptjzcf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3waunfhay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bpcmjqbd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nslfyykt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmaixcgs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yjczodox.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfwukktr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cgwijrxs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3svyhmzik.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ctgfufph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uvqwersh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zjdsjftw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vpmxocgu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3htlwoofs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ttpopkkj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3watspibo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wludzwpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mkgamzuw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gqgmnswf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zkblahsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3captakjw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3skvefgcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kagbwqzg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3loudrrff.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ypucukqb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lhytodyz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ktheczju.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jzrwhimx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhtjwmza.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dhvwckjf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zigogpbn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tfmoslpk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3skgkpsix.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zrijiotb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jojnhbuv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ikyigrdp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljzqwkur.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nleseuoq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3italswal.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3luelufvm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xyiqxpjs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uucwlynu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pronivdc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mahvxefe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rgeexpqh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3sfecvxnx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wrsvxfnf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zwasgpnw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hvrndvmt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qxjcabpm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jknyxeyt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kndbiwrl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wurxlpts.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yoonvjhi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3muouplit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hjdqbhqq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrzrcata.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhckbqpg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qyqntnrh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qfgvuicz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vchgrvll.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aikgihjt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3baeoxdqu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3exyvqhnq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xdzgubsm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gfrvkfba.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ratibxmt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfjfknob.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xqijrrkw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zjblepap.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3shrmrakl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gkdaafca.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3annqdujk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iesstedh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xnxodnaa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qbqrfzuo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3inpnilat.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghqedwrn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3syzvkhrn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mdqrzbdm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yirmxcxw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dvksvtif.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bssfdzjm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3plhdqxjj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tvrapsmk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3klnhepcg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yhhaysna.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wbqjugwo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tstslbmu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kdkuuxxb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gdbyufbi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yzijpxzt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3corsnnve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3sjhluduo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ecswikyn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gbaiisre.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hgivxqav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ypqxvsoy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nzuvflkf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pbxinvdq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibdseont.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3naxcsaxm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vmnkuwlh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lhfvwnwc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ymqcomdm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3utfekbhr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dknuizlc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3npsqjdte.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cjzaspuo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wkjfofme.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mzquavpy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hxquyrvc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3sfpjfvwn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xxhwmfhw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vkvbuuqs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rlguiqjb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mhkzkfkn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lpgqbfjv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3voetxgpu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mjxmjyhc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fawybhoq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdrhmzha.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hiasnbzv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngzcengt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rxcqrpbw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vikzofqm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gclbncha.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3poozybny.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jmfmmhjl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3oitokkmf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ttkhugeu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hotyxctq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rrkwvpog.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3irpnpuqt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kzobriir.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jolnkogo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dbdduavh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gopekysw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hbpzpeeu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3peemiokb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gfikgdzd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ojajsttw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kxkubbks.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3deqetrlk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uqwntxbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yrnjzprh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jppbmcsu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kroayehv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pvmjdvum.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3snddoohi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bwowzjwn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nkfjveyj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tlbixukf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vvhkadfw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uemrnelp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3advblpec.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dflrzaoj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nsuslpoj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kafdxagx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3npvmdrbf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qikqnknk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gcmhdcmz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3btkfulvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3homvktyw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nayvbjoi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ttircotg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3amqbobvr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ekewohmf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rsgqkosi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ephkrkoc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qawsvgok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbsrzngk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3snzrdqqt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mdxlyvil.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iuvvefae.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fzdlmexe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ptyyolxq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sifsrlys.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3iibvvtgo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3phkixwoq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3phcblcoj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ltmilrfo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3avsngzki.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vgxdufji.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3frredtnv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kcpewsmp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bbsbrdbo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dvcucybd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kydcalmh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lhsvyqmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyvuatky.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usmsqcpp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jexajauy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3adpxqvex.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yhgsknui.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3guywvgav.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vxpzcnun.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ocblxsfg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ikxjsirv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aqjoknhz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3atlfqikn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwlxchru.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ngjqepwr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3iikabize.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3saxqbcag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iqsvpfou.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zujsmmmy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wbkwqxtg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kelrollj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lwmkrovc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3slxilywu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hixcnoxr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iefxwkux.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jdncyxrl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ywqirxbu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ylbxohup.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3handgvai.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wwuvbnhg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rgmewnhe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xqphanlo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sshqucws.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jfrejybv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cicxrnpv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lkxqrtor.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kkvlqbfe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rdxpzdjv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udlpplel.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tlezacyh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qdtawagw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xxtqnmwx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jdqipzgw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fowqhypx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bhezmsko.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jyedapiu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jxvscvls.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gkvtkmbg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wwfhjwcg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fhhikosu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mnanwrne.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fayvykdx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jyxbzkla.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ferdibgn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rjkvasaz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pgzhrsuc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ioijrywi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3egqkpyhi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ydqfbkdu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qccieqde.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wjbvvcid.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3djkwuqld.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pzxnoein.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3honwwksu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kqgxuktd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nejavmtg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jyposcpz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3habdutax.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qytovvyw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ygtccrrg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zjsfeybz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjhxaiac.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tkgssxsl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kuhmpzef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qxlrvfga.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qvapproi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rpuyhcjb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ugakmqum.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bihxkccr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hexduzbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zqczjjlm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qdezqsvk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3arzmfsgl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rpyrbfxy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qeoirtqt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3edwhhagk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3aplfixly.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qeimvion.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uibejgct.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrbcbvbh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3olbnfxuh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ttisyrcb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3goypduho.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qbrubcip.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hiokzwes.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fcwhajdx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcxxprao.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sxafrnhn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3grxzaeun.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ngujvayk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xduuwyve.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mazxchmr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hzyslqpl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jplqvzhz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tjwyjaif.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eripdfpb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3flhtoarx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yesesgki.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ffypstkr.html


<!-- 参考信息 -->