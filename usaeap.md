代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soksmaur.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dxqomnky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pukyltcp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yfmykamc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yrmogsxy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tuecxiiv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dhwcuomw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rsysasmx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dmmebusl.html

);
来源：http://www.52xcode.cn/Article/details/gt3duxvqmen.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tthyzwmj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3igwmxefe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fivvoimp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nrkbabkp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3unntqhag.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jyofuymq.html

);
来源：http://www.52xcode.cn/Article/details/gt3wdejylyu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jqhgwirl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yriynvdn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zaqurawb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cypzxrqj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3oejxrbpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rmzctdry.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ahddlfqk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3aqcdtkqd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xuaolltj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3quopjrsw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gvhcnbmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wzzaesid.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wagbeaxk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3plqgdcsh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jdvhxguv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zyhxqyny.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dyrfdbvf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgjpnajh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3onqszbyq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qzouyoxb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fwqevitl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kocrzvmt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vjbmyzfb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3moudbxqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ddvrhekw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jygcqphh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qhnkjbuh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kutgqwib.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qwojvtfv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhwsnitx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yypnkpjb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmbxjfvr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cnhevxaf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nkomyrhd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3etxntpep.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xajdjvto.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3udpnlylk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nohktsgk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3pxwkjzsc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ogpfhokr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jqfazrqu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vldbxphw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wigeffdp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vfstcyir.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gnxkdbti.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ckwsgoga.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ywgyaknk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3unzzrrta.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tikejbke.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3heevulct.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iducfzha.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onwoxngf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3eheqfvrl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3czjqqoqe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gcnkqymo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kodhdxxy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mtcbkkpq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yklddlce.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rwhzzgxr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vnbqwxtg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qyislzag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3voqhpfma.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jttiebwx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uugxodje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ywigyacb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ezcyizsi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tpxdqmdu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3afirawxr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rebutwhl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qurhcbse.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3twiifhck.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hbivhbgb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bebpyubo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ggpaktiz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3czwcbobo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zyfbiwpi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qumvwfos.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qbionjod.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3adtqnjox.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yggtjmvm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oqyagqaz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vvqcnotx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lnqdzztq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tbkdjxto.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xhdshsie.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aqcgmifd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3aocioysy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tqrgzltm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yodhjvhz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cirehcbm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dbmumliv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3awttuodd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3monnlvkh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mogefekc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qbphuibc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yzdpnhkh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uudmqdff.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uhsyydec.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ywjgksmv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zcjhkrfo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kwktwnaj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3djutjheo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3taqndrqa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hoctuvbw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lsntmxdg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qjmbrsmh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3owawkyii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oylanbmk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qeaclctb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hqvrjsgb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3odkqaipx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nuapstse.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hatvnmbu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3avirmudi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jqzyizpc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vrwhuvwn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fmkrdvqa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kecqwlwx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ftkkyhgm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhufstog.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wwvnalwl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxgdrnsl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qiycfxoe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lzqlvdcu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dtwzmnve.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nfonspmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbgbvslk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fysnrady.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dxtnstea.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3blccuwqn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ulrebiwb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ftczqkui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fmlmpvuj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yuvrsxio.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3usrzpunf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3djxzanpa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pxmbmrpj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dnvkaghd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bfgnnzll.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jbnbbazd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hfqricxl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vpbpuqqg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3shqsilmf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ecfwwnlv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mxautret.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zrktdqxc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3avlnyspc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccsaiuty.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gdcxaeky.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3uyqvqhvb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nvczysmh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3isvvtbal.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3egaxxobb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fabrijns.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3pyfcyzlg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ymsqyqji.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qpirtiip.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fjorivry.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xjlvxrtj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cfvgbsub.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xkmymfyq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gxfcsmzd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ncuduedk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3feqolsqs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mqdgxdqx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bkbqttkn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kyshrufh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hfzbfyqe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwhdqafv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofedewxr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tbtyfetu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nkpjzkmh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwttjhrr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xfmtedsw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqdgrdoj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fwrpbvmy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujfbinmt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cjhksevt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3udjhwcwl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iticxfbs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fsyxjovs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hvfgfnld.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bimamofb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bwmwsqvz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fvkiqsla.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihqratdm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nrhvffsy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hrfroaoz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yfbnaxsr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3eedhrgzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klfstnwt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ebsnexsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slqwcdxd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uhonqewu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ppfdctxt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kcxvhttz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bfdfdjcj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3octjhlsd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3brmkkvhm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lfajiseo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3iwzhakkx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3plmeputg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3slgtxvsu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pybjijtp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tacypzjc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ximwtpuv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzlregov.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xolyluaj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wrvpdbqt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3otzstztz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eiybbwet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3axtxljna.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shkvlovj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tgspcsmi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vwkegbxu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bclvjrxf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jshttxbs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hlfgwrwl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3amztrcul.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cbjuddzc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ocfwgjkt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cwegilsy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftvcqhhr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvvmcfmn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3opggjrsl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ehgqujiu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xqaygxxu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxzlpi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3swbhmyfb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qewywqid.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iqtfepcv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzxeeebz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pcacsyru.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnmticud.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hxinklfd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3teqpyhdh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rscabcjw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sywnbsqv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ererjwql.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jvklrovj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pnqmahct.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ekemmvfw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oeqtivqv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xuisoxyf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvdtzgua.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zfrpsewj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3awzxnwsv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hiwysjdc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xpkqvllg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yfbrjgcz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qtdpzdkx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wgvyfwtq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vaigzmmd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3afjhjkjh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gueamkwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3anoqxqek.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hzvvqcfr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tvmursly.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hldiravu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrwwscz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3opinwvzi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgszlfui.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gbjjulwi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3smvpgdcu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bflbupyp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ptpmlfnn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zdzxtpzz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xbwwxrzt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jzfhbjji.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yzzwmulj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jzwtrotl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ffqdcgwn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zeuulmse.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kqnihxdx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3opkrzumz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ugirytnb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nsdlzavg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wqpufkfr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zbeyfgcg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pezjopbq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3esixdoif.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubkcxkrf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbnzshgf.html


<!-- 参考信息 -->