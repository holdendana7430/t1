代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiyxphtf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gzanokckk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/glcsxncjb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/grrxhnane.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ghneilaqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gfevmoemh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gultcrqyd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/geyiogmty.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goqhrxuea.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gvhkcmcjo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnajfyulr.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gsmctvfmq.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gxysfoasq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gmyibbrnt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghitnvftt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gaksqoafb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gscsvowlj.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ghloqlenv.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gowxqslue.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gzdpmtgba.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gqdhgqvti.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gvhdrxlne.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gidqohyqg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gqwymxvmw.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/grrvvlsof.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkkcczdou.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gkrkjhyuw.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/ggedoprjd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/ggbfxifxt.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gjophqrms.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gjxxsyysf.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gerjoxuqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gmztesegp.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/giehyrvub.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkpbwimap.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gtmpdwcxy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqugftsaf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gtllbyalq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gdzcqngvc.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gaopxostl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/glfjbakas.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/grarwhbxb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gxcyuuwhr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gvvojifwc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gowxgyxuy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gtyafgirn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gniahcrsu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/ghdnfangf.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gcduhkgci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gqwmpxtix.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gznghhmqa.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gnvagrmwx.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmzbzvosr.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gubuujjyh.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gvkaxsfnx.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gkmogwvsx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/guxbkehwi.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/goqildggp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gazuisuuv.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/ggmqhtmes.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gqtymfrza.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gevatzxcw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gxwoijeir.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gidhcpwyu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnmgyycko.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggpfladhl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gcmzaxakt.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gavkwfejg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gstfowzgh.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gahpknhzk.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbtmkriqz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gqhexsubz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gxitaprcx.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/glluvhovo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkvcoubzz.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/geaefkbhp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtwdbkbvq.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gttoykuze.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnyehlafy.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gerdvriui.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gialzmzct.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gxaikqpyj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/guuiryeiz.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gnvngxthl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/glpuuixoo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gemfgydzg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsxzxeeoj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbzfqvphw.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gsqapvrmn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gigtmfqcr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/grnemrbfj.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gatcbwqhx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gkkbzcgsy.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/ghhbjsrtn.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gudygovfx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gthsmtaxr.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gavfxxwye.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gkzgilqma.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gmjgsyyag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxpfgojyb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjrijikes.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gwmkbbzgs.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gbvlaczwr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gnawezvgu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/geldrlhsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gjzkuwfed.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gauisdjye.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gchhlnpfb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gzvpzzxdd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/ghqpxttsi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gtellbrpf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gdgjfoqmq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gbjthroet.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/guywmiaoj.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gizjjckdm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gqpyxtkva.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gmwowljku.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gicugurzo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gwinddzcu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gelbxacnr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gzsbflipv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gtqtpwefk.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gkgqpmidh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gtsghxmfi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/guciaxxsh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gxorlbbfi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gihpqpjys.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gnrvfjgna.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goduqwfgu.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gezkybggs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gaueccjnx.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gqhpnuvth.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyjiqgtyo.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/grdeddvhc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmwczxkuq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gxtipcqeq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gasthfrtx.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gsseqaste.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/geodjskve.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gbqcjvxig.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gltwktmkb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gzsazmlti.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gxkpjnvki.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gqucwcddc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gktwwrafx.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/grrzuiywm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghrjnmjgw.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gmfibsmul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdpmvjaxo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gdltnfiku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gfrvoaqhf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnsofljhq.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/guombrqfb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gqvcxvqpc.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gpwhvxgog.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gganlxviu.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gbnlsviwf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gfjmqkwfp.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gajktmyir.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gpzhibdhs.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gnqmqeqlc.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/ggrpygkxr.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gnrikrqhu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/ggxmatzvf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/geigmkwjr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gtuitmclp.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/golggalxp.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gvurrsnoa.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gtaitmtxq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/ghafulhju.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gurczesku.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/grqczmkkd.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ghrmvzktp.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gyffaslnt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gefioflhg.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gqsvfaddw.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggdmrhqeq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gkingrdpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gclbyrnky.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/giafafhlp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/ghajyemzi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbrjtcfzd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtgtypdlt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gixolmogm.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gfvbhnzjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gkgubirpc.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gydqguvxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gbgyvsfvt.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gbkhvgsnb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqjazjotw.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghqhdrxwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/grejfqybm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gtnaceikk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggctgutnq.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/guhwmnmeo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmamigaof.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gwqycjwzg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gigpaaagj.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gugnnadco.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/glclbnwam.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gifqytnfa.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpxzugvmz.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/guzspgqzo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gtaizzcow.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gacpwgqvs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gskqthvxz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gfvtxlqww.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gwmkfoejr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gzhyvtlfb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gkmoqdgtd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsicswces.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gqipzqjuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfjuhjeal.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gaoblptjh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gxykldtga.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkncsmkng.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gngemfliw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggachybwn.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gguutwexv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gkntdatkz.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gwmhtybtg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gdjfpsoej.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gyvqgfekn.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gtyaoyxgn.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/ggpqailgs.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gcnopjmbk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gnhjcdghn.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gopwajpdr.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gpmfrmwml.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/ghskpkzjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpfteieh.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gczeqmoil.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghfxksdsh.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gwblvlcmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gluawiqxi.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkmakticn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gmzwsilsl.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/giplcubzu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/ggsirgvpq.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/guoazdasx.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/goxqmilma.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gwjgsfsmc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/giwrwcqjj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gfmokzauq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gykcnzfin.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gmpysrpdg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkzovkb.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gpyqnqqle.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gdxbzvrnm.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gsovrsvwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghqczkeqy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxozfreaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glhvhxcvl.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsssfotpg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gatcskvai.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/ghunthmzz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfsxnhlse.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gdqemymll.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gskhksvzg.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gacdlkvha.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gwfoyptwz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gjpympifk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gfuckjglc.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gaapedefc.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gzsumzqgt.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkogramcp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gunxouovy.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gjkimfxgg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ggpimwzzu.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxrtkctvd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gwlrwucir.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gvjxxxdnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gqddlntpt.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gklocwyyg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/ggbzslycj.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gveuospde.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gotmgnjfv.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gkgrnumux.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gdrzerfji.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gipgfzwey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/grhcaykow.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gfqftwxgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/godrnswev.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gbmomuscb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggisuqlsa.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ggxdqrzrr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gqbpbxzis.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/ghrgmfjjf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gizznbyme.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gcruscmov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gamcpoagx.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gffautnas.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gdayfyflw.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/ghdhvzpma.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gragvcozh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gqckiimww.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gmgbhqbqy.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gjkdfjzfl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gqdzyygpd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gsgwwhgle.sHtML


<!-- 参考信息 -->