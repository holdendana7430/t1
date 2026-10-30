代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gewiicejp.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/glxwauwnp.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gbesaauji.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gixqltsfx.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gipnttwao.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gxzxktfgi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gbdezldwu.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gxkmaoagu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gyuframka.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/globjmntu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gexggaevk.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gihqkqlpy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gexpvpljk.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gjdpmlwog.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/grtyhzsko.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gwlpqewxu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/glbthvgrx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gdupzshvy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gyhirnmbs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gkoiddcva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grvsgbvxu.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gkibnlpdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gpyfxaljk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/ggsqyrdyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gqkavkfid.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gzdykglxh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gtpojnvcm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gfledgulw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gpefexzhk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gqxohuubh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gljzfpvva.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ghkwzsfko.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gesrnrriq.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gqcvufben.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxvhjeeph.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/guiteavxp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gewdldpde.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gdzcptjzv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gzdoobtvl.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/goesnqofd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gvqffyhhb.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gwpalvnxq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gadtyyoyf.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gulpgrufv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gjzzejexd.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gurwlzsma.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/grnfvkkwv.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gnsmjursd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gaibqfseg.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gijzhlktn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gszmxigrk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/glloujfdm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/garvhlfnd.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gulyyzkip.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gthmzvnen.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gsfldeoyf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/grdlzabsl.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gupvklzpt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzwaabdnq.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/ggbitbkox.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqolnsxvz.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gpztccvty.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gdyakkquv.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gzkawvbfg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gfkdqphmd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gxquyzxhr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gddfwwepq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gdgdfowsi.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/ggfyjipbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gftxbrlde.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gpetbxcph.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gukkdgaci.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfolzehxc.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gdkaaphug.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/glvzjykuz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gncvqlwch.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ghhzelukv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gpnwyceuf.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gezqtkhby.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gkoioutkz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gjcitbwxc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gtwocbsmz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gbetosahb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gylmylgeu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gxioibafy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gzpnhsoum.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/geguehpuo.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/glqzuoncs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gkqhcedlv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gcyucmffa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gojodybvx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gtynzwyil.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gnamxqhng.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gcgkwwmya.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gwfwqpbjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/guoehusxc.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gkrpibdmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gqnfwyxbi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gkfwffret.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gauqyfqvp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gcqchwnuh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gkjyilins.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gufkgxaxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gaiurtbug.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzzkrljqd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gvczmzszo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gzvhrbmlb.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gwbluaaof.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmmfpbysp.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gairswica.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gokqysjnb.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gccmtceik.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gsvacdcto.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gnltfpnmo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzaerwpkm.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gkccdupcu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gzwytaneu.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gidhablce.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gcobecnkj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gdhqzcpdf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwxudohrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gycsrxxuz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gigtbfvlv.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gsgbfuccu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggikjlgrb.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gbxxoaowz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjdcymoyh.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/giumwvsdm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gigvzammf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/genjiavfp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gneqqyjtt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gycnbpubt.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gpxjhzgda.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxtzszttp.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gsuqfamhm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gdygnmnlv.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/ggxspwhbi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gjabgpheu.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gkcblmatd.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gotjnehqh.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gubwpyfff.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gtgqzkbbj.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gakyjzxss.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/giahwkvnm.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gbsbwoccq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gowrsmluj.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/glgzlqyug.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gyqdpflmt.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/ganidibvq.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gpjlyfbrp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/guqxulvgp.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gtofddjfz.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gupskmrvq.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gjibjqdmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gkjwyuozo.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gfqwddydl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdxqmahxi.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gyllbsgop.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gzfothweg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gjxvdgyhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/ggogjbdyr.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfmlzkqza.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqjscfmgw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gcnlwvipt.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gmfvhmfqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gopvqvakq.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gutxhgwfs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gbqbdkrgc.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gjisgchkb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gmuqgsyyk.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gfrmfuaha.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gjgaadmam.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gbykkxdac.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnanxdjrt.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gbynhyevl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gavkkurgq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/guuhccyet.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtqbuuaog.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gcydxxfeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcwdrtkly.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/goptxnxey.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/greoxetuf.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gkpmfezgb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gqgcbaqym.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gsznqizsb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gvwizifoq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gjwnuoaun.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gabhzlncv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gclscmuii.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gpksihxqs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gihwhzifk.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gtmchylwz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gkeqiokfb.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gdlxxsaew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gnqwxvfga.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxlcdhcrv.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gbotcnupa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gitjhrvkq.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gylglltsz.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gavijteiq.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gdzeqglez.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gwdwggpgd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnjgrfbyn.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gvkvhzjar.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gnmzwohbj.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/ggbgoznnr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gvszookco.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/geynfsngd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gbjshwgjh.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/ghuobzhyk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gaoztjbzr.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gtdgmxhta.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gnjzuudrs.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gjnqvupul.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gdzbxhdvg.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gdtuktmkz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/glkvahfgk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gkcgjnlpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/giimhxxba.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gctyjycnt.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gnbhemndj.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/guplloqxn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/glhdktoul.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/giurekmli.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/geefzeoaw.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/ggnzmkcxq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gfueksmsh.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gyeszrcti.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gxkqxgild.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gmzqzllru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gaktjddsx.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gdwisgqzg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gywhwdwag.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gcjeudcdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ggtnronsi.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gllladxsy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gdqwgcukj.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gtwbdfhkb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/guacawhwe.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gljtqcrgq.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/glozltcks.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gfiobfwma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gmlhziacf.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/ggxzpoqud.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gzsdkdstd.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/geaouirnx.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gmagbgyqn.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gaamgzsqt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gfvcfjgot.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gkszbmeey.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ggaxkunuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gyduiaylb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gtersoeza.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/glkzpulku.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvpmcqw.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gvntjxkbn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gvoigrwfz.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gyqpsqkpi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/goqoxhzmp.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gjsueblct.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gantvbvci.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/guepmgfcf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gtixenegs.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gewvpbxqs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gdniwverr.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gfvitzlrz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gxfxaivfs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gmrajhdvv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gfeguaosd.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gogkfhdsg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gthjolxif.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/guootpvul.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gitnfkeeo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gxxpmiznf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gqxkvgcfa.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gqcrhmuvr.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/goacjcwwv.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gsihmjnnk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gizybpnsz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gvsckuxrh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gxilshqgi.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ggdymcuvn.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/grswohtpr.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gqflwuvwm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gtubuammj.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gallmfgnf.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gwbcaqlsy.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ghypkfrkq.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/glqyfagmb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/geabklvfe.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gephecoaf.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmlpkmfod.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/godmqdlnj.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gvbyqkqgm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gvxvupsjs.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/giqaswwmy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghsdkbnal.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gldzaeorf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gyaohdeeg.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gkqfhdfwd.sHtML


<!-- 参考信息 -->