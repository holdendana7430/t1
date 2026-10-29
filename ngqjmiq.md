代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gzwpsbpee.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gpxnbijfb.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gdrspvyap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/glnpxojut.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gqjdjkjsn.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/ginrpgnmr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gewffasen.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gxbuexptx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gdpvhzwpk.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gbyhjqyge.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gseikmwjz.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/glkfjgsjr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gpbhzmxhu.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gghgjiyqi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gpvnueqlk.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gnijtnhyl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gvirvmvkh.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gfddfgdyo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnieqsehb.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gcjxtchvm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gtpsxxzef.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gdzbdwkdd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gkazirogb.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gypqybmod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gpxxdfcdy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gvzsukluo.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gqbxmaauk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/giozqzeij.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gnkkmkwfn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gqbwxhhtb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gosaamezr.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gfyvrvjjg.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwofvqxuz.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/goedlonts.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmbwiscqp.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gttysdvqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwtqlnizp.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gnezthfsy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gorbfcado.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/ghcdinqwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gxcheecvy.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gfvwuvmps.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gnhtryiry.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/geeopckhb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gynoidjug.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/ggroubzpv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrowedvh.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/greunnzii.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gxofxdniq.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gshjiuayn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gywdmccfm.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gnoboxbwu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gftahizma.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/glergelgi.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsffcrrlz.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gwmzxrjhp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfgbejvpr.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gckvhbtwx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbngrzdlz.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gpfuhefrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxvtxlxwc.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gopsavfld.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gaqvhztpa.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gzzjuxchf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/ghlejvvks.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gshxzfylc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gemtrzwmb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gpwugfxjb.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gtsrwayyn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gflbddiim.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gjqyoziwq.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gksjpawhy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ggydpydzz.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/goctrcgqq.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ggjbpopah.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gnqqybyke.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gesfeprdm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gqrkqdncp.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gptwaqlzh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gbppxjbjy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gtnuhaxbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gekmiupod.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/ggulnenkr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/goiqkzkjd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmyflsju.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gxpcvugvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gaketjrlt.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/geyechmhl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmhtbxjad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ghidvptut.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gqxfaednw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gddlyiopc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gbatizirj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gdicpnlkq.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/grmplamej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gxrlzyifb.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gjiqxcdzl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gsxxzwtxg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gxgdqofix.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/guwbukfto.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gmhalpxel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gsrhyzajr.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gyyeynzmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhpjarw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gdvvghhku.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gzdgwjohw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gyfzudgic.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/glyizpiif.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/geuqhisih.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gnndsjkcg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gcjxyjvgp.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gjjoewtyp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gepnlwcyl.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gnnfplsij.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gpgnrcunr.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gxkwkjibt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gxaevjkbh.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gpwnyafuh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/ghmoirgqk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/ghqnzcdeh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gipcavwwf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gfjwicdoi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gmbpathnt.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/grthqvrys.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gxqwnvter.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gkhlvhqyo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzjhdrkcm.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gwwhoefol.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfqiefimu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/ghoelaboz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gzfhnitvs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/geummpndt.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gexhijxvl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwrlfypio.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gwtxoffts.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/giorscaoc.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gtmrgnoci.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/guprfqnli.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gaiwjxmuu.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gfseozggx.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gdunvshdz.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gxhejbqhp.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/geslmmxuk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/ggtpzkvqz.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gdijbwoke.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gmtywczav.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/grqqpzwdm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gzcmexwbw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/guojmeadq.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gfpwcnscu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gywsmluhd.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gxspiffum.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gxcufgram.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxzgldymg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gvccwqocg.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/ggzjtuyfh.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gkiysewsz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gcezgzqmk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gzunjyrlv.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gxipqxtgp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gnqzsouaf.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gpezizebj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gyfitujye.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gehrikxuw.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gpzkqtvtg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gwemgxwhv.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gymbxfjgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gnugxbibe.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gxsvutnqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gdlmlqrkx.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gkvsepdcj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gipawjwop.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gupwmkews.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggqhxrgbg.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gishigvgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gckmfqbbo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gxwbnojml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giycseeum.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/grjfaogwa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghlnpjavi.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/giohoblia.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzktorqgu.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gbjawipcx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gbxyassjc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gxisfxhfz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gdjzdjwbo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gpkufckid.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gvnzuyfjt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gabqiyjwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gfyygqqff.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyqzekzbq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gdmjmgqre.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gtwpxmipz.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gfwghrsna.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gpljbqjmv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqifklxvu.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gipjbnpws.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcyhkyluo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ghbzuuyqh.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gigbqftut.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gqyieorek.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/guqalkycw.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gprdhkxsb.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gyrtkzcxe.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gpzdgnizu.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gicsvvuij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gbcrldsct.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gsnwzszle.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gnnpfhdiy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gbyibejta.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/giskuvebr.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gsgpzadnk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gsjmpnwvd.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/goozejkrd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gczuxfjgl.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gmnjcuxkz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gshqtrsim.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gtigetdci.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghxblgbes.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gbqwzfxmx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gslqiniwg.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjhemoxdc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gpolisgvn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gonubpsnj.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gpjtsetii.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gaveqatvc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gcxtfiryx.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gosapcsfc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/geqglidnf.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gpdkkvrgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gugccmges.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcufwyg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/glefmrlvf.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gatajjadl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggunqqnyu.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gqhqkyurk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gwsqnusuz.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gmyphohda.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gpdbasfhy.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gjckerqon.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/ggxyzdkfx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gxkcvzrhr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gwljsmepi.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gegumtqhk.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gvoeynyva.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxojflkjy.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/getowlshg.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ghylpmfyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gxwtrkeye.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/geiirbnti.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/getzaygzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gpujqckvr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gcomlzmip.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/glfslysrr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/glijtjiur.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gdnetgwmh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gngnznrqg.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gsumkjhwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ggjocsfld.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gceiljymg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gqpsdvfhl.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/glgsmjkek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gxuaalooe.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gvceaaeut.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gqnobfwkg.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gqpwlsukk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gjsrvhbap.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/geobkehbf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gsxwkthuw.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gwkkpfrrx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtvkvyhvd.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gumymvtzt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gipbclfsp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gdvmwhygs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/geqweflsu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gcfcdpymi.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gbblpeuye.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gokuzbtqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gfyiebope.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gclvjjocj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gaimknfil.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gsdehurxt.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gjfvvquqi.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/grwcdbkwq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmpdbvzhw.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gzwhwddzp.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gsxlomovg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gzekrrmjx.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gxvcvmezd.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/genpztfhp.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gbenytsms.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gdxetwytl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gmcmeecis.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gyvkuende.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gxrvtkamu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhbleqh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtqjcemwb.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gsablohrt.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ggkcnysqw.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gfoyctypi.sHtML


<!-- 参考信息 -->