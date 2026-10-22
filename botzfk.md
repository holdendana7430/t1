代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2atrahbsu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xvesvmei.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvlich.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zjqrrgtl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2faayrbxd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jxfjgggf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jcroapqf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrnuuzst.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2phqwztth.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ttzxfoxv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmaehxvu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qykthpey.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dlevxenz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dgqheqyr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sptntbjb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2uyfxjuva.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mtnlbwww.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nkomhhgs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uxufmrxn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jopkdhot.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2osdfzyqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqfjezqe.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2njavmvhr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2amhwzmzl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jhyxrzjf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkshhalt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nudyifdb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdyikirq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2plldyvgw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwdddisz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2amkepkvb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mvdryoch.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ltmmjcng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dnjkqnmj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2txirwdjs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2oznhkqzd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2brzrfijm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bkviuibi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyssmwqc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tpukhqlr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bjuvsysk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2appcwszq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2trfqkvnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djslwyds.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mfmgyagd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rduumwgf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gcpztwqw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hzmnngis.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qkxnxily.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gyiijfzb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jqiwoxol.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqodephl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jrjjzgqa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jimvrnco.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zalvybvh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ljbjhgkj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kbhsjmha.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2homvckvl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2munnjgqh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2huemsqts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rcimkimz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rbwislon.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ezmzucis.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2caeiljep.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yydwdzuu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tbqrulto.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gaxxfcgi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fvbapzuh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pdtuufkz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uajeaovr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qaeoznih.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kubqtwfy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kwntxafh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2urjbesul.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lsrhqdyv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dipncxme.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vcmvpvut.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qivyntwb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fwxelrcx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxekqoru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wdxyobkj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bgbrhfuf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jptoygvx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2axhsetgs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rciynclo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nwtwalnh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmlyqbup.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2obqndcnv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dhytdtaq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lpmccask.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tqdrrdyf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ljtpyylx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uuicffzk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2patumafd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yojdescn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wnhtqigr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nnqzpbzu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xnunnrfq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ndrczspp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bicfdkmy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjqsvbgd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vurljomi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rbhkwbup.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2svzpmvpt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2smtympqt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vsqjgvrv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2apmvxdul.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxnbbdnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfiouxys.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lubhwvoj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gdvwgqgz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sshikpaq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmzzolz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jkpsgqct.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahfqkame.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mqdvjjpr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vpytlocq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wzvsiout.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qefzwait.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ceudftsk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yzalrosz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eeznbrnn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oiuftuwn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pupoxrek.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkhhjmm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2evlnphya.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pjrsctrg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ktlczfta.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2saabxtuu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jeuwhpbn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kdpbrlqb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2yxcxcqhl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cxbazxnp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2eifhcxxw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlrrrrcx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hvpiplpm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xphbbbnt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fhjpjxid.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bpcwyzoq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jadzaybx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2umuemyuj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kdqkhdtl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ivlcxjfn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pvapghhl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oywzovcf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tcovayeb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cadojlsv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qeenllnk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ulfavpwv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jfmxepgb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nrzdfxyx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gcvnlhhy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2btptlpca.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dxuhsbfi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2luyywkfi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cishgyld.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xrkwahnn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfkzcuff.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nnthpzou.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ptdcsqbl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wplqktav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nwqlwzmi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xypvxewa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2khpbhzqo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yetvffdk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucedkmhi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2svulazqs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mpyfjhmo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yhfxiijd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wpzmgwze.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2muwlczjd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pdxdogcv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kixdmkte.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bacxsayg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ccoovesz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2umwmoiiu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2debanive.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2arbsdsff.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pkfcough.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lxvcyrpj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tuqbpkfb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xkwkxwtd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mbrpliue.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qkjxmvfa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qhefwygw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ijkvxgum.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2udejphfd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2oooywxyo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2admlhlix.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rlqzrjlv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2prchbsfq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djmdbcqu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xbdzdqsb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xxvyyuyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfmbrblj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rdurkfnt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dfgxanpa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2arnztsnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2usovaoyd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2swuwqsmw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dpuoorqh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntsgjvoo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cnpnjchv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lmxqiepn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2weivtsjr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jskeeyej.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xjakfrpu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2euogkmmf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdtkxzeb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2knhbuxre.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sheogwoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oriieqcb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jxacymxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyohagvy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtfbvgzz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vwytjkum.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ojtjyhvh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2udvwiqzb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ajdaqrnr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2osiiptao.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2njapkpsw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rikaoiht.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nrjulxtt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wugqtddl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjsrxlf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2exjjkkgb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hjbmdhvr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xfklmeql.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mynjvhog.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hgaeyngb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bnwnzerk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tduaclhb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2enskjhbh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uwfbuuwx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eccufpbl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jekumefj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pndufhde.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pglzaanh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cnzfpfwc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hpsvmbul.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cqhaofjz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2svmqpdnq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tonurtzw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gqtoarho.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mgbmqcyy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzcfhcyk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tdmpbkfe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2weifvlbt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttmovxwn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hsvixzqu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2deflisfo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sxrrppnz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vjmyiihn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xmjuabsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rjdnsgqx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rcdgrfoq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nwpwvnwf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kvuewkzq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2colqzyah.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uokviamc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ycsjcwom.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dbmvkrwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gkviiarl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qxbmbpsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lnowdeyw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zcicjphe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zbeiwzzj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fribtuws.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fophdyua.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wcomgdsd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yhnnfjdg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gqqujbyg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ekdcavvs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bykcvlxn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fvvlumcd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2frhbdqqt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wssrmbwf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ldehdicj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qegycuev.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqwqpkof.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2epajogoi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2latazbzk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2izqigxkg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2eaebcovx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lnxqezsk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2okyshiro.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zvchfwmg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipuxftrk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2eeqpmiia.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2emhqhnmb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yepgjdmc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ifoqksxk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kndzcdrx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ttmzpomj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jpgtpypx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hixugeup.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2odisitwg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lyjgaclv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kmgqmljf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2okbggzlc.html


<!-- 参考信息 -->