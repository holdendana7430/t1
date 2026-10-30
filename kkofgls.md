代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/glqpmwbsb.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyasvhjk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gswprbqsq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gndobchud.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwsuboc.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gjvmhwtnz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouzsiggn.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gzacxcoyd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ggkfnfaap.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwubuxwj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlzbwqjt.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gyzteixkg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gzagvtnfz.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngrzwkdh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewkallf.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahbfzkeh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblhsnafe.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gsgxqcdqv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjvwecm.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gkzxmkskk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gbadlxoqt.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrjkadrv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoayfaio.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gkhwnsxwk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gabwgifci.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/grfeizhzu.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/geyxjobmt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtdbbgra.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gkrkjzqgk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gkfoaazkj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/glupfldps.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmcrdqlf.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkciczljb.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqunuapjm.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqkmesjc.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzniodexx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtcjgakw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqgetxnz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gexgaqkzq.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbglttlf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxwjltmg.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmepykii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnktrpgdw.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gsadrcuuf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjlogwyj.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxrhblz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjddttzx.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcmmdkx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsejmvwb.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gtltoogpj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtubivdpr.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gmryvhjks.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqgjuvyo.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpeoyexn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpkxldsyj.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gzkorfbce.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gamniusox.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gsmaeituo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoaxmodh.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkzfbfkc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcipjtwtn.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeficslv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ginkalhty.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacybstr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcruhvaiw.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcmposb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoaipocm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/ghyljwruw.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihxmpbc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfmfgkkr.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/ghevlubwr.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcaejziv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfdmmuad.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/goctdrdkr.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprgbsyj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheygxoam.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvpvktbn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggokftwpx.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjypbultv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxbwhhz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gisefjptl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzrmibrx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gqddbodaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrayzun.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqajolcsw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/geeyjigin.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzlodfur.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuenccat.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gvhtoveer.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gfaddyzzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgswrnna.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbsbuoc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfjxwsik.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnmcqpli.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyswlgpe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyttwmahp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhlbyedh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewuudmy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvtlmaf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghktybcog.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjmuyrsrd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gldubzsuh.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gectkifal.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqsjqfej.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufqzovt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gcrtoeyjr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpctkejm.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbdgptfo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwgzvsc.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoveknft.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/grxrxuqqd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhnteeex.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glodphaxh.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gcubqasou.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgfqohia.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsbjwhmb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfcxxiq.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gxkvcoyja.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmxhkaz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkuogiun.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqhwvdtk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gyzddzmai.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/grhxkawqe.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gueafdkkn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbytfxbv.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/guqambgem.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfmzaucj.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gtyrjkyuu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyettiezb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/girzymglt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlkghxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/guywhdnsq.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjhpswie.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/guxsjwjde.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxdzocq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbgrhfag.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gikesndlf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gjfdmibxd.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glxpndurb.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gjopbarab.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grdqqkqzx.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gigtazqpx.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcxuogya.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjvuefwy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenaferu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/grgolhejf.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsbmrepk.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqvytura.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxqfarxl.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsuwvriy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gutlqvmqe.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/glgukaxwq.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdxmbwv.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gznkewbgr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnfdtydc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwouwiwq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdoizmqw.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gvrbspilw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwzjrzfh.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdxtoynky.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxbcmwp.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzswynkf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkqgvcfz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpsqxpge.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjabpxcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/geyxljutc.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjigdan.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwiuuvup.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguwtelcn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgxafuss.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhhcmlzu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gusazvbgf.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpfcnjbs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyyahghyz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotngxlqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlyejdzq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmohvxpnx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gekahbvss.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfcdrdvh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkqzxkpr.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/ghtdsrdjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gawdcvncz.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gaqdrhabw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtoonlf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gsjcokzrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbssmtd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnatbumyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqrsswrz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtupravq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqitajeh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzoihnqv.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwxkxwgug.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gvqkrasfx.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdntxmjz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrnbbwlm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixosabgl.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gegsoppii.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghdkjszzt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgrrmamp.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcitngty.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmpppljz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/grxipbntd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkbknbh.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmzycrkp.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyejxanx.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkqtlfuf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqlljia.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gddhcfltn.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glasrpubq.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gewebtgpj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gepbxfrck.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrkjzvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtzmteex.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzuquhdt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoyrbobu.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxqspozxm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphiwhzo.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gkwcycvxh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtqxkqqjp.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ghccrgsgw.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/glglcydnr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbqpioyo.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gevgdueiw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlmhxdyk.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsezcmain.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbnwyjc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glhgqurrj.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzflssmcq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gupycdzsf.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/grxvkhbvm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggccgxkfc.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gshtdlkgz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/getvyhsyi.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gldjksqfs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/giczabufl.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/glflcikgp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grogaosnj.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbywuxvxg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glssnnaqe.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grngrhucq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgigqlqa.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gshzeipsv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnsyosry.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnymovies.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/geuvjoshv.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvldppqvu.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpyamxfj.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gclchmibk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjavrqsl.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghecnamgt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgzjpzwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvxollinm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjgvuew.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gulxzpxey.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gkoejenir.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gidndbxmi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gczcmretr.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgpsypya.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcewtey.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpostrwqg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkahegir.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gkrfuczdg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gzbbandnw.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuozmfss.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnzybeox.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnippav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcqogbbfa.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gktysxmps.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/grbgpjjbf.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gakiepjte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/geflrpsrd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gturbwckt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ghivaoziv.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gogkfemvf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gtknpvgrx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzspucvm.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/girlrrwgw.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gfkytzjaj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehpwioki.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtkvrelfc.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gbjohlarw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpqjmirr.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhoebcah.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gprbotxev.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwfisxq.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gtbjofjqv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gigelghif.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujhebipm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gifggxtgu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnjqoghc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gotchkdsh.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptrmguzo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhxuyzqk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gemwtnchl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkikhisx.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gljfkjpcp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfosmrxpz.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoorqjbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gchodaehg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghmkmmxgx.sHtML


<!-- 参考信息 -->