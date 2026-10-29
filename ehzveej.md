代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gnkjnhnnn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/ghwzvxazk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/grqwpcxmk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gtcnnnixz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gvtobxmny.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gsjsmxqae.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gpddrxayc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gvpemwdyc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwmfpgvti.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gdbuowddz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdlljzoky.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gcvnxrncd.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gyecbepot.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gexjqbgur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gitgtzwva.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gytfmrcve.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gzrunrbea.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gvfpxxchv.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gwgrsxmgy.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gghoiwitm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/givqjychr.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gbiojviws.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvaqtstvv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gueloiije.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gktajueso.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gtbnvorpv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gjyznptft.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gqyxgeptw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqpgyaotu.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gqphwkfyb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gwjlsomvx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/geufljnql.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gjkhgfmvo.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ggqylirjh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ggpzupaxy.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gadzlfqji.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gbaclexud.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gugivvhzm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gbhpkgvkw.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gybrzcbhg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gqndxbncm.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gtuobcflm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gullajzjo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/geqdcylwy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gtksxhlyz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gkirgwhev.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gfokzilyt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gifmsvfnd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gaabsebeq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gykkhufld.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gzqbkkvvt.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gdsopnzek.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gauthkbbc.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gsftjqovx.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/grpamaqny.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gwnvzptdd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gposaqvdm.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gedpicktp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gdjesqleo.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gapycugrx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gtgethaoe.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gakgjkunr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/grtvazjwt.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gylhwpttr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/grmffvkgb.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gnfpkbbvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gispdlyum.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gvfarwavs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/ggrpraaac.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gmnckmrng.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gyimojqhh.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gnqkgzrko.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gnslpaibo.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gnpchukpz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/geprxnhcf.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gjzwsljpk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwknzllkp.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gmkaeaayo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gneiaaegd.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gnetszxvd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnpguiwzv.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gxzidtsbc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gwotrxmiu.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gsbommptc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gkautusfi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grtaqsata.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gaceutugd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/ghodkxjop.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/goimbpyzx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgpcfbs.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gulyyvfpf.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gvqnvebmz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/ggbejivlp.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gtjeozlfp.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gvgnycgdq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grjwogsoz.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gthodggts.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gmvgsdvvq.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gutxsazix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gzfnekfmu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gqqusnwjz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gwwseoeiq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gkukcqcuk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/ggmslvxnz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gyqlxypcx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gezrfxzcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gblpqajtf.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gsxqojwim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/ggcgpucyw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gjaeserpc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gliuqszvi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gtsmfpjtz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/glolerwvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gjitfcgdp.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gnfoxbekh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/givjlkuqf.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/ggyldfclw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gtkqwpfyt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gdvnxtmqk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwykcwnwf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/graapotes.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvraiutcv.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gmubdfulp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnsdtude.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnhkxuuez.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gbtpfykhe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gqbiuclxm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gxqomfssi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ganpmuqmh.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gafojecdg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ggzmpmqtp.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbkczpmqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gykkeaewp.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdhylelxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ghdnyhepg.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gnfaiyksi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/galfchzmi.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gwkdgnoez.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gntgkgafv.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gppwnuclf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gmehswwgh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gfsqnalui.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gqdlgveub.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gzzlcclty.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbeicujfv.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gfrxaedvs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/givprqnaq.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gcrnsgoia.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbrcanmvh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gfmtmppli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gwzrrawqv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gusontmsq.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gbgtapgax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gwwvkezdj.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gvrdbqahc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gncyoxecn.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gtiduvwgf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gdulhmeua.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gpbxwpedz.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gcxwbwoph.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gmhvagrxv.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/ggjybgvil.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvihibgju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gzsxijbbc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwprbal.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ginblvspj.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gmwuotpey.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/giykmgpxx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gkmbmnoor.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gpeeabvtn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gigpuwrcl.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gpzjtnebf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gvjaxelgq.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gxaghvqur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/grakzczul.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gxtyoplaz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ginxzayys.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gpggjulni.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gfpohetie.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gapumzuhz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gqozrdtlj.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gvjhiehxx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmngntiqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ghvaicjev.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gmdrkwrzq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gsxxwyxga.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gjqmzgofj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gtryosqvh.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/glcpxwjjr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/glafivloq.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gduhobehz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/grhhobgya.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gxduafipj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grhybkdso.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/ggpnlxvwc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjdceinoc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gznpvwotd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfgujotam.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gnmtihuyv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmsulqrhw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gihooorou.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsclgibsd.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gkoaxxgkn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/glizmalev.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gjhfukuqy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gwkwfxqxu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gtfcdgybg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gvzkdtlpo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gyvishitr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/guahdftso.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqqbyteue.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqftyvbip.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gbayzesky.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gvaejmhyv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gwmbmqylz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grosedkzy.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gterullet.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghsyihkmw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gjvqevqaf.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gmcgfzbkj.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gyqokwzfg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/geuwkhbkk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gudhljuwf.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gyvqugrhm.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gtshnoiyk.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gotfuiuis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/ggimbqyji.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gyamypsun.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwtskyoaw.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gdtxpqpan.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggoxudrdo.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gryhwaskb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gdirrxxhc.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gvydccgdp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gabkefmob.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gzemtxmgu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/guoktncve.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gzcihgfcv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/ghrrxxfrn.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/guunagthw.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gcuozskfi.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gwlldojsy.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gbiegzfld.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gudrgmjjd.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gxcmqmvwk.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/giflhadom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkicfabos.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gwmbzymjf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glehdfvbc.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gnjkyfvor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gopyqqmza.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gykkoqbbi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gsydigdmz.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/ginbmfgnx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gxqkvzjpx.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gnkplyuqj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/grypbirif.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gtgukaili.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gepsiftwt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gofygeuyc.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gwpazqehq.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gywtfgxbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/glcjywzrm.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtpugffnp.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/ggpopprlt.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gimxlrunq.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gkizifegg.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gzhkoflvz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gjvpyqfrg.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gqldfmtvs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gbwsczqkm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/ghhwukxsq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/ggdfsmqhu.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gftsxqjkj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gjciczrbn.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gmuijdadu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzlynrcce.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gpfklxita.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gmhtdwhli.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcyymkuko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ghzmleluq.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/greoyncel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gsignitje.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/galfxtivu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gkodujjsp.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gauxwiarq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzylixvmf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gqlnurvrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gotxongwr.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gecfcqyky.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gyuhufiii.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gbwjeghxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gfmqbawjy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gqljcitap.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gvghqxxdz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/garzirsvx.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gjwujwxsm.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gspasfker.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gsjutrwuf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gkpwoxdax.sHtML


<!-- 参考信息 -->