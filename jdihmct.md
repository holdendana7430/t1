代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gphravnkq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gntqtelnm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gyrjwxtjv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxvhfenm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gpiuifnbl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gxlbpbhkg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gxrwelhol.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxofppcui.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gthvlpouk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjqblekj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghligrxvs.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gmsgucpai.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfntgelv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/grivqsfpu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gacappmlp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzgvgaju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/glsvncgim.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtsjcteq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrrwplh.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gforrjkku.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gznzloefk.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdnmeio.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktporchb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gippvvmdr.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gkvbzgnvf.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzboyqij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcvnxutv.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdatcdueb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gqfyvbfmk.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gimjovpbw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/guyqwkxsc.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gotuckhmn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqoeudoo.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/guoqupebg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxxglza.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/ghnvequgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpcpejc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ggltrfeul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbciqnsk.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacqqxwh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gbtspfdzc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvlofnz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/guegzfohx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmipkbnr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gchqaskyo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfadppcf.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gznraaruq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmgvlew.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzjbkre.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/guqdkwlfk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshgklnpi.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/geblxlbvt.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwlyphae.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/guuhsdqgx.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkedumnl.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/glyfmtagw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gztnphwur.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhedsgjk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvvhanqd.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqtpnnj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/glyzvskkm.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/glqrgzkbo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqnmynlt.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqptgwzpn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gtokmymxs.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbcxyrdv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnegjcme.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcrqdnja.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkuswpts.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghimyiuxd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxzzfogv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkvivive.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/grksoqaug.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtagjhrdr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohkflglu.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwofopajh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqkqjjxd.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gqilzymkv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdoyscxx.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gjpfvqsbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeokvqha.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblzwwtbv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsewyoqwi.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaktkphr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggcbrgwkl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/geeqabuiw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gitvkwnaf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknldtzw.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gavwcgrpw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxzctkn.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsozqoony.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunrgasvg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gjchpbrep.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsccpozbv.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbyqjpjcy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmxehoro.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrkudcd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvferlnk.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gumbmvjgl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqilccxi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxqgind.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqzmjzoyl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/geupnzuqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzlfckbw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gmzytbsqi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/guukosoci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzraomfna.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gkxzsdxsc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gukyiaphm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/glbflotou.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gknocidwp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/grxppgmpj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gbnbubwps.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzxlwfkl.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvrdtrng.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvaastsh.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqjxpic.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfaxzswb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdlfhmzwf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnwixlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/glcxmpvgf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhdncbw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkuyajvv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gtmuuqieu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gshoehlnq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/grohzuafs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gbtqueudu.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/ginpudspk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbpvpuwf.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gnzokfnmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gehcciwve.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gyoeopfgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesdecshl.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmheqppzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgkokcor.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnfsxdks.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/glgytliix.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvebsdimg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpajuwz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaflvuqt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gmriwhzkk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gdfyaaqyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gyysyliyi.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggyplfju.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geisorlxx.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmrcwpn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gporlmvjf.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gtehvhjcr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkcxpvvr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/golgesipg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gtupznzav.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmbcegp.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/grmnkjrno.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyktqwvn.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gdkkvxmic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gdroynpos.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkggloqjc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrmqlckk.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmfkwfccu.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcnisbuv.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcaoejwo.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtqrtgsh.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcjaktjdp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltnffsga.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gqlznqhbb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyhcflwj.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gmrijxvvx.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gufkapkkq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbdquxu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjkvhtyx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/ghuadjhyy.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gxguqtmes.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gagmlmudv.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gbhekshye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gbxwfztsl.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjyvytic.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvupcpqhc.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrlvszcx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghcxnzmjq.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gcpjuwjay.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gjjpvblbj.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gsdyafdgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbbvlflv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbjvlrug.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfrcyjvr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqzdvemi.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkanzsij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gpurlkxvl.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbhimahj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gwtisbsjy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grxtpgtmb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gszkiehcg.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtbbgmpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqehonmu.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwvggzxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdxlyhwas.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghlrtrjsm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjhvxgm.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghulslpsj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzblbsfvx.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gxjagnfjk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glcastjvn.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gwopedgwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gdvmhsygu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gqawodvqe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsbfvzhk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvtmrghwy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvczplzg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gppbbwliy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvakvsi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgmdjjye.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxmxmova.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmuebthfy.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gunqmhkqr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gakkawkzw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gteffuuac.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gxfgeafan.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnlntlqr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcnrlvmu.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gacuzlcsq.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdiqusxo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gbmgehfvs.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbbdiymy.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxexipsou.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxfuutxv.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcklrxusx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgdcqxna.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ganyeuxsf.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grztmmyry.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gycixzdap.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpydvfxc.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdrseuwi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpiywvuzn.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlpqogmg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/glyfjlplo.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlirjys.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjumjfdfz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyknmkqdw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuismyai.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/giapxnqyk.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/guxgrajfb.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpawakaum.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjlzmkso.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gmjduvspk.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxhzvrqj.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqtvoyrlk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqwdelplg.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmkdjwrd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrvfjogi.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpesficn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhkexrcs.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzekixvmb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grebragwu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxtqzrdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgifbkzd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxpitncy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqglboui.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gepnifrwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsbthmcjk.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gonzqzntj.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/goowjpcjr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gozmftakz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrvgrdeu.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqszswxa.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzcrsutd.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgiygopw.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbouuudo.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gczoxsiej.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gclmmogph.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxfkvhyhm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqiixvhn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvhkowo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsacqqaxk.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypfhkta.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmlkjpvu.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/guivnwoag.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgevwzyf.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtisnrwj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbzoauoo.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbeotys.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gemhphhpg.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxrrnnhfj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkvqxhu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvdhpci.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywvwausf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfufkvoa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmuvsrpin.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ghhpqpiim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmpuotbf.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkdpaleq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gueiohejg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gfczgfntv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsrtwyyh.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdtbwtlwk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gtzjzciql.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/glhjnkbrs.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnejzmccl.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/glllzhxko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjaliutqj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdjzdew.sHtML


<!-- 参考信息 -->