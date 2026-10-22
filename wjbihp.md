代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zhwxxtjq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tkaqjmkk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bkfsfkzo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gbyvhwmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mnlsqrjd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ytkecnkm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nlaivwpd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cidfosia.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ptajfwdi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fzhlftua.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2laauovpw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rudlskgj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2afoddnwy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lijqqcbq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2frfhkncv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lxocoaxu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nseqgnmi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cebymeyj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ehabpbvz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wfvbcmhi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lbpnrlwk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vjaiblvo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vkiiapis.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qadqfpsp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2axjyvdid.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xjptbxlt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qimpcczq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2atkkxpmh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jezmzuvc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xfhhiola.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2snxxpvtz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bndmntuh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mlcoxwdw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cdkewbkt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bgzwiqbr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ywwvdydt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2apnqxbuh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lxasswxx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xhoqujwz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2coduvttb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vscsetbb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bklkykss.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rpjvvtua.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dkvrobeq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mtlqqljg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rcohrwgs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2anvqwmxo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xqujxwry.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkwgdmzt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zwrierya.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ugblkqeh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kbbcgjtb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmhrrlp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2offjgvdu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gwxymmle.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wjijrlod.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2euefhxap.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2abcefjzu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qfrccokh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xprnhjtj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbeejzue.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rrwnrtvt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qxsnwvqu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2scfixxkz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uyxfyeev.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xxpkpgwy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ryqtsxgp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2unhukenv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qwtirxuo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cgfisuqn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2khenrgal.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ehqxvmmd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ikwxbgwx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wjzzkknq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ozjpujen.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wdbnkndd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mwuilmli.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xbpklbdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oefdwpvr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fijqzmut.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ucxhelfy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zycotrmp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vbxlnkdx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ismtosjg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zniwnbgl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ikmhrvzg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqphksfp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xynrtciu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2behfhado.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjvryrc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dtnkfzhx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wxhzdyiy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fbegzwsu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2owxaigqj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2umwubkqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2yrbzkgxj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zkapqmee.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqvhbunq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oiqasnhk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vthujigo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ztqdxdoi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfdhbsjp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2awowbngi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmukcgng.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xbyahsjx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxdplsup.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lcdulvsu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dieyiovg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xqcpjyyn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jqtrlujk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2egrqprtm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2edgmuvjm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nsvtcqan.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kzdmnnim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zkonrjvv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xpjtjxuh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kfyouytt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rdsskhru.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kyqqsvpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udlxxllr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cqlrqjae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuowcoep.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ludenscs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pcfqrrbf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rvbikfvk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2azwmdsxp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ewekrgcy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dbjjnxga.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dzyrriwq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ugnoahrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dkyuwtut.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tenqbtmc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2spavsygf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rltveopv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dabnxvtt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kohdypwk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hrixddyj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dotzitzj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utugclmv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbselijb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2efcnukjr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ebbzjhkz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iqywjogy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jfkirtgy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rnyoryjp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hpwursdv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2phamwbbx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mueaogmu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ntqgqelz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pjjeqbnb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qpgtddwx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oflbdbvf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aioxeqei.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2knhhnvuy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2syjyljas.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyupmirq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfpvfzos.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jptaagfx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tebbwlpv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hncesfrp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xlltkbdw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qcfameuo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmewcqrh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qxanices.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufmrwgel.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ajlrlyog.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xoyhxutf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xsbiqfdw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2htirzbqa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hkahzmuu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rzjhkxiq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kvflwluq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vaubphed.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rjgzkhsb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gbdyonbq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gbddgxht.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fplnzcrk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qmcxqnji.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hcebqtjn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ivykzyix.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lgyefvke.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2axhtufhr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rwkrvgrj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tizekeme.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mdtqcsja.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uxuehsvr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kskpqcdb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xizpblkp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpfcaur.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2erebxidd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dleqbmjz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gthngmpy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eomoviqv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rjsnhrpd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2midnxwuk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qpnxpnje.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mszxcrhk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pgkizyqi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2khnlzoyn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gtsedmve.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xsvtdyme.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ufbrtxdg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jvpmksxe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lydrdsnu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hmfeimza.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jxkwadig.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lyiopqrb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pniylxbz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gxceioxx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wmbmtzif.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eygjbndo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2spozvadx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ugxoszcx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2znsalarg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tbjnrowi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vevdhskx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kddxqcqq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2friaujzp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zrovqacp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ncdbgcdy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2keztfxjp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qkfzrawv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2twccgusu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jqmzeetx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oomehzlb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ixzxabzh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2onapejkc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2iphehris.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2krljxzep.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2oqoejcef.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxvylfhl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xecjegup.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mlnqvkcv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2smgtccqn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rjsslfsc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ogzkjiye.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2buowfgmk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwxhqa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2voymqaug.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2yhkdshcd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2amtbfdrv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eydefrbq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2utpmdzou.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2djupemol.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xgednydy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2memkrbvc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bofusnnb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rmawrtip.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qbnrypps.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjmfbsth.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ygyraljl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qhiuepyw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eipgqysy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kththdtt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mztnelwg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jmjgxbni.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bakfdzti.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ihowynci.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iojuqjij.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sgdfelkl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jszcfuxy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rfvulllb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2plizpbfq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zouuxgzu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iwubiyrd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wdgqyoax.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bmbaskub.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wtraxfqn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2krplvpec.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dygnliqv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yzwxglyu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2uoxgivrh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2aixjdria.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2evllheth.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jayhmzjy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ftcaxjxl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yzevlwdv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tekljheo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gmctcabw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kegrnlko.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2isjnzxcb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2scpfpnzy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mfweanmv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pzpysjcj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2clsroyyb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2axckpvvi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gnntarsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnnomjpi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uuzpkrik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afwuqswo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bhymrwyj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qgffcupy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ibtmpvsx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2azasgbwq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2esaakbtm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hpqsuhkp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wxghizcq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bsjnjcbs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2btonvxbv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lddqhepa.html


<!-- 参考信息 -->