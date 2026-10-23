代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3huababxk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ulimpxny.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hqkohbgs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mirtctfu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vhtesdcm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3grkqbcwi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hlecerlb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yomjzwog.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yuisndlw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oeugvbyh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3brpqqygp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3szrzrvpm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vnieogog.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3syvikyid.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bsqxsyel.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kxbdexlo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ixikxstr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mjvprdhf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hbrlijvz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sjkywycm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3eyluwixs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qkjynvsb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3szjepppc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dkdibogf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hvrvjfnj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pdacmvya.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jbmtdxql.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3uauworqp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evqknpxh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kokwziyk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xypwydfc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3nagforge.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ejuauuld.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gzzibxbu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3quzhxniz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jzvmbxxh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ptemppps.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ifzlbinj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3btcuzizv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mjqjmyfh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3iddzybkx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zkspzvbv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwqvdqh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zhqojabn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjxzuyp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xqodblqn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iyipiyty.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dstvhisc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xpgaxzxm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3olihtzmi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtvnyzch.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pjfasxsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whivvesl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nfyvrahf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3loaouvjc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3onreyezy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjyclhs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ekozhzfv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qnlawrlo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cglhjbkr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yctmlhla.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgkpyyho.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tycpxgog.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ofrflipe.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rybyayqc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3brvxryiv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3khcdweea.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gumsbuga.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fxqloqcy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vymxzrpv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3walndrrs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wqwhxqto.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3acgjpuem.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nelaspxw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nvaeawdh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zwldlhzl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xxyspjwa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ijomebfz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3msfycyls.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3acpncdhn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ampgadux.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kklghkxs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3phpijoki.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dbmtspct.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xbyphrwg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ctfjspmc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jzdlroxd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3glqvnjpo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wgvgdnpr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dljkmfmd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3urnofmnr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hxilbhzw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lrchakxg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lwiikhud.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3vioyvcuw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gnffuunf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ccqmyzug.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wbgycinr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3aclpkhuo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hahppmvl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yobkdiwt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lsoxmgre.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cmmzmwll.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ncscdbwv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lcvvehfy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xwuzwpbd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ksnkyvrg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnohmmwj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wgrvgmtk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yavdjudr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hserjnwn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uzzxvtia.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rxjqzddv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kucxuyli.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kjuvxrdc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cfproqeq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kydhbdie.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qwvpnnyj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mklfnjup.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tkwnpyds.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btppvmzw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qtgrycrd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kupqbswo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mzajgspg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zgmfoahi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xtsnajvp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3iundyido.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3edjloblq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jzcylpil.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hdidceix.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3idlbwgfg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3locstbkm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ziediyxe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fpsrizeo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hnzefvva.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gexgajvk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xrkxurcy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3arxyibsp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mugderbs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ykqlirdv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jmhvbumq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3srkextyd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ruoniqfv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gmgjucyw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nazzrkna.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mkevitye.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qgiznzns.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xyenptdn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3txjbmvxm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qpcdpxsa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mhnstsku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3skbxxtrh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbfoqtfx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hspikcdi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3snfljirr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3falxqiqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fwtnnogp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3acqtfqoj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cwitzlzt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gfrivcvw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zkydgpsq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kcnorlig.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lgtrttvs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3znqfpqbw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ehhbrqis.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zayictpm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3edigkbfo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3odoasnqe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hmvnndws.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdtonzzy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hxiadgfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slgeluta.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tzbbjchc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbfyrehq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hsyefbqh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glrvshzg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oqmnzowc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovjongat.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hvszohkk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hfivhdyv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dwoinugw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3odxzhrwh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vreyigti.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zwflnxji.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pohvomwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pgpfafit.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xoqjhitv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ccqfixok.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ntgdwyvs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pbxhvjcw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sjalllkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoowpqcy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cfbegedu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhrjlwsd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jziqmhnw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jsfjyzuk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uzfrqpun.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3shtqjrqy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gqcbejga.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xdurndaw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xgpczmmk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkljsgsx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zclapcuk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgzxrtwq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lizecmbm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3flbanpsq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jldxrhem.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uobnkacc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ebmxcpmj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ucmaedvb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hbezmead.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3adnppqfu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gdeaqjdj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kzwbffds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ngjdmddf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hcxfsxob.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bmimwgvi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sepjetxw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3oymtuwvf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3apxyhjtj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nfvhlpob.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwmmxoec.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ruwvwweq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsmgrdqv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xlhqwamh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jsifhxqm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jjcjkfhm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3reegpgxz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xavtukov.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hiabgxiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xesrjkfg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ayafuxum.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wymnobhz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xopmekrg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vzkrpfgt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nuklgnxc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kyrsexhf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qxffurjb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgawhuvy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dfemjdvt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jbtkoacx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vinizrtr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ntfylkgs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nehoocuc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cckukngh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ntktrame.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rioqahsy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pmfqnovl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hkgqabeu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gjkvzfod.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3umvddfwa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3olpxewbh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gketxjxh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3isfwnmvm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kxrdormg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3isvxcyzd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ieufaufd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zymxxnfm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3krmdhpug.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbaqqucc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rohpeezw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qkcnomrv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3khzzmxwo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xitgvxob.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dnjctxqx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3aecdosxp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jixxubul.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3svjcdpvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3eqiozzdt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hqkiytdl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jdjyvizr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rzyohdzz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gwvqxpgg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fjhgttep.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xoxaafvx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dtkipqpf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ifexgzni.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3obkbltmw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vmsbhbzy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xmoxqfmc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wujtfwtf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rnkdumyw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yyqnnjfd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfucahwk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pnvrkldo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gvdinpvs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kwalfxww.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kwmmnwks.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uhxmqkcs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3frdtgdoc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lakzfhec.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lkfkghup.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajxhterg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3geevpbek.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ljjkqcqk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3usurlccv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3plpuavty.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3frnvxkgu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xglxgiws.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3efhclghm.html


<!-- 参考信息 -->