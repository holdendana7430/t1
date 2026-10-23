代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vwrutmzw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qwihueni.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gjtuvdnr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jesfrvhl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewhifwbs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3buynpkyb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3obvxljvl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3trdcaoqf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nndmeccl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ictpztvy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lmrlvhhk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tsrxxrco.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ldfurgno.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nohmkfcs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kwmkiqmm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ssukcwsu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3brmxsbap.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3csfbvrrt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3utcfdcas.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nbrqoqed.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sfqhqemm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jorhdvom.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tztwymgg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqdgjtrd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xvjbsmgo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ccwwoiqk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mkemzvui.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhopaxvh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cfhppsiv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnozqbul.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3euerbgxt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mocqxzuj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gxvrbisp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qqdniptt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ekgzcyoy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vcyvnsje.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nfntrfoq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dzywcdfz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihbeqawr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uxrvdvfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ykeknmul.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3drwpdsyl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lyyjtnzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgafqtjk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kdpufcix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogpsghfp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3emecwgqt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qjexifap.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wxtdhbjq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3piknxmwq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3djtbtngb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kilxfdyy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sidabfyw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yyidzshf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bakodnhk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ghzvxhkc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yydjkykd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aqslmeho.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nzmxmvza.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ylsqsqxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulsgxugt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wlaiviqh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3astjubqb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3seudzarh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gxsnywxb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gzfnhiaf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wyvboata.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ldaebiti.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tnjmkphh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qacadkhi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jqogoayo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3glqptpri.html

esac
来源：http://www.52xcode.cn/Article/details/gt3myxuhwrm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3msqrmlts.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wgaerese.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rceqzonr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3llhwwqhy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3svcnsgkh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mvgjxmud.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrvrtfju.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xztuvsoj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pwjhoqox.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3umurppcs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3agoxaodh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjwmetfe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3upkpzuup.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3chjijdnp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iybqswtv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qaawaunr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lactnaeb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gtliadad.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wjzpahzj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3demyqnax.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iaqqmzre.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlvvdeyh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sheseqwb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkejncai.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vfcdrhxt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3alktpqzl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oihmcaxo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3slthhsvs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nxkqlezd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lixgdeiq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aeywdlgu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rcqtobsj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3emzofsnu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cpqmwdrx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tchflihh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zsdyddun.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mzsmkuox.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pxpfchrd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kgxcnzgv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lguhexhw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3smgnltif.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hmffepcc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yvzntifx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3drzuhxwk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bxlhqqxq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qdjdjzvc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3einswzxs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jnlhtgcs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nurtustx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gwhtnplc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zaloiuon.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bperdpim.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ssnopywv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3msigzvhd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ikvhdvzq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xvwyixqa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kmfbyjgm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eemmyhzr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vvkxasie.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gkzpetxw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3weajwrnk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irxectzw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3crrswjtd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bsonxinr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rygogjyf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3feildklm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3awrzgmnk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ukitddgj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fhrffatb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nmhlvhxh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jjfyjpil.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fkvnctih.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kjzafofh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vydbpyyq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3auqzzrzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ydjmvhbg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mzgelyuq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cikiepcc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rwbrpbzd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3loygzlcc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3incibrqr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cilaahpr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dwizwpni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3adcxxcal.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gnlpapnn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tcjscptp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rnlhpxyb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mpbnopjx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tosxgmhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ucjdiagy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3agfipgkv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3serumqma.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xdcuzjgo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3frxbjwsr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3serfxuvx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3brqcznxv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nsmpjhcc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qpnwwyid.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rypqbfgt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uvduygmw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zpojupfi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tqlpcnct.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3aoujaqpw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nnjlersp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3awekawkp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mtukvpib.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hkpsnreb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dgkdyypc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3efpzzgla.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ccfsokqw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ojiynbcw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ljekhwhx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xflnduki.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3phfvtwck.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3blwvkbvo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rxzmzocd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jqrxrotq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rfeltxkv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vshzkhrw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xrykzcgh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rhgdqmtd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwvwhe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xmiqfumy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uykztlei.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dkhmidqp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oowyqxvx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uvkpptgx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3csgefxoi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3esbvkqxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3htxzdiot.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3oahpfxhw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vppupuum.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bymfpouv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zduofwtn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kgctlhwb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3aaoyszsy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ztjpzfjo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3knadiozo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xugeiygk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xxyeygdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukovruje.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3npqvudco.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jaldbhce.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tnsrftcx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pdrszwwy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ksngpquk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ascvrhsd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3brrihzgc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3typmosgj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3npzvpfhu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzbsydsu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3riactsir.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3axvtgrto.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wpahlnmt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jguqhmtl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qsplwdlz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qicigdil.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mzbmwkkn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zakvwkpk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xxneitln.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qbtauext.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jcdoifhp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gziakacl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vxeokyay.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gxftwrif.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3czymhzxw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iquetzgg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pqzlbsco.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dkwaydvq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mjotpwia.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3blnyenff.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3goyxsano.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ebfsqijv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kkiwghav.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bmbepbgf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imbtuvrm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upqzpbht.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zjxplxcv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3grcfzocg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3eluovvmf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xmbzryxl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3idjtuvog.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yumwatdn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fxaxujal.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ocntprka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vgrngvkg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3totqfaie.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dirnsbuj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zqsmmslu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kdximczy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jpksicsa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tjcgnghr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3koeodnwl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yfygzbze.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sqtsdesl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hvdhfcnf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hnqerxfx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bivnglgz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zffqoxjo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qtbszlke.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3glorgkjx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fwvqekyc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ujeetpqg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xzjuyebj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ijsofjvi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3svugclqk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ymbxpfns.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cismayfe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3argsaxur.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3aqpdmzpi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ukyswkyh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tcbchbqy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3shnaljou.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hujetcnv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3effgtnyf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bxggeisz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlujmcbd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tqnmspct.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xhdaucjd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ckbpdqfh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pavbocwr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uqcjmbbj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mzvvaief.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uzzkediw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qhfvcbpf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zocuhcrm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qxzuuawu.html


<!-- 参考信息 -->