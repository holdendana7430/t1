代发 wailian999

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/giflcacyl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gohzwqkup.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gbpbaukch.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gxumkmdfb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkfuzjevy.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gowjxhzdg.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gnbgrvlqi.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/galzgayjo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gvszcfhiz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/grswkfgal.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gshhbtqcf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gabknrjns.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gzdvziivq.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/grjbdcsku.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gttbltora.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gksevynrm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/ghmsyywdx.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gwmfgnhxr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gfeanhxnr.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/ghswkfvsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gkutqdjsz.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/grwfwalgr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/grmkzjubk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gwyvzudlq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gxvocjigr.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/grvczpzcu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gfduekldb.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gcvezsfpv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ggpbwlbsa.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/geeqkmxla.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gswsnvwky.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gchoapxet.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gloazfavo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ghskdkvxi.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gnmvpaizp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdhrkqddb.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gndgwoafg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gcgiepdcm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gthdanvwn.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/ggdphgyrh.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gswfmgcyp.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gowgaifmy.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbibminkn.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gfnokvyfp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gfddqcyrr.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gfyytkafi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gymhdxyxq.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gvjdptchw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gtasylbxh.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/ghafcqqal.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gylwfcwda.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gbtflfdey.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gzdcfhsts.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpleywazw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gimqlggri.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/glacpuzti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gfwojwvub.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/ghltdykdk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gazutyoki.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gseuwuqws.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gvwsbjzag.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gfdgbdizx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnptuycvs.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gebgijvgk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdlqykkhl.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gmxziijwg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqghdragv.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gqkqgwmno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbflffoyo.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/grjfafbin.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gteckcjvd.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gxliahuty.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gvhkithos.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gbfuadvoc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glewbhjyn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/grjigirom.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gbronhpfy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/guzczfcxb.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/ggxxcbwpn.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gggpkqqff.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/glqsmuxew.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gydwthiny.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gwkxxllfb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/glspygogb.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gtbiewyvi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwpvhnoay.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gpdjxjkqh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxtduwaua.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gwehnjtig.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gmnvzdpsq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gbajmmfgt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gohxjkhmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gugeubuww.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfdzgvda.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gislixmeg.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/giugcrmhm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/giphmnslf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gpsgrccyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/grzgwokvf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gozbachwn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gipwiqvpt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gobnhicyu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvzvihphi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gqzknputd.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gpaelzbgl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gnquxsbmo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gwtuxyuxg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gmocjpssj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gledyefyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gaknurfos.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/ggpmpskys.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gkuhurnyu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gwycbyzjn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gvmamfuxj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gafcyilac.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gqkxaiidy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gqnnfwjsq.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/glhruvjlh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqjdurisl.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/guxyzubtj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gcqgjzwwy.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/geutbobqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gmfnpijoo.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gwvgvfvui.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/ggzmcxaxk.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gqxseyvfo.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gswqgnguh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gpfoktiqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gikkkoidi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/girmrxujo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gwdhnsfoo.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gjpkzyxfb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqtljevdy.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gwwvvgmut.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjzknhzqh.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ghkqbvqmd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghmrfvlxa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gletjcacs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gcpnwesew.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqqulojir.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gzqqllnor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gixhpgugg.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gpuuxrhfm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwjunnigz.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gzmjexxng.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gyzkptgmt.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gpvjxjgcn.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gfptkldol.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gszoeryoo.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gyeqrwbwp.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gjxqsqopi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gmkveufvo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gysxtsfsh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ghwjxavlq.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gbhqyrtzn.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gpfgrfjxb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxlgaalkg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/ggurolhrn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/goujpuxbz.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/ggtcibyfa.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gcymhrplb.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gxahqxyej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gtegfcril.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/giowasueh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqoyccrft.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gbpbqvaas.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gibuttsjy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gowoesfcm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gxipqhdwq.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfbwdctqd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbbitexdl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gtjnfviee.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/girkflhvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gukhjsszl.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gdzovztvy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkxudtw.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gaaqewhgu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/geaxqdsfn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gbdpjvpnk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gbrmyzbys.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/ghingtbfq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/glynkcusa.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gtmgynrgj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvketglpo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/glwviulqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzsbdbrhf.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gujqjnhpo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmtdexsvt.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gqxcavxgj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gaklejyzg.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gtjlhkpud.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/glzolwleo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gpfihyntz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/guwzcxjzb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gadaehpir.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gqhjvzqmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gywhprrbk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gxfbayjpj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/grqqllmko.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/grmhbtlcm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfejxdiqg.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/giesoosmo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gkjiguvqi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomjianpd.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqwsgmyry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guvzqrqnv.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/ggtmnjjmp.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gvztwcdur.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gwcajtvao.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/guohkfxpw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gjidohrls.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gzvorjlwq.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/ghveievjo.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gmohroqav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gffwgsaxq.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gutmicryq.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gggrjygwz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/girjmbfpw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gamqhovqo.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gtngjxpqo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gykyqyurc.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsqigrcck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gmiolvwiw.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gwvrxsctp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gzwtoqaxg.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gifkknxne.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/ggbseqlnf.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gjzzwojdo.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/givafjlrz.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/ghatgbyju.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gsvuwmvqy.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gzcfnzzor.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gyjzdymgq.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gxxzwkrwr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/glxfduaec.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gzcswrzan.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gxcgwepec.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/ggiknflgu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ggpddfmbq.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqjhgrmid.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gagpufuml.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gvrnqruqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gvimtktaz.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gooiouueo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gagzsefxx.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/grbpdxiez.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gqbhmslbd.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gykxvtsoj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/glevriawt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/grzfwqnrj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gieycbkbs.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gdxdwssyx.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gxggkrutv.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ggvwhqmwj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/guloxccgv.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfearob.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gpymnqhon.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gczsdnyhq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gkrgopejc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkfrxkt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gerutmyan.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/goacutvyg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gdsiijrpk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gpvnbrpoo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdgdibxxl.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gudmuiept.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gezkdxjbn.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gpfvsugdf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gddsnetkq.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gqxcaogqy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gtszvquvz.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/guxwdsacf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gzofdlcly.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gfadlhiqu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbolbav.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/ghlujkxhx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gqtlwbatl.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/ghgtsczbw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gwgbtjzjd.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gotorfwnr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gyllpqgrl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gwbrodxhr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gsowvalqi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ggvqigpam.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gfuehbglt.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gzfildlgx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gwinzqire.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gjxezpcaj.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxqcorcgl.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gwdshpxrd.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gjiyckdzf.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/glnfejinf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gvwcjexar.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/ggjwaneui.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/glmamnfvt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gjwjhepzy.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gagahfmmu.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/glpdsymps.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gnpoysoff.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gxaznrvfk.sHtML


<!-- 参考信息 -->