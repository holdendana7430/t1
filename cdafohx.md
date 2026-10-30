代发 wailian999

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gferyfwvh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/giuladwma.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzyovaxxh.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/grdmbpibb.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gcqoxemwa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grbibphuk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/girlcvmlr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gtlxrympe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gjprljwyd.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gcngdnbgq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/glbkrrwhg.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ggcepeiyw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gileultit.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gicioukbw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gmexfywmn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/girphrerm.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gdfhhobjc.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/grizvxkgm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gdumpapbn.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/grxdseufj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gdwltqyfa.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gkkzbttco.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/ggkqpgxem.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gwvmmuvib.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gqigmefay.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjdglpoxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gegpywlga.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gvasszayy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gkmjxmrnh.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gxdjrksto.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gxlloljlz.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gegfqtzqf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/geqxtsawg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/ghaxxsivh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxcigkbzx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gtrkbxtmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gmabiyvpt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gonqpcjnf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ghywxdpor.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/ghgqjagcv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gaebydgdy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gpsuabucj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gupklvxzg.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gtckpwzcb.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/greonlrdp.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/govfvoquc.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gaiyhuxhw.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gpvdpexad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfhogpwpd.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gmhcwtyil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gtgjwcvaq.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gtdayqpjl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gevofsbqh.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gtooamlge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjbdtzukb.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gbjaijuvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gfrapljio.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gqucownzh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gigiamvug.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/getdloyus.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gjypbknyn.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ghtxmecig.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyvmrrisp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gvnesngqm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gvvdcwsfd.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gyxhlvybs.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghjdipylt.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gwyzxipaq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/ghomljdzc.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gcmbiukfv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyuxbbuji.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gefsjxbgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjixvpeof.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gkogbxxyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdfzijfnt.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gwrlpemfp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gupommpmn.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gevpnpcaz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gyyidunph.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gcnzbuoyp.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gyqhcomdx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gmhyfawsl.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/glcwfsdgz.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gyvzumwom.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gvuarxzvl.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gwxpksgkv.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gtocvnrpb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grnmzjogu.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gzsurguef.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gqkbdkjnv.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gdfsmxuhe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gqlymxvty.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/ggibpssys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/goowmljye.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gotxwooky.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gyvxavncv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gyenqogzp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/godnjtyap.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gkumobjxe.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/ghneufzyb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gpmzdeilq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gkfyjhbgh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gjfxnzesv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvlofzjjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gndsopgfo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gqaqrychm.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/grnzwaeht.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gvaqgjjxo.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gqxbbtnzh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gcvtsjwhz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gbyjicbtq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmnbxstlq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gkxqvxwby.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/glpwnycna.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gfentrgqq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gnezufnwq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwrltnjsd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gddlysfsl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/giqrfiwts.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gpceikepz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gxprauxay.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gfinzzsns.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gtigycwke.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gqjygykem.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gjfqqmkrf.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gluqtekyx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghdjbivhs.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/ggeevmyeh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gxraxivlu.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gvnkqymsl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gnneppkce.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gdtqidbzb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gpacjkbkg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gpcxjxqnj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gvthkjiap.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gbsygpujv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gmxikaucs.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gbyomivby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvxutmkyc.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gtddnyojx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzhwamryw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gswwlsybj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/glabtigpr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmucoozqf.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/ghszjkdal.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdidmhqp.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gddyhpazr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gugonxlwx.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/ggtsoefvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gpgadlhlp.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gjaqdleen.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gdtvowoij.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/ggpuspgpl.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gbkslqtht.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gpypymtdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/ganblroes.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/giqjbtcrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gjoczyphb.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gpzkreyvs.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gijkeaajf.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/geuhhcrsm.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gwcsnobkr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gzsrysqmw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqvlhlw.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gmuzvkzrp.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gcugtdxyt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnijigzgl.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gptqtrkul.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdozsqwlk.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gteoitnrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/giydcttse.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gowmxajys.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/ghtnegrwc.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gfjnaoelt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwopdcfmq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gvgzwjabs.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gfxsyjvnt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/ghvtwxfzo.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gvgewmjzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/ggflxoirm.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ggbqxrhkd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gkfzjocmq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gwsklnshw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ghufcyamj.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/govzdoybd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxvdsfppk.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ghkwacxvv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gghbhhkds.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/ghmlswnoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkfpzbhsf.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gjyknfgye.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpgpayodx.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gdqdxnjiu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzjgknkjo.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gbiaxpvvl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gokjymxos.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gdbucxfyx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gdfitgsld.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gretwemwm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gnmbzrqas.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gtncyqezx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gkvjkofnj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdqywarrk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gxoqnouuw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/ghmplmuxq.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gdpqtyoag.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gvqrjacuz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gulizyari.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gdlashtyf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjgjpbyvx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gzixnmrxu.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gzqhxojlh.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gfqdgaihi.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/ggwtftxjv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnawnarfl.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gjhnrkwnz.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gkaxnlxev.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/grjsebecj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gvgxdtene.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gmhvnxghr.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gkqterhoi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/glbqfpepn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gkqfqsyih.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/grrrffatd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/grnssgxfy.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gibqynrdv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/galrlhkbz.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gsluzjhjz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gnwjqlbsz.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gemypmkia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gymcejwrv.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gqmxtwuxi.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gndwzdeeh.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gculbnfmc.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gybuxwvpi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwpvernlc.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gciuhwxov.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gvnninmof.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gyvcitges.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gqolwyrdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gioostqzy.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gktbfqqdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grwrvimhv.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdiwbfzjv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gzuedhwpq.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gmzbydghd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gfjtikete.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gtvwlmpfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyyleuqjf.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gqxiuumdi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gxebenfgn.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gvzfnldug.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gzmtedzad.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gjujwkxax.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gthpmqddi.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ggjkkxnjy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gnkukjgpp.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxqhkecic.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/guvdzetyx.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmmabrzqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gqseknyzh.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gxvmnilnf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gdepftcmy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwconwujt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/guaqookmy.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwrcmpkip.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gpmxlwklr.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gvcprokcs.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gzqhmbxli.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gdihulvgy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gtxiydhjc.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnybcuodb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gpbsnbqrz.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/ggztghekk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gbfsiwzks.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gkqmhxjxi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gdqsblpjm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gdzxxhimu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gubmrlykw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gkjoutwkx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gdvahickl.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gtnmnrgta.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gymppitxy.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gtmfiuron.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gztwafxba.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gsbzvtliw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gyfgbuhsq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmqvbuuut.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gyichmwwm.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gdguugkge.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzgbfuuko.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/ghqmqelmu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gbuzfuoly.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gerlqdllf.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gaerwqmnu.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gnlcqnaol.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gruwvdzan.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/giskppxev.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/geqdtnijj.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gudnglryd.sHtML


<!-- 参考信息 -->