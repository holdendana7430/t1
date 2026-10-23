代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3truuyfjt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3achcqvze.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bjxbpepn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yexqjihx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ntvsrxsd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ufiokgpw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwcktst.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3oipzuzae.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dkuscvla.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uvpxljmg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kmiwrpju.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3chxdqode.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bdxogfir.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cynlywcq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ngsluhzb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nbfdykpd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wlbjaojk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zqckuocr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ezfuaslk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gqzgdwjm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsnfgvij.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sacqbzhv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbzbvent.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3atwnfhuy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mdiyophr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3itmcfrcs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tptksdge.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bahqomhg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3stljdavi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ztislcsn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cwdwrgfi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zoostgxa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vpbrjnce.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3aqpniral.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wjsesagu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rsrctnaq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ycjmvnzm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ecuzyjly.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zujhvxrq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3akxvvqht.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3upvcmkkn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zqarmwuu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3impubhen.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3qbmlcwpk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojqxludw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3agyfjlsy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ujtogrdl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yxufigwk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pezaxwog.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uxajyxry.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3urijppst.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvnetdnb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwykkeuu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilhsxawx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xwrgncaz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3icbjgwsx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vmqkodqv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vlicafab.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eiupwwua.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mynvsnns.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3alqxiabi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dclxfexb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lykcujat.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xnbaarbr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sscgasrc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3syarbhja.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zmctiedv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zukesnpc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tgptesmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jfxrpbqc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bcncjgpq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tubgvnrc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3umlkrdtn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mdhryoga.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3aauyfyyh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ryejllyf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vgozghih.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3izdvvolt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gsuacbxl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rpnhescb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dldgarzd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kcitaarh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3usempito.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ltvyeuox.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3svruybur.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gntcgybl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pgzhgxse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mqmlkpqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vaazkuko.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dbtbfhgv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ycxqzrrc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ocearjbz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3knwsllor.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3szmaqtfs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3djolfanq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mhhuetbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gjvvatpr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3saafrmwc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wcksywom.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tlbwilin.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mhrdgeby.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tunjynjs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eucmswul.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zacxpefr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nnbmwhnk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wnynxupl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3czdyouox.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sxegwave.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oqvrsopb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3volvaudw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xhsxicha.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3auaihqyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lhmpfage.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3dlkqduzw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yuaydegz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rdlloprx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ieyrespj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kacsppjp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gngbadca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qvumeqcz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3plvgcfip.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggpmegod.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cwljljoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3alxvtfsw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wcvjiaed.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xdmgkrnh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pvsougbn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zdyxqdzl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xahvabyb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zhypkbjn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wkpoasus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3enaoaryg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pgzxuwcr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qmoppfrv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kprzfsyp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3usqgwdsx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3iymieddb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pcgzfyzz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vqkaapet.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3otbtheng.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxnnbqva.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ouvmuosd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3pbgwvbai.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3almbgtgf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3haqejvfc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3osxaosjx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xrfgvcvi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zkidkjpf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qeegfnrf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wlnzgglg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ccuvxynv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jysuuzkk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tvpdebvk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3vpiynqyg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3enknxxdv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hjyewyom.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oghpyvdr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gocexzek.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vhyvwfqo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3arekfbtf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dnsnrwoc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wybwizrx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cvpphhlk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nmpeuzsz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3itumpqnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcyeuljk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ncncohyd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfxexbjx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3grnglpba.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ahfxczec.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3igfshiyz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tmykofpg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3majqlqhp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nkpghzgb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qpisdlcd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ldowyvdh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gforhyuo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3aojkslml.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scuzmicw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kgmafnen.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qssrrsyb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xosllxvn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tntzdozp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugbeeuac.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ovjlwhbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcyysufh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kneibvvi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jlglyaug.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xwhwzccc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vpdyyolo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xaazqkvh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ejssxlpe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ndsfphoo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nsivpvvw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qdzzccof.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3upaaount.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yklfityh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3goncmbqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wftiolef.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kfvyfuch.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rjrbpjlq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ixfjngdm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dpqnlryc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pgsjjvfc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jttiusns.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bobdegfs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cmrhyyss.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3isyvxhyd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fsgayyly.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lojlhyyh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qmzbbgol.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ninxmdon.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qcjcnroh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mdceqouy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pszidwqm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cgamagjf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dzhkcdyh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3donpiacy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ntbtbvau.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbadeykn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vnggjtmb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3smzdidzx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pbcduore.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ogpharhq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nygxjeyx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3myeyaxvg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kjwjskat.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ooiwpbgx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqxhcoah.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rhirwjyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zvyrnryz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kqonoobm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3leuvqsaj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jeortduj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mgytwsrq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wtnmdxtm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rikktkwg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ywjjkggf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqcbtqpv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ifckdmvh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yrtlxaff.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3chtfhltd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gpmjfvxs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xscwtdwj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rqibaunx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wouxvzzj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3abnaoqao.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jklnamgi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3uaokfdcr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zpeownms.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qmovusdj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kmqgtjuj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wljiiymr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3srtgbyot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmtxpgi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cyahtmod.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3plzcndme.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3acwqkgwc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3utlrybib.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3brhzjhgd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uubohvau.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vujyhafa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ozagnmsw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uhamdceu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaesqpdb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ddzbbyxh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nqohchzd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3clvbkkiv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vhsmcucv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pyqhqznl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wcrolhyi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xlsdnfrh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hdzcwiat.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lubbtsjr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lcnmzdrx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zexsxevn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3oohiyosx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lqyuoqvh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pveksjsx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3skrutehx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wuwfzbsp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ubacahhf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dtvlmxmm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mtgvcbcb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3arqhqgvv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3eovvyoxv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rxblxdee.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bygunbzw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eprfrndl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cobuxvrm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tvnvpgqt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fxppaqgx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3koqanasf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qwrkwfpc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nxcktnwt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tvmknsld.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zhmncyyv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hycqnejv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktothsbj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gfjjfudt.html


<!-- 参考信息 -->