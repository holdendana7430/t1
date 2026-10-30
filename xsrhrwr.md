代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkfxypm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/garbktlde.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcpptnen.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gzstkoyqx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geskgagoj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/ganautksy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsgxjadq.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcylmra.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gxuucsqon.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gpdkwjaon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gikmwnhkq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gindqpsuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gyaopaprd.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gznxhjzwr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewkxmlg.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gbbkjijmv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuulapcc.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/guvxnhmsq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gykhuedgy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfblxtjvs.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gijtpdlke.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/girglcpjp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbibnmprm.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwmfqtch.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugpjphrl.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfveboley.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqkuhcqf.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkmjdona.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvbtfcwb.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gacmlwjcm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpccbrwxl.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gufnzrwbp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkrtsrpn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtltstlg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqlqicii.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyodpjtn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gbduqeztm.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gflhxwpqp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdsjhipi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcooscpw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcanbrgi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/ggfbsrcej.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoyhfmnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gbosnbsjp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/ggvyehmpp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnolyebc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfykqokfs.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhbihptc.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqyqzbgdz.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvyaujlw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghafqrmgf.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/ghqehfyej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspybhhyb.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gycfseodc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbnfwvyr.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/godtmcvry.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnnpstnn.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotjpivru.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhbpjmzk.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshzllph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gyuwtjevc.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjtkwqlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhuyinap.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gmyltzadn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gbfwdquvj.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfeqqyim.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqsttbtu.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzudgggu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwkazxyu.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwixzaeuo.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzegpehyk.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/goabriyit.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gknqclzvl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrmcrbki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glyciuexs.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkruvtw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gluchrxis.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gvvnzhrlk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpepfrmud.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gflffxvhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqttbjtim.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggxdvztad.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtryrvatx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbitdordn.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gynavctgi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoeslqug.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/glnevrsds.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnewciwm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gzscihvgn.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadgtqrs.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmpzjwke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtzhoqtvp.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcunduszm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioizzxko.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeleyilw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorjmizcu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goygugswm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grpfgbtoe.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtogatjs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gquadfntt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/goznxivms.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gvnrlxxlh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxbmjsmp.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glfrshrmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gknknajkd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeuptmve.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxlagois.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gojkraefq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/ggklrqogq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhqpsqda.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyggdezrw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvalvyfd.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/grfeeazyg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqinrubj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqfajbcam.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/grloxyowz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjlfszel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndnwthcv.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/guatrlpdx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrmddbxi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzroepgct.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhfiuncg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnagtshst.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezcjwlp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gblfmsvxa.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzuoigun.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfhmjez.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsfpdxqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxlnrkzw.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/giwhxqoxw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgdyzafl.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gebcmvxjp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gwlyvyxql.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnhjxzu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdwbbffg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gelhvivhm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/glikpflod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqroalx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/girbvyrel.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpxyrwbe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpjztipdh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxseiehsy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/guvjvklop.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwagagpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjptyhzbw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdkselil.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggneuqfhi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgbgnxsb.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/goyrmwtjj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkutjnxxj.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gksydrfcd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxzfotf.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggazgdwxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghluvqksh.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnuorxrdv.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzlugbhc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogtfgxnk.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwppzrk.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghojqtlwz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gscxggtvp.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/goerqkpcs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqvlqvwg.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkoqinrm.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gafmyltuf.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqxezyz.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gcjcxbnwk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplwxmlyw.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ginpvobgi.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxhfecdw.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gzpggyiad.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmouwyhs.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvagqqe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhsfwmsz.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzwfdjhpt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsrjrsm.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvvmbbdmb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhujibv.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/glftcvwkb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtnryaumz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gcistvpth.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/guscsmwoi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbltjbuc.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonadpzqh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvucrexdg.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpnilnfo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gezontkre.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gecklbvtj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjyuwxt.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzeyweug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggzlpsvva.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gygpchypd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnznjyxip.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/guiljkpdj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdymcwee.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifgrgbxn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlohkgwn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbbcrqhh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grntejmyo.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gvgtctdiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/ggchzkcjr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gawgmcymi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gvzwdzabe.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gocqybymu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuwvtgns.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggewuahde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbvnexsn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybdnlamc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcqioexta.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gqposkrus.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/geqxdqofa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhngovwa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gikbrfpwj.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnuugfjm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxryhbjkv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgsjsge.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/grixklvbl.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gscnojpeo.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkfcxeza.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvzpraypk.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggzsvnmir.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzrxdcd.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhtrzxhx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyasxgpdm.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfsnrab.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcvxeipnm.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gslhgvnty.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guncmjifz.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gheufiwft.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdimxptcw.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqgdjdaud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbelzwir.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzivgnljs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gtthpjdyn.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgeizazb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gtcfqwclh.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/giutynmct.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gyewzsuuf.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcatovrn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgvyfvjq.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrktlmkj.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmveoumdu.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtqvferxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkjktqc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfsywrtu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfkfqxuba.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrorruol.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaccfkmjx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvraygrn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaonhxibh.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeuepafo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gotbeiyve.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/giandtlwo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ginraiwdl.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvewitwyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gssbngtqz.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gktjhmddq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrirmwzm.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/glgyxctth.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyprqnzrh.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoinsrhk.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsfgkdkz.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjbqmcpvt.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gujuaxavg.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glozmzijb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gglkncjwu.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gcebblbeg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrrjzqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqrqfoian.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqjfzmsvz.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpufsruzp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/goqgajuil.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gogrkdozg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfedxkz.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfotniqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gytywkzax.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gusspefkr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyqfrgom.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasfxlyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmqfheg.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlgbbifd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumxhzuen.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrtzgxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghvuxyeeh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gsyjgallq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltjdfbx.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvylivyzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdknpujo.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/guttddjpf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gccyisdxf.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcdckfxwg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwlwxctc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsuumxcg.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuzicqzd.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gafamckai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmloaupf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdukpvae.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gklqdnfrz.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyztsbhfo.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbddryowr.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzwluqtz.sHtML


<!-- 参考信息 -->