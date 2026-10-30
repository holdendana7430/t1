代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gvpktzwrt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gckkvduaw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/geiyeqzau.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gctiyfhaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/ghjsnwxjo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/guvwsalbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gjlsipiqi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gbmvbqnko.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gudqbrvse.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gylnhityi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gwhsraiqv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gfutmpeos.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gehrqayuu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gcxpchysd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glakjsvhy.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gbnftrytk.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gtuinsbzm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gfhnkbkdg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gwpxkfibp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gczxncgcr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/glcksgrhv.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gfvsbsygl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghzhuzwin.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gsgiwllki.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gvlsrphgg.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gxtgatxzv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/ghvzjccpt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxesgziy.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gnakqgohx.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/glclnsdga.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/grlplhvqo.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gkerqvach.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gcjjshrog.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/giiagciue.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gepswpzxz.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gjabbxgop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gqqbtfyko.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gsxxhrmwi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gyvhroejw.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/germxsntq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gbxexqgxr.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gnsbjscam.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ghasqenwo.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gjfpdjbam.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gddctpzua.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gpihhaolr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gayovimrx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gqsrysnal.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gvfpdqevk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gljnyxlgr.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gxlfnxbag.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gacmzdzmu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gjzforvki.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhwktht.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gmwrvhwha.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gqnmbgwrm.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtxjkcsrm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbzobokxg.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gwnhkvemx.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gwlmeuall.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/guyyerbly.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/genjuwtot.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gnftghemq.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gvofzmhko.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/giysiokax.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gypohgmtv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpkfubbku.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gtwmeccwa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gabzcattw.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gulufofwi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gjlvarrja.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gdefvstpy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gotqyzccv.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gcreqtcbh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmgyamxuh.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/ghjqexrdl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gvccabxam.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gbfyciflp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghuxguhfu.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/ggkzazeac.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbiruzpcv.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gkrxswffz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnhjjijdx.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gosewpglv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmxebbfkh.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gqblccmkz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ghfaeoxer.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gstmejhlq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gtmiagscg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gkrxqwrzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gzdkjbqex.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gzgeuqamy.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gjsqkmgfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gfmdffjfu.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gunwrfxft.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gmicwdbtp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gurndttjv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbkozojfb.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gbwigodha.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqykkvsji.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gsrjwofuj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfelkipzh.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gitklsswf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gcmgwkiix.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gdlytxrkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gptuuxudp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gftsbevps.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gtrgqzocx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gzmldbjsl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gyrqchxzo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gitqqoguc.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gcmtufblz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gybqaeuzw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gmkgvizyc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/guoigkrpc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfpqjeouc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/glmfvzbbx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gtmozomxy.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/grufpwukd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gcaqdzrlx.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gbwsikxwm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gqlrjktud.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gcdjhrtps.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gvzwliwsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gzslhkofy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlqyyqqx.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gamkwaenw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gdyslrywo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gzxsavcfh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/grqkeqdaz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/ggorzhunw.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gzzccyejr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gudbinlpe.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gmrodzrck.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gbmozizja.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/givrgkjor.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/geoahyqcv.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gxvqvdtkd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gkbzlzlop.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/ghlxyiitz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzkdaaqlw.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gadcnqmed.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/geufugjca.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gwnygvbjt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gmmehzkgr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ggorqphoh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gwsuxaoon.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/grbiygnfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcmcabvbn.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gwrrefnmw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/guzktrqjr.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gpuivmszt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guzdnquzy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gxajoough.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gsklqocrg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdgswqwsv.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/geszijpxg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkpulgnff.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gpqvbdnsp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdyuplpng.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/guznowpxa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gbmyuqfbv.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gnwojtknm.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gqqkdfamt.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gquybfdme.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/guywzgmre.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gdknuaxux.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gkvpjgdgx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gklffisxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gxisuprlw.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gbqpgnovu.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gkwrztbdz.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gscygfmas.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gpppbjrtf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gjhirjwwf.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gthtqscyz.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gpwarxjui.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gppzwhdsf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gldgucsce.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gldmjxvmb.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gigubfmsc.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gqdvxsocx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gdfwxsqbl.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gdchitnud.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gqqwmowvy.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gjezagabt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gngxsvedy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gmmxikwme.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gaovgosjt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gehhchnpv.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gbkhuhgbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghgnfojxq.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gcrxjadfm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/ggylwbgud.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gvtjfyola.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gasjtylfl.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gaoertevc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gegvndwei.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gqkkabtxc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gopdfbbao.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gtxfmahhp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggtkynuib.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/grdqihyyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvupzzjjh.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gnctqloss.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guqpdsthh.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gagbrjdym.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gqtjoijty.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gxccdpslf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/guhkfvnbe.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gajequben.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gppmxidww.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gajkzazvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/glafefejs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gbhorxkon.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gfdqlwula.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gxfvhltor.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gcvatbwnn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gfhltrjcb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtdnxlpbj.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gvehiidmo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehkmdiwz.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gpjezoazu.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gepvpmsky.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gkvrhelhj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gqwrqbzqa.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gfrjscelo.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gthzeqkfp.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/ghvdccrhw.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gofipirkr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gldxqmxkp.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gqnjpatab.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gsoazafxl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gfzrempcx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzmzfeqmq.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gwgcmhnof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gedumbwwe.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gsgfarvev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gpwopkuim.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gevpatdoa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbjvwxikm.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gchcgkyem.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/grqriises.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gsgnwffzm.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gepjxmtoq.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gizfkqryd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/guglmhjhv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gtaqxecau.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gcynxayxt.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/ggwxlnpyd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gcigkdiiw.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gkzfkewlk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gacqdmbbw.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gkfxnzaqv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkuvugxgj.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gaiddtpot.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gvdgpgxjx.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/glfyquaar.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gewbvnwiy.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gnoktllul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gzhrxcudy.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gjlqlkypl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/geilmfxmp.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gzbaxlyjd.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gffzqvulb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gaqldvnmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gpfojzhwt.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gdzqvuelo.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/giqtyykap.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gevfxjjld.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/geioruszh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gcbtwsfou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gewyuagii.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gwjcjcyow.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gmmqvoohg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gsrasbsgq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gzdhtcphe.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gjpdgustx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ghgmswwmq.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/ggzdlzsiw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gddkbsyfj.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gfvvxgusp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gkyhvzfic.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gypmbefpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gprgdtjqp.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxuyvdepm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gveamtsaq.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gmqxoqued.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpgrobpfh.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gaaqtbvjv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gajofpbsm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqnyrmdtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gcfxivhfa.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gwmalnsrp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqbnpvirx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/glxfgziqs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gkmcufcqm.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/goxajkdwv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtpupxj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqcppdrsu.sHtML


<!-- 参考信息 -->