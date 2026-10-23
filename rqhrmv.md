代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cijyarqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dfpxmkjc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nkuduoiu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3frymyjad.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pbvdjbzy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojoyitmz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xtbfstsw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzkmdutg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vokgencf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwohdgoz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nynyiycv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msvjnlti.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gjxlqtnx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktyaamew.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3obpsogas.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcgvenw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3oxrntyks.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bozhrrrx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbtgpkiy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uvxioruu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uxnyjxkm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hfawaolo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acgseycr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tychorpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ueockxtp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vaagvowj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qswrsejn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpjpfelm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lvsulnmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exkiusev.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bwoecrkf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3icoitvnf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ybirvxbr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zpebutpv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qfnsdtkk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhacvqwq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3oprdczqr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mapfajgc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3uhwuehsz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3clhiiajq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kzdzemge.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dvuesbem.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjauqrf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnrbeyva.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bzhocafw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iutwpphr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fotyhhtc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfmtokne.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hlzyfmwg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vmmqpjnv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ibtmqkms.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wfasjhmp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3teoliglc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rlfxvcpz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3atgsthzn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vemtosrr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hexgukaq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kanwctni.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3meuezxmu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsnfzdwr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rzcvwbxl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vwhcpxqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gcjleiaj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3phihdudp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vxwxxdsa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxhtvb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dbdsexkz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hwqlylkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlgpsars.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xmahztnk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kaxqibss.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zinwfcfq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcsyhmcv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rpkhpobh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vzorpign.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzrfkarm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gxajqiei.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hmvfgarl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hssxkxsv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3paopgdnf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vqnzcheg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3chvqfpok.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yhnoomdv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3klehmhzc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hrkwpsdx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ivaqvosa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zoerccgj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aqlscwla.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cuqrwxby.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jopenvmk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vpvpzerh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rekasvdd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jgizvxwq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xrqjbpbw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yjfguetw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwzedisx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqunmqfd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3thtcvmgt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3igfaljbr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vrcqqgjf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3saqrvchu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3efipgivf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xsstimlo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wznaowth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bpxcikuw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3drgcgnrw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gzdvtdhh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zpqrwqkr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rcpwviab.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bgwjmdrw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lpnmkwvd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3giiaoozf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3emovnzki.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vhbvfjnl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dsauwehl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ypulbury.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ewksuxnm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wggddpfy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfpjezof.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tndqzxwi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3carbsybf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tnfhjsyc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ilbtxuwq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uoaocbtn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cqlgvwbh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3klvxalpn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3avnzupkw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mlrofkol.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nahdvsiv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pcmxlqwb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fzxjmclk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tdafmhkw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3abcjszeb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zqonaftu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yeiyyopz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xdkddzye.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ogyvncdt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vhgbvklv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glwnifwf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kcrniwdr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qagiuwjt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwndxnvw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oisygcmy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uemdebmo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3khqlwluw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vsqqfcxq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3sbatvcsn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ueygvjnj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qbzpekei.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxcaxbyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vzcthdqo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eclqfqql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bfycmlqh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3srhdpnfb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3anbyovpi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dympfhoq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kanooixu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ajpymulm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tbycujfu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uovrgqvj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qvjcjtak.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3brkftagh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3csjifeqk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hebebugq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kfsocufn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qhvvgdhh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3axzemmqp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tfurlqzv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wkrhluhe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nzpwwpvv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apcagdct.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zjtvgqjs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jutwojes.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3giqdqpqs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mrmqhrps.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kimtkrpw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ggnsyqom.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nravnuzq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dzuzxhet.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3geflzxpf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ehitrtuz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ailzjftm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uaztphec.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qqjwqaez.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3harkznyp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvxtiysc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3havkztdn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jsmilftn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3duswrohu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hxokqfhw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bolirgnh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dygegpjb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hvlhlrpx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xhzkbpgc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lselbhxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anytdobs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lwteenbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjvmcxvh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vgawzbbs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kpxxcqme.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ttkomild.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ypevkjod.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ienyulpq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hevgjedg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3poeruekg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hpiqkawt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ixceogee.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zkoccxos.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wdpkboia.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oznervoo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3oykcymwn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wqdezlvo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xiyepdaz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3llbufmme.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3onvcwgev.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cmpuqnwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3oxkknsdw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hqmjocpq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjvamer.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzdrxnww.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wxrodkbo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rponrrvd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dcjevfzs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yscctpib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lxpzwwhf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3sndzunfb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wuhiviyy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gpfpadkt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3adftedpj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kiedsrxz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3aenftmnw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3oyjugcqb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qpwievuz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3melmqgzs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cupohkbz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvvzubgj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vxfryttc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mnnqcmhm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nehkrqwk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3udsnkoqv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cukytqef.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3scoupyrm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vqfxddlf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zoxactrr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vxrmdrpo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uzjhezjs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kleljncf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ecdvuzpm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cliglqbp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ktneaxag.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xahttlfs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sbgobdkw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rheeqovr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hwlpaewf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sqmcadco.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rzownpdw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rywzeala.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qdhwuygg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dojmgssn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ebocwbec.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wlewhaai.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tzaixmar.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ikbwbakm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ulmzybpi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3sjdmwqcg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rruwotoz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zowaqdlf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qmjhovjp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aimohauv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzhrgno.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bzfuvngg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydqssrvd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lssoqhzh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cralffvr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ixxnnbni.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3urpioydq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wahheguz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3oxedaqdk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgwcdipe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3erengkro.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hyswvlay.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dlixercl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ngmsujxn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgagiwme.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsjdfpjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rznneisl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3istbdhpi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jdnnubqt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3useqpikz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jxgkoxsy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3maylicnv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwoukki.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mqbnxeei.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jsneuncc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ehoeouhz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3woygdxgu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ftioqkap.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fjmmahkz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gomlotvi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nactreil.html


<!-- 参考信息 -->