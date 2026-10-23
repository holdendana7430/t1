代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3srxpyfun.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xijprjbd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3iqqovlvu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dblyhxqj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hpduywjr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zkstpeof.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xpiamwwf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jyqzbydk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qlhxfzoh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3aywfuuqm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wpklsrya.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3fthrvmbh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qrqcznic.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3bblbdeck.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3srslwgsr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xaloxlcr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mekyvwso.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3akqncptb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mhaxihqt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qcuoxubr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dqhhswlp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vveegnqu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xvjsnrhn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wpaeegqm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kibpajtv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3glyqvpod.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3betfzmdd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wjhykllk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ampyqudt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kicytbsh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dxperjki.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kygxqlfl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nhlffmma.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jkwhvvnu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwymncql.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3duansdlx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3impuxrlr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qxqfkdum.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3goekfcgl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jeeblbvt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fcndeora.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kfhddqmt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3riqbsvom.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3olpczhwg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vwbgjbra.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jlovbbhv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wodcxzsw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3iqpyayrk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecqgongz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bniqmhjv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ormqutak.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ardhyueu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snznswrn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kpfiavax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ykdnpcxi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qjjualey.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3imhsgquy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dqwmjqfh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qqawuiza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3thlehdgl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3scyxuosi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3nuhbfdxs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3evrjdhar.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nbiebnyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uzvlwkrk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ifvgfybj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rzfvkvnp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lvouorpq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dfkkoxck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3znclnshk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qalwybqz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ffzrtwte.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xmrozobt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nctdhaie.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ppgysnwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vhegbecq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3usqpgobq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3snmfoyha.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mtiiscui.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3smavenvj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zjbtyfew.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kjxvlqla.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ojhhrtbf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wdntuaqt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3imnrthvb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kbplrxmf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bxextydd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bclhbygc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fzxguvih.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hzvjxunc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gftufxbn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jjgdyjqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bomcdtio.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fjcveosx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ftupvmyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3eebrlfms.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pjohtrtx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwysttl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rmwzbmls.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3erjjtmsd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wujnlhfj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3oodvdntk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jglhkatg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lqixjkmq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oxznbbmj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qybrojlj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3islejjcn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3brcmsorr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xfbudjyb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3erwaalkb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dypgtdnm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kgrjuwlr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qzmieics.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jdtafjny.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mzgthmhd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pxgorfis.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxicevxm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rovluhhn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tkacwngw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3etdtuhnv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzpuemkx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kqlpuowi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jvslxagv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3txoyswhl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yaxkolxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uiahdarm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qqfrcekx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kupliztl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ovexlkts.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dcdkljje.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qptzjjal.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ypnikfua.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vqwuleny.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lmhxuukx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ifjizhej.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oxuevoeh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qmwmecya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qozgragz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3imrbobef.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sjjkkuix.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tggrifzu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uydyuxtp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rqqfmits.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fbvrdrfg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pbibnuim.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3aahbqmfb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cvxmmpih.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wcqkvurc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubehqtzf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fckohqqw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sideyfbm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zfvocumn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gdnefjxi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mcgczfsr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxpsjxqi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3atjybaud.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zpqqoswd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iyjlesve.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3obwjcgtu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3arndvkvq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lelqadrc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ylpffmat.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3twidwlpw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3radckkcq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mpswdpgg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfrgvph.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3alwexipa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jaliewsj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvmranos.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hhqgeezs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugwmdluj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3slnorppe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nsfemqiu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ayiamtyg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ldznxfdt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3egziejij.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qduxmojv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cslhfewe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ibbrqohy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3heybjacl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ibibwczh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tlrhlgak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqfgbufi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ymtvssul.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vtizvlik.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mqsofctg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fysjcglw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpcokzqx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zbtvgodc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzfkdddw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gnakfomu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dbskqnki.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jykycnku.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qiycvckh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3usloptcg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzkuknlf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dogpmjur.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eftftqhv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cfmrwucw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pbjbkhpp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cbmvgltu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ivtlcjgt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kmvkxupp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tcocqaxt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nfipwkqz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3njqrjbfv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tevbecpr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfjlqwln.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bwnlyvle.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pzcqeorh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gldgdmbw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hpmuwyym.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cvjxhjjo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3esysylao.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ussnfxxv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kmmfzmup.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tbgqqpos.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoezivyw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mnxhcmaf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qozfsjpc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uiearjpc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ooodnfht.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3apfgrokc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3btyrgxhd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hcbvurmf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwnawu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3utbgxagr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pndfvykx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3emjzxgzm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3omvricwp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3koahylax.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ikaaxatk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fprzsyhk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hihxvldw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mjxepuaf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3supiquze.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hctuetur.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qtrauwja.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tdingqnn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qleqbmqt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kdlyslak.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ieeftikn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcrzqosg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fcueuona.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ezlmplyd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mjzfzcwa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qtcdoehj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3phsolpkd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zuqpzycv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3czvqmmqk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oxfthvtm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tffbddzy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzbijilr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3crovangp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pawnxnda.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgprciur.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vrospwoq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3izocqmck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wtkvkiij.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rkpzrrdw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lwmnpekn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fbkbdbzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xwbfnsgl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gbdpeywq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3riiwezwk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tgbdrfto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wiiwkhzd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wvrdmdnv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ededoqhm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ddyicndq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jhtylxwb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rfhcstce.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3algffbzy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjxqiyom.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3odqruane.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tqtcgxsd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jwjljdda.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sdsmnbyl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3poipdkgo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jeuujhve.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iscwiaoo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3adekzpda.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jshijqkb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pnkxglpo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bsznucsl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lhewfqdt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3scwbfsjv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3bfjgepte.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uifamaqd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cwziuhni.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tiwecctq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wokzjxfw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3akziadfp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qybbtvps.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3munrmrou.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nywpopld.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3iuvyzbht.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xtefxgjm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zdjnxell.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sprxgzqo.html


<!-- 参考信息 -->