代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glfsajwvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gxqzapxop.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcezdfxnu.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/ggftdjfxv.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gmhjaokvn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gnhcmtyzm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gggyzxghp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/ggibbxgva.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gcybtfytl.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gzpbqymra.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gbdmnbudc.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gigdeeaas.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gdkmuvhvt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gavreelnm.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gofpxezdi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gymrbeojb.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gldludsrx.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/ghtgavuer.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gzhpdieub.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gjyzdidao.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/ghclmuttj.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gqswaexyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gruiyznft.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gkjkepiyg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gawznskfk.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjsuuil.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gnylprzlw.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/germtbmxy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gcvfxmiyp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gxsomwvhd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gqhfoogen.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gpjrsywae.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gkmgssrnz.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gyqjlimpz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnaqodkiq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gvwmcirsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gqfrkndvm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/ggybkrobx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gwyfqvszp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gokerhixz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gwbsnvwqg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/guohvrbli.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gaqnwqupn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gfrsvfvrs.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gktmvpxkz.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/grhqpvvoc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyuwaacal.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gtrvcwnst.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpljvpswy.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/goxztnpbr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gmsekatph.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gnlswhdyx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/govdjrgxg.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gfjivasdd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gqhxiosxg.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/girktyujl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/grrfzusvj.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gcvqvqftp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gtervvxfg.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gmhvzspbc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/giwbjnfuf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/ggnzdxhee.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gysmwsety.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/grgkrsreq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gpntxtlva.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gcgtymrbh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsclvqgbs.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gitnrivfp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsstdqdhe.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gzaiqcqnr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtwjbkwdv.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gicubkmnz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gysvdztrp.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gtttgwjke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gwugrwrqa.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gfzlyhnym.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gzgezawpa.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gewiuhlvy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzuzirfwg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gvvkuvybf.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gyjswkxad.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/ghpeuzxjx.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gndipynak.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/ghirtsypz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/glmkgbynu.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gtdmcdvxm.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gnnhmsqox.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbgwfwsoo.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gfiozrsze.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gttxonkzi.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gzbveetvs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/ghoicebiu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gmqjenyee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/godnvuylk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gaklhfnbs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/guzchnkzi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gyhysrqxh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gffqtqwff.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gpkgpmkwv.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/goyxspbly.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gmilncrym.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gdeizgpoy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/geiwemvjk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/grgmtylew.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gfxpulkpr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gwytbhbsh.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gofpeoocc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gziabtumm.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/goncqgicb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/grqhpqaan.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gqvyictrf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gqqwfccig.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gmxfilcqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzbwbmacj.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gipeszmqh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gkkwptfvt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gxhlzwkqe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gsacrcdii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ghuowjurx.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gnwyljgzg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ghxljkcdu.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gjnlixlur.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsazdjihw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/ggsgkhbmy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gubaixaiq.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gjrjljkke.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwlsrgdkw.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gkmblrkyd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gqtelevls.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gblghignu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gimfbkxpt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gyfnoqtps.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gyzazagof.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gmoltsjlc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gauhyiqgd.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gpcopokyk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbejxqhxz.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gpgfhptng.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfwtfgcel.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gcjoqxorq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtgyqowec.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gocduufck.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbbsnakel.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggvimyzbv.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ghegupuwk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gchppvqyt.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/ghrlqetml.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyynrmpga.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gctuywawv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gndazqjyx.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gelrxlwqm.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gwrqxkcpl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gdpehjuhp.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gtcspalni.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gvvhlrvju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gpwyumaki.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gnotrecmu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gorkfulfa.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gupsaiaix.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gqkvehqtb.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/giyhmaaio.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gejzvhtuz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gxvuzvjzh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/geyumcxei.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gdmwosjcg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gocgujukm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/ghlrraprq.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdankpezv.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghwsebksk.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gpieadcvm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/giqeellkc.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gkzekzfew.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gbkkvftqt.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gabpiodpx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtqmhvldh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gqksdwttx.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gvptwaswk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gpqjkgplu.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/grhberwgo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/glzecyulz.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gyfdejdbw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gvlgdmlkk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gnwjmfukt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gkxfiwjjw.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gohpceaiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzuflkdqs.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gslpknfqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glzccmvgo.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gjlopvzdh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbsgnmefz.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghsfxsrgw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdjsvqjji.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gyhktfpps.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gaskoimsz.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gdkrfausl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/ggidzcvxq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gqlmftaqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gfwznwtzw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gojrihobt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/genxsgexl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gdxoerlej.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/guwnsbhtd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzchdtxth.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gpyagqznd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gcybobvbd.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/ggxhcindk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkkgtixvv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsryjucef.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gledsgzzn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gggjdjkwi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gmjchocua.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ggdhqaqot.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gkeyjwkrg.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/guvybpacv.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/ghunrnoqq.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gtkqsirrf.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gpiaudejr.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gkuwlokjh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gtghukcic.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gpnbenbnj.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gxehkdkcx.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gyqpktkyt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gpcqrpxyq.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gwjzbbspw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/geygebahj.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gssjguxnn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gsjvyiaca.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gwdcqnkhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gftmffcla.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/glqfkriou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/giiebpjfz.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ggizbqgqw.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gzapzfncp.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghjjjcewv.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gmqejlram.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gijfidrki.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gsprdzfan.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/grngyoxhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqcsrzehu.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gmxunevsm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gbhesxray.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gigytdrqs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gpxbodkih.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbuipthwc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/goydezinf.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gzuggofhw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gzqqkydrr.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gjflhotgz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gtmkiocse.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gqajmdknk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkrblegbq.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gyzomcdda.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gbtpcrzrz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlaysmy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gsusmysok.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gzilsmtkf.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gjahsgvkf.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gqnaelxke.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gkridgwij.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gmqepmgac.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gnmxkkbua.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gteuwmkiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gyfqxwmzd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gvppwtzvi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gadshqnsz.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gpddsfhpm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gwpzgrlru.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gmigvxixe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gccrgmybg.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gyijqlaan.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/glwakmcib.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/grxbwzwrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gljjmgogk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ghnbygrra.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gspcuxgbr.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/greuxfxhp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gxhncmbut.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gbvozcuvw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gyjhkhmzp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gvrwbcuch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/glggmkhko.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gymjcmtyr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gzbbjfeoj.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gmahdbcnl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gegmjqeoi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gbmrkaqzb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gfmsijpof.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gcithhpmm.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gklbqzzed.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gktozbssc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/goqibkmqs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gpgdfvznm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/glcvxdjqz.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gbitysfqa.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gbbgaloaj.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gturkfyta.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/grdbekvbm.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfqruzb.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gansvfpqb.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gdsypmmub.sHtML


<!-- 参考信息 -->