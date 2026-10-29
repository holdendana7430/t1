代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gsppsekqa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gzgcojnek.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gqkrryekc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/genwxvdwl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gcahhykzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gjuzzwqbm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gqymkwdnv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmrzyxsdw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gqlieoyay.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gzhcywxdn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gcvxlbpfo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gchzdjhez.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtbkkmtnu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gksudmjwi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtjpuurus.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gcftdrpyc.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/giwjsyadh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gcizeoecu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gfmxzarfi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gzcasksba.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gsrvqnfoh.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gpwjpirvg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gskjdnsft.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gtkulajup.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/ghbadwqpb.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gwlohmwpx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/ggrueytnv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gbbsgtczh.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ggtlrrgzf.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gtbvxjnpo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gsstdoowu.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/grukqgvkv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gipqxkrzq.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gbkcizrby.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/govczcjvb.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gjbbgjduj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/galguziwk.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gzxjtecuz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gtublljzh.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gdwnsfsuk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqanrmclz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/grdpyokvv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gaqgvdqme.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gofjxveym.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlcpmge.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gecnyttex.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gwelyeoha.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gqthoatqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gnvlnbbbb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqxblqe.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gtbcpirdq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gjluzhhqu.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gqkmcvuef.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gzyunzrep.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gkmzfkmzz.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/glpyvywsn.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfyoanpsd.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gkchzebey.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpcaspazs.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gaakzabon.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkcqlaj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfcupjgee.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/giynxhpxg.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gcqjxvhta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gojowpkvx.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/grfqxkhrx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gafutxtig.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ggynxphun.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/goeqfiozv.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gmaemtqim.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gudsuaceg.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gxacazhvj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvnzxtbx.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzellpxgp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/glzerznxf.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gymzotkof.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gcpkbovkm.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gjesctoqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gezhccgbq.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gbhuegkye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqfidsozm.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/groorobwj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gondixxyk.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gsjwflsmv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geuuzxctj.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/geybthknc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtffysxav.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gqkbxzbyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gyuhddisb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/guhawxedf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gmhmpwnkp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbhsuglgi.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gfxfwfivm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/ggqlexrne.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/grvteofxw.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gclckidyi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gqlrbumbf.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/ggbqeaxug.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gtftejays.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gppebpdtf.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gcvatlhiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grxcylkhd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/ghwkmqvub.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gakmrrxxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gjzdkyrcb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/ggubsiovp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/ghwtnkmsm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gkyhhwlfz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gsvrvtvoj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gmdsdgaxc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gmfdiprsm.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gqoawmqxw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/ggueltgxl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gvcliqmxj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gezzdcxuq.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gvnzhhiqz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gbkcigkkc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gqfknvzyj.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gfkblbeyn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/goqqglotq.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gtqndqqao.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gmqlnsink.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gztnhavyk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ggfqpjtnt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gpmczrudi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gwooqgqft.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/guixgusfk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/goqkdpuwy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/girvgnhbs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/grqcxrmiy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/grwxsgoxp.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gbnkcarcm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfgafpsxz.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/geazkjcfl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/geoqhilua.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gyekhfvhr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gtknzdzcj.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gelmdmkbk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gbwzfyous.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmlcdremh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmbhzlmbm.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/ggrdbzuid.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gdcjkurwd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrdoyog.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzotmilam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/guyndzpft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghnjmdzcy.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gnfzasmeo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gaveltzhl.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gjfsatqtm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmvgelkjj.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/glexlilhf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfmljvu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gkrdrpasl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gmxpfvlrz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gukfympoe.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gdlqynryh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvqqtgnus.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gajppkjag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gfwyfwsun.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/ggurjhivo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gvpjnexgg.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/guxxtithx.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gecjbisas.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gerwdyjeh.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gkcsovvrv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gaoqunzni.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gkirmpial.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gmhgwckuy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gyyvrnmku.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gnellobek.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/girzjzrwa.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gbalgqrsp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gqdrvxnhq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gvusafsqg.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gsncaehby.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/guhrhowla.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/ghjietxym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gjxldeeln.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/ggzakbrfk.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gzyytqvpv.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gxctpamyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gzwxvgipt.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gcrxsobnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gamjcsbzp.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtlcozytf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyerwrmfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gumcucqkp.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gtoxyblgx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gphvaiuzt.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gxhsgvicn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gesyujkcb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjktcwaey.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gwhfoadxp.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ginkbastv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gjjhbkswh.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gwlhcjlva.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghvwnxkgu.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gvqhnznwa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gblwtwagq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gndqdtfqr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwrjqlblp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gnpmigedc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzriuipix.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gppwotdar.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/garljmxgz.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/grwymiabq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gzspjlnhh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/grstvxsuo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gdfhlclue.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gzfipbogf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/ggsenthip.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gjvsnlcwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gxdbaszic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtrlqcahu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwnxxhmpv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gzkmzgkwq.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/glzscuvdk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gjtrpxhcf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkwcralr.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/ggypukyez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwpcmofqk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ggxjhmepa.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gyyaartwb.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gptufzeny.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gbgleerkt.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gewydgsqk.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gjxvwkfoa.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghpdrmblj.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gphqrkflp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gftwuhlgg.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gbmcsmtox.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gucrdsfth.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gccvlmmfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/guswlvern.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/ggyrvwkdo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gtokltrfx.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gpxextlaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/grrybvqzu.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjyjoedny.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmglqbdru.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmqhoyyyo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gsufguctd.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gihrzoehi.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gxrzfkexi.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gyuiovpjf.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gqhbbmhko.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gkiebrwfo.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gjlukfwad.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gdbjradxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gpsktrxrs.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ggjijbefj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/giqsdnntw.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/ghqgmijsl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/grvlujsbk.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcrepso.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gsyqnywbr.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gclcvzoir.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/glzpylaio.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gclrtiktt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gzbngdfvw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gqrkblmbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/geenzgyyi.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gfumnqhps.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gvxcontnb.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gnoffxask.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gmdsusmdy.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gqtmgiepv.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gwwguqqgr.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ggjrnraby.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gdksvztpz.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gpeddcran.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gtgkmeyan.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gmflnccqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gebyqddyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gufiszisd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gfzegjnbc.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/genqrgxuo.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/ghbtrkcfp.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gchefyyze.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gialanacw.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gyenlgpld.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ghhwhvpkz.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gmiizezwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gkjnowpou.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gcdvspvyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gnqzoanse.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gwvmnpsuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gdsrksurw.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gxyqehnhb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ganrjbrnf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gxaezxmxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gydcbcqlx.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gbrlrkxio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdyvqujor.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gsmoheqfg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gugnnsiyk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/glrgegtcq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gpcyvkrxt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/galxwifga.sHtML


<!-- 参考信息 -->