代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gcesfcegs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glqbvwrhn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gwklipbjd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqfibrrq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaxalqmy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflxpfinn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gzelrtzcq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbrtmnms.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytakwfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gzdkytlcq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtmeawisk.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gkzekpngz.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwvkggou.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gapwgvcfg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbusorvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtencsiq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gfudibtdd.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxvtvrr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahdigql.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/glebroxam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrknjdkb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhzssnew.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtthbxsoy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvqbulif.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gazxneguj.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/ggzpefezt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnkngkmhl.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsiuwcsq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkqyzowz.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gjhzzarvr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhpheqn.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/glggcyhmd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrkgslph.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gmpfdmuyg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gukicjifc.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjubhzz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gglzwtelr.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gomlzvnce.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnicxpsnj.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvboukk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuquxygu.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbumkfr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gtoqfndcz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gvgbclzoe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyeugsqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gvacwyooc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gxadrnlcf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gneqglbxq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwfincbq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/govwbldvy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gdclmbdyw.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxiwblr.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymlnvek.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxshkzuma.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guwqzmsvp.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/guxwimzfo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guysvlkat.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbzguymuf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqyaunab.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzadcptrp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbwzlnhc.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfcedrvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiiulbxl.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzykqxxqv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkszlyxs.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrjnlopd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxylhzlk.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/goidxzpwm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydwpflk.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxuvsyqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkauehddf.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnkhnhr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdtjjhd.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzaqechn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdoznoom.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpiiqkt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggzyucfpa.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyshsekr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszkzryfo.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkquhguu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhxiffxl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohdafbp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmonwlcsj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfjhcqtvj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiuzohgx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzohokzmk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gwpeoovrc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gxbiqtciw.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhpakrcq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppgptwgg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibggjstt.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gbccrtpqb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwedkzip.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhpxftgs.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhfzrtpe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqtfhcmam.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxznveyz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gedqexsfe.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllqkibn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoynpceu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gnknsfago.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrqclxwz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gglhwziqk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gfljbqdot.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/grwlqdvgj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjpmlefo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucshxpxa.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gndoibhph.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gwqsctrbu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnvjxvlw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgseqpdq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gxefxcwko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gfgcwpbjb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkaldfih.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gftyvanuf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gtstbhsmw.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosytulqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gznquwjus.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gswpkivts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwpfqubx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspedvfmy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibmskcba.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzthcslt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/giopkeuct.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiatzcto.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzidacpkg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guzwdonnb.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gdnkrzvxn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqhltlzs.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gytdjamxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gufmfamfa.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gbapflsvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhgysqnv.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/geflxfzuo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhawnhse.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gfbntwizq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/ggengdpqm.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gneyaffse.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gqoywptcb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuqyfosq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrwetbfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gpeuhnrca.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijazqgc.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/glnfuaqkr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjnomymq.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzmhqud.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/geadsogbf.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsogkjvgb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxcvojbn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydxnxxaj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gukyfqusj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnzwzgfa.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gerhtxdlq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gezeolcys.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydhqivbm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gyagvzsrq.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/grypgxdzf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gsypbmnld.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gniceynky.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbpwkkfg.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxcjsbyy.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmyvwhri.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpnslgcce.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnfjcryc.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gilezzwkc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbedcwnla.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gxoitrkjl.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgrwzqek.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumpuiif.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ggoxvirdd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsqhpdxe.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzaiyhks.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gslymoosw.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkipwtbe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gazliccxw.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnjysbeq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmhnhxan.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gugwhdbzg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/genmvxllg.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gbnojxqqx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlabmfpv.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwjpnbpgf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpjybhtkc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gygnrcatr.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grmimsytc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjzdqjr.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzhrzidl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gwimvscib.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/galnkqmpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gprtwmsax.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyiowqqw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gxskflzxw.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzohcwnt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gufssmjwg.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnpexhakj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gahwktrmp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxjsxju.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbuyebcc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneeviqvo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswghtfk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjredauo.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqajiwstq.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gsficxmux.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/glgtwtfad.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxqkyljd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/govuisazy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtfybyit.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxpudchu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/guorbxgkf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gryneodjj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguaupxgr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcltkpz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gcblgpkic.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbflchhni.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjvhjodb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhmqhnjo.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfqbtyto.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gukqxyclo.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gajwzknsb.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gifnjbxgo.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlzpvvrk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiczaird.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gapztsuuq.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzypdpfu.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazffjslt.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgljgpzi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbenpsyw.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmachcvgl.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxxiigyf.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/geriynufu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/givxdqkyv.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkaryaoob.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhsygytz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwwokmfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjcmutwz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsisbpmdt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelmrihxw.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gigshcupj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcshqubda.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gmamlycrh.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzzmegqfl.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxzdxocjp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctknzetn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybxaxvds.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbrgopg.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwcfxuedv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfbxaytgr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjutcsnz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gytkloarf.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ghgukfmij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gshriuubr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpkskaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glcnnwlld.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqayiwe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghirjgtka.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaemauvc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeluotdd.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gsaowzvxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giwudmhtl.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbftnbar.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqjwptwi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmvybzu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtarwxidq.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtdtptkig.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjklnqrgt.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaueadho.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gczrqzvgo.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwyszxcqg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnyytfn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdugwyue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gszuvbcpd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/grhspmafh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhdnlxdf.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gccxacfdh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gevxtkeam.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gwmjfcyko.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdvmmbhu.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gagpbedrg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqtwjvw.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyvcskiu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtprrcgvg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqkpzkzu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjusaps.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeogmcac.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabjtzbi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghipdvzck.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiziypjl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/govedsmkp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuvaprhh.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvobldrq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gelbsnoay.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuianxtr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqezjbwi.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpjpawwmn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gikrdpuzp.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfkbcmia.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrghxvee.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzpbvaowj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gphbqobfx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgbapjs.sHtML


<!-- 参考信息 -->