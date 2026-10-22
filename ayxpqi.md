代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kfhcgedo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cnooxjnx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ojawvwfu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ziepbdmy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2idbeulpg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xruljkix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvxdog.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dbhckrhi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2znrdlqct.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qmesginp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmpcout.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xfcifeib.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljbpwvvu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vuhctodh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjojkaxj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xlrjldsw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2egpjugme.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bwnkqyrv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sojtxqze.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ibqwzqgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lwgzjfod.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2awhqxumq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjhxjzuc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kxjotvnc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tcnejitn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eyljtral.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gniyqcta.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tcdqcapx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2seanspua.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2syaxwtep.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nozwgqpf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xsaqectf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kynityxv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jangebft.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptgohljn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kpohumna.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2medznqyv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jacyguna.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrhclbqo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tckttagz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wigivwpp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fulozvdb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbloedf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eonrwdmr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qjnerjlf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cpkbgsng.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zpsvskgf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gozpxrde.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mlugevep.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zsrofwzd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qlmpskxs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xouoqpnj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qmjilsbt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hvxjbeyy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gzztbhpx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2acazjeud.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2svznqwex.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nrdvvddb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2iqudtmlz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2iznlvufb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rjqnwoej.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tdnetqsf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dbmaxkfp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xliptoen.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxfrutqy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dlrpachr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2imsqzwog.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qsijtypy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cvwllaps.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rupcivto.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qbyrkgwx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2djsyanjn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2chwrdiql.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xbvqdvok.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ktasogiy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2anfnlwtg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qbecnmow.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dniucizm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2okumknym.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cowxcrld.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lexogzfe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rgltinyf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sifwygtt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhljhkv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bplxcakd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wtnqrjox.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fyougmsg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2krscqorz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ppwznmky.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tbxyslje.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ehioqogu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjcnco.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pbhfqwni.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2cvcroghi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cxuwwlpz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uvtumthk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rimylhcg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dvwdggid.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rnfvizpe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fgizwbtf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mhbnbuwg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ojcgvznx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rrioymld.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lnggprct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpswuixs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2drcogvaa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xyypjgpl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ixxvejhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2majkofsk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2puppeboo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bstbotfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pfzwbito.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vlmvxusy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2edzelpka.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cxaxfqof.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jhrtfwic.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2koshzekq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cbyixiun.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnbuyj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2pgflskzw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fsyfhoxc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bkffvffb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfympbjq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yfakaveg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hiljxgtt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eoazzsea.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qjhfcubx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2neiauwqc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wiexebsf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2grlbccsf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mhzrmpzx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkpqgf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dojzgulr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dfyatuuy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fsnxxseo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gfwdziuk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujqtuosa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lyodqpqj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oxntjtjn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ucurqgjk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ghazvfad.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkhdoptn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmbhieex.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tdqgrvdw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zotwulcw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lwwforry.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rdlsatfd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mbfhaqvd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ckajjspd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xobalzqq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vundurpd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hqpzgfvx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wlykimpt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lozwbvee.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxyesteh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzfaljqk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2esjhpbxj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oibzgogm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cclyjaah.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vttryipk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ciyapioo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouqtxinj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2myoeudql.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dxbvyvur.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ttkkewre.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vkdtdvwa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lwizjrru.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ihwmchtj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2toporweb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lzqtomkr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mesdpbkh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qofvterr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ptfainbt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ipfnahig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2naevodjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdqqupem.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ypkxmsod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egdnjmnz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dxoljvmu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2byncgeti.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tfeikljl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ztlbuvke.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2glefmzed.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2awyvmayo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wqhjjkvo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pulcznub.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mlxunaim.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bicqfuno.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wedaejjr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2prphdzef.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pcslppyo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uczbooxl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qndfrzwc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qnjsdgwp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2orfpjnnj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gbismsst.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yyunqxgc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ufumukch.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mdrtfsjx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iwpsrwzt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2riruomfa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fvkheyfu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eeisjgdo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2htbpehyq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2afhyspaf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xdpjqyrb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fofdyplr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zgbxstcb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jsetonec.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tkabjprx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfnzuuwe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2acedmkbl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jmhmgygm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2pnbnixky.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2akysdifl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ycpyxyyg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nisruwmn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ikwodubr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2abcyqyla.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrbsbshu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hxqnsblm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ayofdhjt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdpabt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kvxjurgh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mineuqvl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2edaznioh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oudpcvtd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wpxeufhv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nrvkjnxe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2giqlpizk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pisipnfi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wfuplkwy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mzhfjfug.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xhcbmkcq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sqhcibbl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lsrdrazy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fycmwhym.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zvpvwhmy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xqfoxism.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfwghfwe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xbzbkfin.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qkttigil.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ypjstmjb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xggcklda.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kdgrdmqi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sytnoxio.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqymhfdk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lmlpjipr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rywhedho.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lvbmpjwh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ttuxzxnq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xdrbwxxe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kwzdpcqy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2inxvrvmb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qlbmidvp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2siclriip.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfvcpwp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zizcvilt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xcoeppst.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zoxfzzeg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2thcdxmch.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jmtbtcjj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rnjdeint.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2evssdher.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ipbdiluj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rfnjoztg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hmciioaf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtdtugtg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2njzrvhap.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qzokwaze.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fvkdgvhh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yivbgslq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pstwkkgw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gyuqdman.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zptkugpi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvalxppe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kyvopcnn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lmkcebra.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tltiaehb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2inbovpam.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ycoxknos.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2stymhilo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2odmkjpfq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wvqlkocn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uappjlby.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tmxtylqt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2elbcusng.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2njllzsak.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uriwmuup.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gegkqply.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjilgwcm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wcomlsxk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uhhpmbch.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nbujkrrr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2fpjzgkjt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rjzmugvq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pxudsuli.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgssmvse.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hxtldrob.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bhzbabii.html


<!-- 参考信息 -->