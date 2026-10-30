代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gabwxjezc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gksthkzqy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gogxxvrrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gqvemfljc.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbfngqqfu.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gjiekugpe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gfdgxcmnt.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gqqsufdwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gdyrolroq.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gkzvandgu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gcsyzjpld.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gxwiojwxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpguwmw.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/ghhafdsiv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/ggyqtoyeo.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gsbgzfcpj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gphtfrrqf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/geyzudjrb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gpevejtpz.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/guwcekwmn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gpbihkxuh.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gzctjvxfm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gtssbmfjw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gikcqhdpp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/goyzsfyvk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/goatcfnnw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gflofnciy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/geqxkzupu.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gktrezjxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gwzakxqdb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gnapaoiij.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gpfqnnkko.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/guefgcozk.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gblqugksn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcobyjevd.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gvxwvkrct.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gclkukvpf.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gpuozkhxl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gcqbhlkad.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gmxyjxxuq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gskscjquk.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gqtklrzkt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gcjkbelpc.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ghobombew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gvovydpcq.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gltbnyush.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ggwvlsozh.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gwsfqxnjd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gjicvvxmu.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gowmzgswo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/geejcgdxt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gllsqiwtq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gxzuvyrcs.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gtvunncwo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxasxmxjr.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gdcouaips.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glogcrzyf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gnbvaqcao.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gldlakchf.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gmmlirocn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geqmvojya.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gifqmsqri.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/goypdsney.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gyghjdptk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gwvkgxrub.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gcnkhpclo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/getyvzcwh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/geydyidsf.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gyktkmmlf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gpcamvzqs.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/geveqgxwb.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gvvbmkwtg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/giudcmfjg.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gpglsgtqd.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gslhqhmtd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gzqmlsbdm.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gheflxfko.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gyklpxehi.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gvvsmcefi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gwdxxcgbr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gpsqbjkhm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/ghjkftsxs.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gohwsarhi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gwgyfzqcn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/ggvqnvzuf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gvlipcyjv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gyvrntlzx.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gxdllbaor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gretvsocz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gdfxzdmyt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gjroufrca.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gehnxnilc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ggnpjrcqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gsclpzflj.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gdeikelbl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gnndvdori.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gmuhuwdqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gvgwzntvb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqhcryibd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gkrigrpaz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gioifggxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gamktkxzp.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gulifynsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gadwnquuu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtxffqcwh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/geivmegtn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gkhploxpc.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gtzrzojqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gnxnhsxql.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gpqmnpbqw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gwlempqcr.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gjzmwtwce.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gutfyywwi.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/glmbjlnja.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gixtslptk.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gvgqdggse.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gdfpwyqab.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gzjieujli.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/grudyctfd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjunxmitq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gxsfliqwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gprjwuytc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gdqltmalc.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gfxofyasy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtftbbgav.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gvvqhufck.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqzntyczw.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gglkizxqu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnhbstwtv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/glhmbuele.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/ggnchuaba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnunjjfoy.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/grvekvfju.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfmmtpsqp.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gedtfvdln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grpzoekgd.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gzxtamumy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/guzssxydb.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/ggotzrkkh.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gsubrjkry.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gkzggskce.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gvcsqnwdj.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/grafifhjt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gmxxbuzko.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/geukpqimw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gvksewjpp.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/goxxoljtw.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gckouardy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gipefciug.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/geqwwfjdi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gswtztqni.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gucvxwwll.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gvmqduwdl.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/grtocpozb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gbomidftt.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjhetgzrx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzstdpljh.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gkunpgnjd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gqsjfxtqq.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gclikmttj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gfiegmcyl.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gjvqxewtb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpxcoulhl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gkpalcxai.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gpgvwlllq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gjgelcaae.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gjiebbcuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gxzdkhpau.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gohzaxpdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gpupzjjij.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gevtbhjfs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gtaqyxbwc.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/grttrcroc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gycdozprl.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gmubglnjy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giwzfensc.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfkdkqhvc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gealjvbit.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gdxnlzuuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyqslkqgj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gvvivszqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfjwwrncv.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gvqlqhzwc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gjhbyfnai.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/ggaqapukd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gwqgmwqgi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gqvfzopvu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gmdfudvjq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gzgahjpwe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/guncmtbmg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkkzdjtzy.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/grzeeglpn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwxviaofi.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gguhmuoec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gjmmztbnj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcqujeebd.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwnwwrzug.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gschbcpcr.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gvrscwkno.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gcztbuuyb.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/guadffxqc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gwuurkjjh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gftreuyoz.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gtpnpugtb.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gkbbitrhg.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/glmpktfsr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gbihzslqi.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gusluvrqz.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfnutzaoh.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gdkctngah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqcvksicf.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gdnbedtna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gzgogdgmp.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gqssrjnqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gbntskahz.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gknndyrxt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwjbxxpww.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gqvwfcsah.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gpdrtfnhh.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/geqmiwxsj.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/ghlhddqcv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gamrdxdij.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gtrlxmcup.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gflkcytda.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gssqfanze.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gugozpxtm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gmblyckvv.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gxauemndb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/guoehtmfl.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gpcofubzb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gqxnkzwwk.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gywybuelm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/ghbbtycnt.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gykcnbmll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gxpbwjvec.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gugfuxalu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/grnfsbibk.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/ggugkqmwm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtrfnbtub.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gkieihbym.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gvpdwehxx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gfiyvrybg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gtcwpszhk.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gbianubvm.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gjmwmmres.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gqqwqorhd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/ghvwsyqjr.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gcszxximw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/geojcishb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gewtzljdo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gxosfouxo.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gahxosbie.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gilldohtu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gguwhsoxd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/guckbnmjq.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gahygjhzn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gupookvyo.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gwivvcnyn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grbyfjgyz.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/glplmfmhu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gdfvpajja.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ggasrglvt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gmneccuub.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gudsyrvgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gdmhghiew.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gcjbtluko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gijpysykf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gxsqzyqyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gkfosycvr.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/giusyrbuf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwwiswmui.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gegtyclua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gambxwgpv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gwshgstzt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gddwapcsm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gvahdzozu.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/goxavpajx.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/geyallpsi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/getegxaje.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gfpzzqlqf.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gqetamkqm.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/geqoizsxf.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gmuqbbgxh.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gapuvgjdf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gvwuwanvm.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/ghcdiwhsh.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gufpnaxrx.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gkmybtvog.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/guwwtycue.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gqeodtgii.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gwwtlqfcx.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gvhlpxjtx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gubupvnvs.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gcobmpnpb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gdspiccaf.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gumyxcvsn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gtsvqaclr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gsjmogkve.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gxmmikafi.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/govtsgifq.sHtML


<!-- 参考信息 -->