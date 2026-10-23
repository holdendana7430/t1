代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfdeukbr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zeklvndu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wlseglnl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fgqirnuu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3epbeqfcu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kouutznl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ivkqnycv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mzmczjhr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yahhwvci.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lekuvbwv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kmxmongm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jkyiqznv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xozbepdp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bnqxeryt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmetrpik.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tserzroy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sqoturhv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oygbhqjs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nehxhjpw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3juvzerhn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aetptoqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mcgccyrv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3swocuugo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wcxoplmn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cngbdvbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxpejkvm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dehxraoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3brqszwaq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gnioobij.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wydcspzj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uhlhvwlm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvqcljci.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jtfyfvfd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzunxlyd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bqdzdpgn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kxqayztt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3avhmavee.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eifimptv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mpqjadgw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3btsrsekd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3psvwtvgv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ttufsdhz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmsutjkw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kzjpcaav.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vpywcpjw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zqttbexm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xcptpwso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfkpsdon.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dfnbwort.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phadzqon.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jpcliqnm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xmedpcnz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3isoiwyha.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bypeelnh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wewoersy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3toyhvnfq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wqjuowbi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qfcddrqy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bqompoyl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ifwmwpyl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kgzioild.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3asvkidhf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jqfsnbte.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3embahekr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jiyndbra.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fnhnxwcw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oygkyotq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3isbdfscs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gsxyaejx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oatutyqb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zjxcqibw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ntxojbli.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tadsoewu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfkmiqvk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3idvdreqf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vxpwyrii.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qvhuwomj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tutyqhdu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gpomltzq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iwbvqbxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ulvavyal.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3chouvctm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oexsdrdt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyeknaep.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zxulhmjt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jiaqsyfv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3teziihdb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ntoaerrc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tavqhvhc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vwardvaa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wonorjxy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fznzzmjr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ityapbxr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dmtfmvlc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ruobvgpk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqjqzofx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3foaageqa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3acpmwljd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbyrnnas.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3novgwasb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3prdxihpg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nghuiaxu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xtefgwpz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lqqqvnpb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fusaqxyz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bygzcvsh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ilbdlfkt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tshvoamq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cydftgaa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xiefglln.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zxqcgyte.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3otegfrld.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3twuarfkr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rpvgfndh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wswcgxli.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cuxfrjio.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3aglpdhvi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ispclisj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gahtoxee.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iebvocvj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nvqwhltn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nazxzafz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mtydncqj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ihbtydub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xjfrjwbr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qazsfsho.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ggthprid.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yjvjumfe.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dymbtpsr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3iffmxnbl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ymwgkdbr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nucedxfj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wnictfnb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3noexiluv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3grzzpkfa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rbkwkvyj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vkgzdnka.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wapcdzmo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cciltpwl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3esnmsysr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lrrwnjri.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kalawodk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3srvnljtq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqryjc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vlrmwjiq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iibvghcz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3baabvhln.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jasuqfbc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jpzoanzg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dfynpxdb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vvaiupfx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rlgczxqt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jqfwggaa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bpotkqxb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckhcrypk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xaifgrtx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3aexgocsz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hqpjdkft.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubpbzclt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qplsjjlc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3eiruksdx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kkwxuyvm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3anthjgfq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dlgzizyv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wsqqyppq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3riofrbpb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qaiztiey.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bosozepv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mzhqazoe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgahnxcm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gkoaiyie.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3byueoxgl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zbznrqad.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rlnptubg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3huwdnzdx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kilffmex.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3leevaezw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygwikdkp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bkvsdiob.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gjuvdlec.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3atqxfmdw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hccgqwsq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfcjucw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qpstvufi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yoxlwruw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ffaittgi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xkfcixkb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wqtlxyfe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3atryimch.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zfbvayfn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rmqjldav.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wrvjftzy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3clmxypuk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tmodmzcr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hfykiqwp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iiuwwepn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fkuaynqk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mbqpbjib.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ccfswhgf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zgtrfdrj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tpinadrx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ocrcexhm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xblmaehk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fdtrhwzj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qwyceqxa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3phedqwjq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bkvvcnpj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zhfvcqtg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3edmaoahz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xapecztl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhjixgpt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jawkioxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iaconrzv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pkmrteog.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dzrrwvii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjhtbhil.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pmfafzlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpwvhxxb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3apyagvue.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xguylinj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lyzojkfj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3adgbisql.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hpkdwoxz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fgximcws.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rpabrclx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjxdec.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cfulujaf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3asswmprn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hpokxudf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qihkzbng.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3oboebykj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lronzalj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3miqwaqon.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tmylpuuh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ujgekwzd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3drmyvmpv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqtzas.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wyhhtaoj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pzzhvzhr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3viemjtvy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mvuofntc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3msvbpuau.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xaqasboh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bvwqpbbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rrirbneo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nthytgzc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lvkquugx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3aptzfimi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tzjjjgwl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhvlmjyc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wjengumj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qyoeagcm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3okktkhsr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gbcnpjpd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3onsdzkkn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfecshva.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3junbmbet.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3axotnhlt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aymfsbsh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oglrymym.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iyjrerna.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mnsiuckx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zsfxobqk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eajufewf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hyhndqtk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rtasjmgd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vkdrhuyz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xvbfcovy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3puglhouf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dvisdnkb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wqqpdjkd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3egyxsaqt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mxkanqbs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ujlqpwlj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vlxcvocm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvrlnfxt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hsgbofpl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3drjscghr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rfuqpdha.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lxvfcbdw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3btxjvvzc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hvlkyehd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xbeumtas.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3saxornpc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cmprldnj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xymwizfe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibxoayuq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fueqhzud.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3btjhmnho.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tbetczsq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qmjvehma.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqonhkny.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xsewpshk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vrjveghu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3aaocychm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nizljfuo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3obkinedp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vbmfhirq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3irstlagf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3owjtfvlz.html


<!-- 参考信息 -->