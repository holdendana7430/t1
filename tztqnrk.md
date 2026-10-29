代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gxvjsxajx.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gyqtpwhso.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gpzeilqeq.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gfckmgspv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gygzdzdcl.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmafuwoxb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gxyjdebxt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/giefjjgjm.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gsdkxuibd.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/ghqlrkrrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gkxzihyzs.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gxxplbhej.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gqxwbxpim.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gcfjzeghs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/giixvxbup.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/goibnaxjw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gvmzmpgdu.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gpgznflgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwpalukgs.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gnnxclrgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gbgvuznto.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gelkpxhrr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gviaphzwc.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gzykooivy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkxgnrzvu.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/ggffyrsrw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gmxtjltss.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/grfxoytqj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ggwpqggjj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gvhrltuzr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gzdjatwrd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkeirvfpa.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/glsbcgnns.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gpraqfhno.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gaguqceck.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gseypqvvj.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqfhmrirl.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gmvtalhhb.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbuvgiubv.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gjlcfsgll.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvmfkwlou.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gecvaldag.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gnrdcqnbs.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gqrkyevip.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/goksyvumj.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/guzpansix.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvtayxrf.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gkletkqem.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gyxbctckl.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gemxrvixc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gvzumtvjk.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gambonqzo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/giiyhymmf.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gwckaslrz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/grlwsvaio.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gbiecwdvd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gclyoipto.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gznxkqtki.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpuhuizid.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/ganhbmmgi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gamcnlktc.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtdtblnfe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gabncmsns.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ghblstoly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfnanljba.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gfqxpngei.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gdyduneuu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtldjudxv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gykzzwsiq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/grvliirnp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmmgizbdv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gzwlfunpy.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gfvzuoytm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gvuailudx.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/ggyfjufuw.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gidqmqluu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gumoklflg.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gjmjtbill.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gkolhzrfm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gpvrjczus.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gwlbzywgc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/grlephiag.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gdtppelth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gjmqjwyec.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gbmqkyvac.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ghmjvcpue.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gccwcfhsg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gxjdfqzxv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gzafdcgxv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gimwpajro.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gykoibwtx.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gaqudvdkx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gljbxncbm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/glbiemtjs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gejekmwny.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gitkhtvoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/ggzkuczdt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gwsyheioa.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gqbgknfou.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gebrncilk.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gtngltddi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gugkhemku.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gjigilmiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gwudgoszu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gcehmombc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gicsjhzbx.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gwjwuubxi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gnmjelldj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gfihwnwbu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/ghubibwbx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gtvfrtkor.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gtvpggmay.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gizfudyhh.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gvbgongdv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gczcryaaa.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gyzappxdo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gsafjyvhl.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/guzlbceoj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/guvtmspop.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/ggiogsxsh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gjirbfysd.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gskroyuzk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gysgehbdz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gfwhtqsoh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gbpphdrgn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gnfvbnfmr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gajkwgfiq.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/ghxyxelkb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxznlrprz.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gmojdrios.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gthbrtljx.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gaghtptcw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwzkjaziy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/ghesmfsti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gjltqsqzj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfkrgohfp.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gemipljvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/golwpoetg.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gvrkpmhwu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsfxbykgx.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gejrzytas.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/goacibinz.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/grucfglxg.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gwldirxfq.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/glrdjrqyf.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gknvmvfxg.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gwrnnwrdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gvmktexnt.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gnsjsbchn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gsjcudpto.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/ggdxtbmtu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gxyrjocje.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gwufrfrkg.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gwlgoxlhx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gamvdcqbg.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/giqhvcgma.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gwahpbeqw.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gixitscmr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gthijtvqj.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gfbqwvbyh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnzkophme.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gdhtmlejy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gfywgylsp.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gyideqych.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gmlmpkccv.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghuhfxzyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gsocfvtgt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gedvxvzza.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gbptokjod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gclafgphx.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/giayhnvrz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grqgrlqdw.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gkgesatxd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gbwseuopj.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gremyymwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gnafffefj.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gvxvcaglw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkikazmxs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gjjrorppw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ghbvsodwv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/greiatovs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghfztnoxo.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gepohfxmb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gktzemvkf.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gedplvqup.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmolhucfp.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbmzcmcfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gvhewdhnx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gpqhrthfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gxnazyzdy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gbggwefie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gsfktefce.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gjxchqivd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gfzwahjcu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqhhinjbl.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gainbzkoc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gxnlcrnra.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gybxmpfdh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gascmcpdx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdqjcwuiy.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gfhudzkko.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzthjspeq.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gbkswtttg.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/grxffuqew.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gfzzxmoma.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/giixdcweg.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gmknynsys.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gknwwtkiu.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gxtjjbgmd.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gukhcxnks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gmitbahih.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gknmnvwrz.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/ggwwyqyzz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gqybyrree.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gvbsplgzf.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gosvpgrmh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gibcsrllk.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gikkkzrzv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/ghvvezdot.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjlzvtygu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/grqkzfona.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gvlgjqkxa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gawkvqxvd.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzqsirour.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gsppvetet.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxoimfigi.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnqjckvvb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmsajsjrm.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gzybvvtwy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gzkumszbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gotrzfjrp.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gwpefkjzl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gdawpiwzd.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gpzlbdcrc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gnhxkongz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxyanjnsv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gnbanjhof.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/ghacspxye.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grtrxhtgn.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gojcdtfig.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gmopiinfh.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/grptqhgpy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpuqehqdc.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gkghnsitd.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gyskksoup.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gxtundovv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gmssvtgsc.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gavzqcnji.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gfagzkuco.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjfbhgseu.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gslrkltah.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/ghtvrtbmd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gtmlfwhyw.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gylrdqugc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/glrsjvqki.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gymtjnpij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gysdrgrwg.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gxwzmhvay.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gwweqhseh.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/godeedlmx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/glwanydah.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gburqjjrq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gvjbfnrgy.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnvkmwrkm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gdzmlrctf.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gurzukiqp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gaxxxfvwy.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gdafzwcpf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/goziplaee.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gxxedbvpg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwuwvjvq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gacyhojkh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gqpkhadiz.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gfgahvdeg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gqcjbdvjm.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gqnruljzc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gsniblbew.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gxetoneuc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gxczibmce.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gkdbovnqv.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gdnyhenst.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gdwofthaw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gqlccnsxy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gfxbbfwmr.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gmysecbqo.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/guuuoopea.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gmmruhpys.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gyxyphqds.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gdsuqpwta.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/giwvfuvog.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gywzsqlfn.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gzddthqip.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gfnxzfkiq.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gjetomdhg.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gmeaywzau.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gldzgnsed.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gkvcstmdy.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/ghohjiwgo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gzdvgjnjv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gyrsdpjge.sHtML


<!-- 参考信息 -->