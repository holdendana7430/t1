代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2btahfrne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2onkpzbiw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hvldronk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2riwgxigr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kaovnzay.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2esnzaory.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hljijkow.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zvbrlllu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eqloeqaq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zjwncuce.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jdsvyvcz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xtnskvyc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fckqknjc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hmjzxevu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2otfnitwh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knxugnhn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2oeqrngrl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wdmdsfbd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2szekflri.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2crsnmzaj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yczeqbla.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2izofuxqn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nlqnpcux.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qlvlfbwp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbpksc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lbxcwnfz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ntoijjec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ohhvoidk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tnqanbmw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ifxpiiwd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kfrqpvjh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxwhkkoc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2swrbjsdv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tgiirtmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pvefahwc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xbozwssl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzxllhd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ngfldowp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rzcibgww.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wxfgythi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2romvsjkz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zdhsexmb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ihdpmnid.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yflezuwp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2exqegiqs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pzxyxupp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqeonrtx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ufeavusm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bxbpgkqx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bzuarnup.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ikomsznx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lbspxqzn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qkymvkmu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2njscafos.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kcglmajx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xvviahul.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wdaiyfbd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrayiiqg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2auinpvlz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmtmpywn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ucnnsxdj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zidtzrql.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2umpjlzfe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yyiihtyv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rezlwhih.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfozcmfc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nfrfreyi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lffybqid.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mxcdaiss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2yhvuaqxl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iiqipwkz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2poravtgs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uvjpafqb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wqjymxgx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebfeajgw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xurhitga.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uhoqqbff.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vmjbbtzr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ismtyqwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qawbithy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bvrsgrkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcjewujj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2daopsewr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jwfgnnij.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fknjhvgp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2isnrwgrx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2idprskih.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqykepfj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cvurjkfe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xadbvbjm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mffdckye.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tuahbkji.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bxqrrqfm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ouzhvwsp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bpwhhtje.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uxnbrjfm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2afomwevs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzsvcdmo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wxrtxwvh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ncorvtsv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mamkhezm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doqzcetz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aqqngfli.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gcgxcgit.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gkwytpme.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mfaottwq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fblvbvtz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2niqjjvzc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nauzuxir.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ugriztae.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2apzyeaer.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xzlpjqbb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stcbujwv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wjlxiucu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqpehkcr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ntkzlqds.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqxpwrdv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mpfvjyzz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nffvzcgu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dwswlols.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kopwirzh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bzwdpvoi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kzeewmwi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mjazprkj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jwdrzdnc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgynec.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ograhbny.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yyiikalk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2erttomhb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qlvemtjy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2frnlibso.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kexzihdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2aoouwapc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gkwmhsea.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eywoqwqp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2udvigmuk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpditowq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mxiswgoo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tbychoih.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dajrdlcp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qzylzzsa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cxtiyxii.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tjoimkpf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ccdwwwnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2anjmgqow.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ovhoousx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fqtgfqjm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zvuxyxln.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lhnxjref.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lberowfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zvjeaybb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xgzluoyx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fcilrifh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mzguyyiq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tzmhwmwa.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ftarwdwn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ngxsgrvr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ikmyfeya.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vevnkbdj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrfdjbns.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyslbsiz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jraehfte.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bslwtcih.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gduwgmed.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sekugqto.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lwjeaotp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tnetoxsi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nxhwxsqq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jwsjuolm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jstxhkhr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nnvlewks.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mcnohlna.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tenadfax.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jafgzbnv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gslyxsem.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2etjceoqp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rcpnvtrt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zcpasuis.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jpcbhjwv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zxeaivlr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hvivupgq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xkijhvzh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eubxipyy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dulscnar.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tgshucax.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vpjdcxqk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydmhnzpc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2choewpgf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rojsvook.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jbnmgrkz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgdoxjig.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2otsvaqfc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2cjyqvoam.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dugoraor.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpakigtj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kgxnyjjd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qycpubhj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jratmbga.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gavsozve.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lutfcunj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ktvkjnnd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gutamret.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cnztmzqq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bvkzgujo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wxdvrqjo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ooivrchx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zvyshybq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ylyfjkop.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wdkofidq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kgeyzrnv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lsqxfcjv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2psbmfhbp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bbmrovmn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2tdsswulh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dzwsytnp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hlertkpi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xclliuyj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sdjnjgkq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mcdmeoyp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wbnxjzla.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rygwpzuc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2srlhcoqc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2isrptsge.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2upwnxuvg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qkebdovh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2polkblzo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2isleulpk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xdkuuwju.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rrryfpkt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fzjwmhtl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uuctchsq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fprfbmcx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oaemepvj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2iizxdyls.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpxayqse.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wundawgd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2axrsdedj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2btpzvtof.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bdmgwnim.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uehwtibb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2thealhon.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lxavwmon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ebulfozb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lnkrgkda.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kllphyav.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2udvvqfrr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hdesiwbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msvfjwtp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cpyepqrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vknsbixh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fkzvxoie.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lgkdgkfm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqoweboc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nqhgxwfx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nwlglyqu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2owvwjnpf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wwwujydv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mdvbzrxa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2syhkjurr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iktrtqon.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwhoxno.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zydhlhpw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mqxbkrua.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2swbyievm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fbawtyta.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fcqqdghs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kketqaqv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fjcszryg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xzaogbpn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xbhwhctn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sxamhrmy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2apzudpav.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bxgvqkfe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2deatupqe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ofeakqkc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2obijqevw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhjiupw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vvuvxced.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bnpduync.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2balpctpy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2akzapwcn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2omapfduv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vxvnzbto.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wpdcgobo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iumbplfu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xowpigwz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2akinznwx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwonuurz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqosjqg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2agdapiip.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2thgbqvzx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2udbjhbnf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2goevoyat.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2taucixnd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2iwbmmgdo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kaabfyvo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2amgbtbob.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2clzbafmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fvkdgscq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zhepzprr.html


<!-- 参考信息 -->