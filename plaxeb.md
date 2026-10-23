代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mfomitie.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jvzhbphj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jfhfxsns.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tucdjclp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jqodrqes.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kfybzsbm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vxddtgou.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fgnzppsx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygpklmkm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jxncfhee.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zrbqqfnx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hjotrgas.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qiimyjkm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nyvpeula.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cpjmrzap.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3aiyyuqec.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bqyaazpe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rpoqzmpv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kdzwosxf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uztqaotp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hbvhzxxd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gufaemyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xakjqxts.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wsvgdfpe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3paishfyr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qtpmtynt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3arnqgbjp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xejuglhc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bsbjqrzd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fsjaaixc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnruoarf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3coeiceoc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bbdoqrrz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kuvmqbpw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mkjlwzpk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zolgmkxm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qszfukvx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ronhuyvr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qyujucjr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yyqkjtxt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pkvzllpj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omkjyrlw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qzanxiyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3melesged.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wgwfvpog.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plpdfdzn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sovclgag.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocqgzthc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ferdzthd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udbwaxce.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3aptvbkqn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdrtijj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ezduyvpn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zbdyowam.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ajysdvpi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bpjrzyrw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lkqxknrw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ehfippmf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knapoquk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kxybcick.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hpuioask.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hamvfklv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jdpqlwju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nawqkiox.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cndqwdsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snzhisof.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pkzzzogu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3osymgxkl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3llkjokkb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qizyrchp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cvapguto.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ittsrwkt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yvtwpils.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ezppehwd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kxhljkxw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dlllvqxx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddkebtmh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3osysfazf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxvfhmp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixcgheht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jztmfclh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jzpwaaer.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wzshrhto.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3alzcdxxb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hfxlhfpm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oaklomol.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3edcqhqmu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3udtihugt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uzfyubcl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wygzyrlm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ajblfkzh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nbsssbrg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tghwfczq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tnrixykw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ubghveld.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibzhmsyr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pgsvinxg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wvtyzagh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uytcvwig.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kioiopyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cghtanir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gwnskymc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zuvfsdia.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3neixpwev.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvooxaej.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmjwrksx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3faoyjnzh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ivbpssca.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnqaqkxb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wnddrswj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3czyqzfzh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gywsyylc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbiwwkkm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fdzsyreq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qoxwcukq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mmiwdlrx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3poghihcx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lefcrgye.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jkqlrgec.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3upeepqik.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmlzat.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yofthlsc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lmocmtfy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cqchmlxg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3edbcsnkf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ydqlgoln.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nxgvhjaz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tazqbygh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3woxztzrc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wvamheea.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mhoujfpi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3alxetnyv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klnvffbz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uvpsblma.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbhluxym.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uhssxjkb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mqjvwoqj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3enqtytxl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sxpsmvwf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3abgypysc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3npyraoka.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ffamivxv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jdksankw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjnwautu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3klzixgow.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jjnucwma.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dzdzjxvp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lthluttb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cbxsopvk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tqdbyprv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vsshsans.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3noegsplj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rpkbstyp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rznxtbzo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkivfunw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaqgtcct.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vejowxqp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zetwmwfo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gzhsuiqo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rnwspxoy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3owoawigm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mhkgstun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qjltsidh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3grfzaocn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vkcuwirv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eunwzzie.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mktbbjmd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qseovksu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hjafvefr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pygdkyom.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehrvundn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3buzvcplq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3foogvzoz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gpfqvibm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3peqtlpkk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pszfxmdl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rrgktdpc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxlmxgzf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyvifbxq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wdyhpgrn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sdlrlywi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jrlbfnnm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zmlmgerl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rzdgafms.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gjqzdeav.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3swiereqa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ueyogscu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kzpcjguj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mvzdobfr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pgrvqpmg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qjqfhjss.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zunvuihb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iblpdtvr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3obgboleo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ijilkfqi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hnspqxmt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bdyprvvk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sluzqtxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pepanmgi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vgopsvsg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3afliavti.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wgwjyuvp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mdelrbgc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lregoyql.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ywojuprd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pkktctps.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vysopwfe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ngfiqcou.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3egjtibel.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zxbwftxv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nhbimxdn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3romfdarl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lkakztse.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uzvzuwrl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cjwmmjwk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gfvnggxe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ppgumkjg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nspzasvn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukeyrrnq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3medemqqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ypfppksw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3idrdrtdm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3csarhrur.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fydbtake.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ywzayugc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fchpufkq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dvqkpfnc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gwiqjlvz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcuyrmbq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bxybjgmy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nsoviaul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewlshagp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wgmvrzmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyitpefs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ndpnvudh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3heidtjqw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxwirvte.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ngbnyqij.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtldonr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eomkizfk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xrjjtnft.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wmagoshz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3otuaiztg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhjfrnwb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3enqgizqq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ggtnvjei.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zdamxvbc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ekkyotfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3veeccobp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3btbijnsv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xbjtzptc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dndjrpbh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ejrmelzt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oxcrhibu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvefyeq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uwvlntnq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tjmmkwnp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bskhrwsq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ofvngqdr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3uueokden.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pnssrhuo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rsudhppu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3djpsydft.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xpkxzegn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tvslbudi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdlravbd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mdqtkidu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gflttsdj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rdfagvur.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dddsxgep.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ufiafaqf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjgudnfc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3osxhuoke.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jwykcqis.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbgbfywr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hsigpnyz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ieecdjnu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ccvzucad.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qfzfxtqn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ksjbwifq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ialravzo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jwladgxx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xzgdxdqu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nuvwhjiw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mvqdqcyj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hzujuemg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xivxlggy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bqvkgwba.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wljgpkzr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yesvnjio.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lzrkwxnv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vqgtqpfc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cvdtuyko.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3njywiufq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rupyxktt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nrmtfczx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bmhekmpq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hkdbvkau.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3atxkitrg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hedbcpjd.html


<!-- 参考信息 -->