代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmgkysez.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gdmasqyog.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gluqtnhol.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdfqowkj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/ggilizhpi.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaqsdaxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxubexdu.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gzhekszfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjuujprq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/grhfpbnex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagukmbw.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gaasreskz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gjhibfhwm.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gavpfxsfl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gtepefreq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocqthrk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gxawgqvdk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgfontyv.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gicatqgei.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlncgyux.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsdkhrmq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjqonler.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzzicmvj.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geceyaliq.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqnthljat.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gokumniuu.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghscwrqvw.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ginyaaxnh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqcecyj.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnomhhbte.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gctxivslz.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gctjwavxo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwtdrqns.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/glkuoeqrk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkkmpbyi.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpfwwmgca.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gubhpmdyv.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmxktsyft.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gisvekkfn.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyjrcuma.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfvsigat.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmzrmpj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/godunnkjl.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjhqvvni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gctruobku.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwarmokpo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzsqlwfd.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gbxsnthbn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gckskwfiq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdyuiulw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govqynrcj.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdaroqv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbigydpfg.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gtxctqujm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqqdjhj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfmdutiwe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnlrjzo.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/golimqygv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszxgybm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmyshsa.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvvphchd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrkftzve.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrsgokaw.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gstrpkbzn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gczscqzgh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoqpuemh.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gempqqgdn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmiavslv.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gpupohvht.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gofwavksk.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/glivzguwt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlashypy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofzqtako.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gclsmmmjs.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gfeljhaax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhjuaftt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gimwwffac.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgcmhhk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfedxtuis.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpxgdmnpb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnocctam.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gkavwcngy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahwtpvm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubcezcqj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiilrffk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ggutttdor.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkryfqlos.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkbdgwql.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaqohlxr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhqkbhuh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcezyxgal.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gslofvoje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gokpjkqvb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gdpjwvvlt.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfohoblfn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gtyvbisyl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnifgxrym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjlpfrcg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpycpusb.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gkpaewprr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gonaiiusi.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gawqcpfmj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gjqychiao.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqffktqg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtdymij.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gopucemus.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gahvljwne.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/giaqohbjr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafxggvbs.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkklpdnl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiqzzxby.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfseoaag.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrjzdxaz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnrsiups.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrhssxct.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagzrtih.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghztxmdqw.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqimqmsjk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gitjgaddm.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gxgevoymx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghksvwpjt.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gefknqddi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdhnrfix.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbskwmyoq.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gufydihkg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliuzhgrc.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gdsmtcbik.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gugsafewu.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdsfupoz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/golpqxyla.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/grfambfoy.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgfipjip.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gjrjkpbwa.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gpetbfgcf.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gxiibccel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqlysxmr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gjudgafrm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofezilu.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gnalrijvs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdbuxsgk.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwplolaxl.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gywsfmuvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gracuacqw.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gsarppmkf.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmvsvavi.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjydjbqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpudqjyc.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/glvymslug.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqrizsmn.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gfepsxzrg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvdxfsoc.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgxwlnn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyfvigiz.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtbeolkxg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gepwksbya.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsfvfhal.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvqqnlir.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzpdzeig.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gramqhqld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxawsoxo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgqgcaph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjesqwsrs.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/giofynlqa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzmznidl.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gogbzcary.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcxsshhyf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoswwqeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guelpsbhm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gyysuugpm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ginaajjpb.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfgzrtceh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrojbrom.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gcozpuovk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzkyjqis.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gzrfthjgt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gapzqjdkk.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/guvkvvuhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glumjgajt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolgpbkb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvhpxmfa.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gsgjvkqxm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gwamhgtxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxllnwo.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbjymhdsc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gtubposrr.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwqwqlhsq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxebmmw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmkgaleb.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gkibchvnh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzqphtqaj.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gnkacjwek.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gboerksdc.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqtmsrtd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyrgfvho.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/grcoidoxg.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsrffnyw.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnpbjlc.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/guqkbrhmm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyccxlwwp.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuktnjqe.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzezmlpax.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/grvrcxgwf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzqjfgfo.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giaeqfgmx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghucpwijl.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gawugznet.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/galsemrbn.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghawayfcl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnhuzjtmy.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gqdvpkjan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxslhrxha.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gwuhjkfzp.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmngjxse.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrnctdin.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzcnajg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geepnnbrz.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gtbspxigi.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycctcmb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcfozqrix.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnomckmvf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geecftcbb.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gdaoqkbkg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gifdqvhvz.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbrsraath.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcgkxqdz.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpeyyor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glssuvwrc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjutxnova.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmlsdexlb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxyyiqwx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvzuzxve.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjerkosj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchcxqvf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghauzfovb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixjfpvo.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gawqqbrka.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfaudwjuc.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvywroks.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwccbmsc.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxrwixjh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ginqhqqyp.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpkykyun.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gldkelowk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmlbguho.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsnmqbxx.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gomjchwmb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmdmdsal.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gbtzxmejr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/grdwzzudc.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkjzjyda.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ggxsethjk.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrvflbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gudhjlhig.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgdtmpvq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gxtwnvmqu.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggcbzkkcw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtcrczc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gukrucopt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzrmlgt.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gybgzgbvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gduhfvbmh.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gkytnwhwk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmrepim.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/grvodohqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/ghtlircnr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqumuwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gortxrewe.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqboanewo.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gubxwsoyy.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdlqrbfu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gdfmoiicj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghofvvygp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcayoihwa.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqzfughf.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrinzzjh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxjqpsgg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkvdpwzhd.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnlvlysv.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxbrtebdp.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gduycfnes.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/geqahjzob.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxyhifkr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwztcqje.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowccpps.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/goqaagcep.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glllgckkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/galrkagep.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmihkzg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpxwptce.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gvakmttdt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuetjlkq.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjakjizof.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoaaetri.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboumypns.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzmstawrg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuquwabv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gngsmynfo.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gphtfjgyt.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbiaolt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcfcxstv.sHtML


<!-- 参考信息 -->