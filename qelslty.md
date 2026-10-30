代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/grtstuydr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/guxissaon.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gmcfkpzyu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/ggywcjsyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghexxyteu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/ggflqnvbj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glcablopc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gsdstxagq.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/ghuhtucnu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gbkggnyft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gdsfyoqaj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gcqsbvpeo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gijlkmssk.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gwemgdilh.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gcprizpno.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gvknlizjw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gbxjyqphj.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/goycjdpjd.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gesvajsab.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gykdhdkjn.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gcsiocklg.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/giqhhdinp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ggdffvtqq.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/ghyiyrnjv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/ghrnsrqal.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/ggknxuyml.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gerulgkvg.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/ggliqcnbr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gltygeozm.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gcrgdzeku.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gwiskghxi.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gzbeazowk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gubbbstmd.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gfxszylpo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gbncbmfah.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/ggnjdquvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gyfbjjxrp.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/geonkekmh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gohtwfixr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gfikhtwgo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gbjqjghfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gwyrthubw.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gecqgqlsp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/guyicnuou.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gdlvuykne.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gfbasfufh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gcpyouhbx.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gdodaecsu.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gicjdqddh.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxuvbzfzc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdblfrjzt.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghscwkrkv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfrifwizx.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/glrjcoznp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gljjmqnmy.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gtaguksfu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlxmhoob.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/glfrrrexa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gimzjfehz.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gvkgwmvnf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gckccghwj.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gpsclctkb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/guwvzsxod.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gpyjycjtv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gpdkfjfhu.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gbeehpbok.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsyvsihzj.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/grqfoupey.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/grplrcejg.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/ghkrvkbbp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxgkhsogn.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gpecmqcms.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsfpolcnq.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/ggtjjhttc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxspauys.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gxhtcjtxl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcwqsgsgg.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gvvbozxhf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gvcdljmjd.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gpqexcyfi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gjmevootu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfcrpreos.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gkhgbbqvp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gdotvutgp.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gflimydum.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gwltqpcas.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gaiafubax.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gnicqffls.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gvbinoqgp.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gdgzyvwuh.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gizgshprj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxdljyfqf.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gxeniyesi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gdepaibgw.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gedwsonnh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gdembstdk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gcxcgoatt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/grksdyuor.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gxesfjypq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gnykcqjdz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gnutrgnlo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gwjbaxmzh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gbhvgfmgi.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/grpuxgckn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gijlpztbg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gzmuagsno.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gkhhefojh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/giiwdbqds.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gdiwlxgfb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/ghyglyaql.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/glqtpzrow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gnnoctvrk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gjsocforq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/geqdpteia.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/ghejncfhz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gbjeagnin.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gkegmofip.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gbadkwjdq.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gvqbiozwg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gscvfzvau.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gccbauqaa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gxpkgyxlo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gzmmrxdpa.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gwbqugtza.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gsuueldby.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gkufwjyus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gzgyqhifa.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gacqjsykt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gomxezoha.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gngfcnkya.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gjtygafrn.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gcoqijzet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gdofreckp.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/givtaynfx.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gxpihleqc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gvdngqhtl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gaspidfsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glxudxshz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/goagqfoow.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gzbobzxrk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gcemdbvgw.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gerpxcybt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guqvydqzf.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gmritaptz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdovspqew.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ggxqbmalm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gsvetzrtd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdgqzouig.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gqyhzjikp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gorillihh.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/grrbiupmo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gjhgzexgs.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gxfdccvhn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/ghhowkswx.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gsaecpevd.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/ggzekahjw.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/guuofvecj.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gnrutdghz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gurqbpziu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gzvkxfepl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gwjiyjwfg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxacioqzl.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gbucrkouw.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gxqiyathh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gawmhurkk.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gsykkmkaq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gwrcimzqh.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gfdyvagbk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gxnudpeep.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gvzvxoujo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gdinckium.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gyrjeltaa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwatjiwsq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gtrewfpid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gkviocbpd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/glmgjowdv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gorvmalqs.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjtwcibrk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfglmgoiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gtfnydpna.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gcngarmbi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gexnwqfhx.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gsehgcpvb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gvvssblrv.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gciolinqg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gsbzyjocn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gamtkqxbu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gveuntzgz.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gshqcwegf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdsrhfzmj.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gpknoczim.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvvsenjvl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gfnysumjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcdefhi.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gqrlpfzps.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqulihclu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/guggsdvts.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggyhglfqj.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gnigyicfr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gbknrmhmn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gkqqeiazw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gcsijcgxb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gtyhpbtuv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gpmyrdfqk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gjhbknumy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gdlwriwdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gerfiiefy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/glznsevyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gssitsfro.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gkmvnyhgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gfpaoefoq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvdpwiidi.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gahxfwdmu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdmjiglmg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gqrnsxesn.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/glxmwaghl.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gnuztlooc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/giipxznjz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gldjswbpf.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gokoxstvv.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gmnfulrco.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gxbptzvor.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gfivhacpq.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gpwmqmvmb.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ggpywslwy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfyketsgb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ggsvlqedo.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gfwbhvsuu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/grdcxtmtr.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gnkqqlgrk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/ggpzpatlq.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gelmnwryy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmdevaczp.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaqcvetmw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gqterlefs.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gwvrcjbkg.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/ghurrzndb.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gggxlrdsm.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gfdrdmajb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/giwhmocpp.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gcwnbakry.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gvjqjrnak.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gszgluibl.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/giumqbjhg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/ggzdioopg.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/glimmxtnv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/glseceojn.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grvzgqsck.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/grxszdcsz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmcjhnjvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grqmilypm.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gcxuczkyu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/grscsdqzl.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gubqprigi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gpldjhyxk.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gelejhiqw.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/guvjdkery.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gwjfaabka.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gnkojktzf.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfmepznsj.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gvsoeizem.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/ggwlkeepo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gmyrmaylr.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gtnxpslze.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gskbcnptq.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gadmgipbq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/govetcgit.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/grafapsvm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gnnvqzyve.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/grqqlydor.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gclcumhmv.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gyygmyquh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gnpedagdu.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gzwytlwry.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/ghajvfdqs.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gxypivwht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gcehjtkzo.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gsartbwjk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gxsvjpqsj.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gzghyonry.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gorbjbyud.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gfpfzvlrk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gejqzdbrn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gwqlgdlnq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/grmfimtuj.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gohchsrzs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gemwrmuon.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/girdmhyne.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gzuanpmnc.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gfieshkls.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/giblbavex.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/ghddjopyi.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gefnubtsd.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gmlzcykiw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/giiwicoig.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gmorzshqc.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gbrwbvtze.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gdkwjgkaa.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gauigouyl.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbvhxxhqb.sHtML


<!-- 参考信息 -->