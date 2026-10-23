代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sawtfsax.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kojcuvpd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3phvtofaa.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iqfdatph.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3trucvwnj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3roauugvv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vjdyacmj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nmfafwhw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pdvpifak.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tgtmdmov.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dlxiokwm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3usikznli.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3umuntxpa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ndcpfgks.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wbidqrud.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qqtljnli.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aavoazdc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zufkbdoe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tfdkohxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3diuiyscn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jwodfwpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pkriihez.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fliopbfn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfwbhjx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wfbohkuf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3sqrbawmn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ukymitqr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lzcyznig.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bsfxttkh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gkorhzob.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3abhsqqns.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gcwwivpu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wlvekcml.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hplgqxln.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tmiqrlng.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3idviopun.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ggtozsdw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kullxlcu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wzzfsawj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jdbvcxkr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3edzjryii.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rlowrbwi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ockaqqkp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cchrczjj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cwrcbdxo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqyyve.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3riizcmwf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bmcbtkao.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hyfiirtr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uugglntu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iflnhbvc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yaddxwjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rdfjxfvi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3amferdpy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jzgmdbfc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jrttzptn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blwshbae.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jauchcpj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xnvivfgv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cdqbraty.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qyogbwnx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kgycujji.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3btvavivx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ygqmnzdp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3binvrixf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xmptiutl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tserkpmx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kmbqqhkr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tptghmru.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xttirgvb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yxixljis.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vhtbslje.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jnqgyzco.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hewkdfsm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gxagbjph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gkkifubh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jfopqczg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zccjoccq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hipdqdkc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fmeovmwa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qmmlbodv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3abjvwlwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gbsmudqo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jzyepami.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yjjoenne.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ogdkmghe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3yvakzyox.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ouhuovcv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iracfhyc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fanrchci.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hmksmcwq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3eapibedh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wgytnkwg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lzcmzzcl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ckwgolou.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wjmnizzy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdklptpm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ivtgkuwl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rkchoijz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iwyljzze.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bejsussj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mrrjmdar.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vvkjaasv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bgqgxrsh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kejyaqek.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lcrmdkbz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hybtbxlr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jlubzwvn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3evaffhqt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jcmjsknt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3paoqhesk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vjwoyypm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xnoranuu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3crpqzjnk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gsibyrqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lzcyltod.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dbhqqizt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stirsfzw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qxsdlnwm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3caeljjvt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uoyxzlbk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngrdxlwm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndlstwja.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tgsdzbca.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3utmmwhan.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nrhcqnav.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3aonvobwe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3habrpjho.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rfhsmfro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uefvqnyr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vehxdadw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3llctvbcm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hcejiara.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hctwcwqv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwcblpml.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ngjnmbdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lxvivhzm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gjrvbscy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vxxmwzrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swacrohx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tzhqlowp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfahfipj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xkpdtaqj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qsplcmgk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cqbjxupl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bbinuvzl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nspjeydy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3viooxdrc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dkrhcpqy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tsjusnva.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gqgoxwwy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zddyiqmy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3itfdxmdy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hcjewccf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xtveeowz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3txmnjdpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dlafufig.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3reoljzrw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zksavngt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cbijakfa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sroannhg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pulvubpr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uscogwtj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kcfhojmi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nylrmcxr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hbekncnz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yqhyztuj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tpteubla.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gpmcfboq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqndrrqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uctrynsq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3olomfjck.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wyynwxlc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ucalldwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nriizdej.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sawciawk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pzyuelij.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bwdtfgxw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ubvupvuo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zbohrdwo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qlbfiyxl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pwfegsre.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ydppfvko.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vxlbdzbm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vwzwprab.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vzhxtgur.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3klumxvoa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rohhatpj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yuakrcai.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vfhhwhfb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gjqdgevz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ehvyyuww.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3iuqbjrqi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgfmpbev.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xtcpsvaa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3esbuxvmt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffjbizfg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ahpurqse.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mhikhrqp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jvcxzbge.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3utojrdkq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3aioodcrh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3evlcaqgj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3txodbxep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3woinomsk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3exyrpepy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tizawkop.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3shvgmkfh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hqvquwii.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bsjvkcez.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzextzb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3epvvopmt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bjkeomoy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gvtfsqkf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nnjhdtzb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tdoecvob.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3phsaqqpq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ahragvhq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xwvpurxt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ojmxktkw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eviqepum.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3osyhrdzi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xwrivbik.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fibqqhdh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zlztotry.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tfppbdfa.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jnjzfcpj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kstcgidj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ttxwklzw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bhstlzit.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xqxnrxpn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoohjmfb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gmebxwpx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3udyzwkqi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qtbvejul.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yiybsrnd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uodrkjxa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xocjkeix.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nhcnnyak.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vbzqfxsw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsjoda.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nirejcau.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hkfyafgf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3akcwipyk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hxnnjvsl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ryaadpsc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rxljmezg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rurwhhyh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dlhwvmex.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ldswtror.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3miyfuabt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ayunywqi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dhxjtgcd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfimroeb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jdnoywvh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tmyjxtsd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ufdsqemv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oymkfcpi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cslxvvxl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bhbquhrg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mkudoeac.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lqwixwzk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nhgvawid.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uplernjs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pkjpqtil.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nucaxndd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jpfjvtfi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3iephqxvm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wkshjqqv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yjzynaou.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ddphtmbm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3onphnttr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nhegchdw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rvhqoliw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gezxxnsv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xvpzyyjg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gozrwihe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bpltkupb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fvgmtcge.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3clnvgezr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3latsdtuk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ckadkvba.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wbfzvmnh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xufeigsm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qvmhpume.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3emhfdeci.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gtepqvnz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gpogdvlt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yyashmoa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tvoafhhj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tylflgnd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3byfwfzye.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uknidfgy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3uvabqojj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xpppontt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnzlpvfn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3iisdnwff.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3swjoukhj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myvdbqso.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3udoxqijt.html


<!-- 参考信息 -->