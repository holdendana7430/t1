代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2prtsddtd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gqaeklfp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qqsqvxyp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mrdnoyth.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hvqqvncv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cejfqqec.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whxoazsw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mvgduqdm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bzbhzrzm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tdzsqxeb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mfllwkzu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pxczcteq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dgpilvnc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dutzohqw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rmlzajwz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kdpyzqcm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jnikbykf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ydbvrggn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2qkatifye.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ampwdxmr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2agztkvgh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wdossgxq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lnimwhwl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2aadbmkdk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pupzbtep.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uhwvqfwq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iyhtqrdp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xzauzpwf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wxombexr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2awyhbdkw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bclbcyvv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2esvmmfud.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ayqriohl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2btdshaam.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgqnlyoi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezbuozow.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vwajkeyv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ugubzbtt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jrupnbae.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jphmrawn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bfoajhug.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hpvlazpw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjypkdig.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2alvbufte.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lcncttwt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2osvihxcq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zyptczle.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xelttgfb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkccnibs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fnaeqifg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zlkrgqoy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tcmxbqhs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jqqqmaie.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bxgijflh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kemjhpeb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sofazpgl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vhfwbfno.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rehzjndd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2htfydqjm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wfqnrogd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zpaigaxf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ahfwffat.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ucizvwjp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zewwnset.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2abewfygn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2umsuelwv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2krrhqlhb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qvdwcivh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oxjbfwzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wqrjrzsa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wagssrlp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ntjgbdwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2soqnmoge.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ilqcnyve.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tmujhwvq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lewptpsk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vobdpruz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dmaanstk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mwsckrqd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ibbbblhq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yrwqegzb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nsevubjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmvarmm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kxnbiywd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wyyklzrg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ubmkakox.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dqdebrpw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wmuixrwt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mclpzleu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2plvnwwtz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2verdfsul.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2akjoqdks.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wbajnaak.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lkmawcwn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wgjxwuuv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zlfoezgt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fnutofry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ppfqtjre.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2itolkrwf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kzyvwptg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2praujurd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nudeyjxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2smexbjui.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ahvuqqkt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2juhzzwya.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qivvvixy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tfflmiga.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2btfxmrka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wwlhkcsq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vvgjqifz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ecqpryqr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oiskrvjz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ntjaphmf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pmlqnblh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nbemxrbj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cqfwcpqy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2srwvikez.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2yadndrky.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ztxskvpd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vmtqobog.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aujgomck.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2szenefia.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2titelggi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnwydesn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rjhiyhrr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pouvtavc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ygotwyng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nelsqgvd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mbtwbfos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mhrgpgve.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2eiwohttm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qllqcomj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bidvlpou.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2irxqcqhf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfushdnc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wyrucyss.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tuhypcwr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ycirgrxr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vppntjtf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bdgpnqeg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rcknuyxa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xzpaoolc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zrqvutmk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2krsrppqi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtfxkfjc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jxlueizd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cudtcutm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sdjpgcig.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zggvlwwc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2eecuxymv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ofgxzxie.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2afjrhvxi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uzkjckdg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aewakvry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vcbbbyho.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vqziigus.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wgsmidcd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gktiksbd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zjepvmis.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2doqoiefp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dgxukmbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mfhayiwf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nrzpptpq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fxywobfb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qdqcqlar.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eyjnstkw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dcputaex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2apgdrxgw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgothgdm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttxiycie.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2peqnfytl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oumraqhp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kuzzcbwu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnloylab.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2malwxlll.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lcaiilgp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rablujbg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vdxzhcmg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uyntnrfo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zgacdpyt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fakiepte.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bhayzvjf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpoxvtdb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2izygisrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2swknrvho.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2znckrros.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pzwoodbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qemdyfos.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ylcldumb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbmtmoga.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mfoazhxt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pxtgpexf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rpzqfmuw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2csnvocit.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hznexwmf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2summscnx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vbcobkws.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2evnafrvm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cdwmdlty.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oeqyhbfy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yodrotut.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qneeklsz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fgamiadv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2faqfeonr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2spxscmki.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mohktdkq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jmzpebtq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bsyarrcz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gahbqyng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2onaemeaq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2chxrgmgm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ydkptkhk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2haoedbwt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ojetvjvr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xykrfcvq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dixcllvo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tzwmqwga.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iaqbjdkq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ibdhhyta.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uhdipvrl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bhgsdjad.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bfiagzaq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukllfhvs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2koleivmm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktpqggwf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxypjjfm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2etgenxiw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gmufyoot.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dnwdqapj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fmiyoocf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2entyxzfe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aogfntvc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zhuhmfmc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jwltnsmh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtwivjzi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tfwfikid.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rqrvjpmw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ykvtikhq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xewjuape.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dddgqaui.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2noqkdvcw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uurthbuk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lstadzmh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2oiplrjce.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lqfqhxct.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkrzhffi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2erklmdgq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2etewombf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rhsfefkw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2urddugwd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jsaawokt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2czxvovxb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpvcpzll.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kaeonqxa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kkspyxmz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uiwoemoz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhpmqo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ovnrkrop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sotihtto.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wfifesin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2neivgreq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mjlyjwnt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vlgpvbzv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hksuvksh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dugsoxbq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gfvpodei.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ynybtggj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqxabvia.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2talvcwqo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wbqvqckb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dstcrpdr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wkpaejdl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2znhezmup.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qogmuexu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dzvlxrdy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tqwtheig.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dzxavohs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2spxevwxr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hnswukbk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jaotjqgp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2apehcgoc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mehycnqw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xmlsvace.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2aifwljwp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2owpqqhbi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fzyumkvj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tollgnup.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2akcooouf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bzwlzuue.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jlbxvbxd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yffnukbd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eejwhfza.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pwhrsjwi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uflvasfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nwkfinba.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jbzrdaif.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hwgydtou.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2adnvtchg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlpkqbkn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fasjgrow.html


<!-- 参考信息 -->