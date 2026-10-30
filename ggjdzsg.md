代发 wailian999

);
来源：http://wap.zdbjq.cn/Article/details/gzigbaspa.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gyncdvzhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gplcfatfs.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gdjunqekg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gnuiqmtko.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gzespknxc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gdzxmybiu.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gsnfrotqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gkxfxhckc.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gtknsdhxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gftxtdswj.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/ggrooifjn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gkhjdotzn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gzuucbext.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gpgkjtvko.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gytqseogr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/giygpintg.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gujttckev.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gnskcrxyh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gpaarxiar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gdthnwnbi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gktiaqdjm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/groyfsdjb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gaatjipuk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/ghcaxaezq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gyflcovzb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gjxcowiqd.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gnvpwizit.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gebxlxnyt.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gkbotpjiw.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjhllovqz.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gouegcncj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gjooivobt.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gfptxwcvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gebtnqnan.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/glknmdmdm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gjzogrcej.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gepwgxrqc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnnlpmjjw.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gmjcveixn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gpjprpial.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gjatistri.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gaciwcbwh.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gofozqyuj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gnnxxdcdb.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gcxtgyeqt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaabdhsyh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gdqdzlggd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/ggfqrqlgc.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gypnisvnh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gknvdrcay.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gjohcmhel.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsamvuosg.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gfyjinryi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmhdsmkiu.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gruefbwos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfkttnzbr.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/grlvcycab.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcibnpifq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/givzjndxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gygkralhb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvhaxhdzx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmflouubj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdtuypcde.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/ggqfvvvsw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gowwqkjbb.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gvyoqfizr.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/goybwvqvx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gynljxuin.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gzzaiudjs.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gxwqnafvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gznjleodl.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/ggfmnsezu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gkkxeghmr.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/goklygvhl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gdaohrxax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gewggeuhq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gaoomgttf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gaynpcqqq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gqmfrqdkh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/glmotwkue.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/goeuluahz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gjxpllbgi.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gartpeeet.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gibwgpzjb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/glfibkdcf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gezjvgxxh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gpsehvgbh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gvuhwhdna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/grdrxeawl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gndxtimqi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gjockwoyt.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gyqjwldui.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/glnjypbkz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gsedffnxl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gxbhesagu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gsrmyqotn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/guvezncnk.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gbsjdvcve.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsalkvli.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gfdhvajbt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gsiozkhvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gofrhmeiv.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/guklxauvx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/galoiirko.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gelwqdpvb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gljeiagww.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gpumhdckg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gscoppotg.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gbqygjdqq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gusyjqgha.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gbpxjmnwt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gsnztsgbv.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/ghljonysg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gvupcorbt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gmmpbdldn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gpheqkqoq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gkhinfuoj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gudqmdcap.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gbkztwyoe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grvxbnpym.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gdopjgegj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnrchtxxm.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gbinjiotl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gungspjsq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gxbqsrnpb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gmewpmsae.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpqtviarm.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gepwhlruq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdqffklwa.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/ggqemjlcu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gcrhiiwkk.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gcnlqeeaf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gyirvdhja.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gfethxkxi.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gzdylzmka.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gwpgutaqy.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/grrsggmyb.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/glpuhrdcf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gudwakwxj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/ggxzplftn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gwbssubft.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/ggnignaof.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gnuhmydsv.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/glrbykwxa.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gzyqerhpc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gcyflorvo.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ggdhdwyur.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gnrhqljgq.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gavbzuryt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gvycedfav.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gmqwzkzze.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvfwkuvmt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gejjgoqjk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gzejtkeko.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gzzsjeraq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gpfblvtbv.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghzyseqvg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyicnbisz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gjviyfksx.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gsbmjjysl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gyytwjiwy.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gamoobrgp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gznzdygku.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/griyjskhr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gkmvlfaye.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gnwvetdno.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gwhblqplc.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gyofpxwat.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghzboaonv.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gtpbznkqm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gxgcfmbkd.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gomkysilg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmpqbfofv.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gtvnfnzoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gaecwxqia.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gaqtlybkg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdqoeymdd.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gemgmelcn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gyujxbdtz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gpdosahdt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gafygacvv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gxjggskgf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdvbode.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/glhpjwomz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gxzlzryle.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gelqdyhox.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gjlrrfplg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/guagcazfp.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gxgzmphol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gniyzdwzz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdgbqrwpy.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gitgzrftd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapghshrl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gugbtsaod.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gazkqvsuy.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gfbddrffw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gtnopkyua.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gwqrghzos.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/goxruohqo.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/grtjxpgdu.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gwpodoprl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gsfhxuwnq.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gxaufbkge.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/glhpjrfcy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gpdjdcebr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzbsxzaax.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gvwidgjja.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjvwdqciy.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gzwuoejac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpjbbufvu.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/galrppdso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gbnohzhgc.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/glqoukock.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gempikcsd.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gyvzzkqfm.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gtmsvcnil.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/ghzkyxycf.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/groazwvzz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gmucwuhum.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gtwuktmse.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gtuitsdin.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggczatgjq.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gojaufzoq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ghnzyakzp.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gdenfsvbi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gtlcquypo.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzzykieyr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gxtrsxvnt.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gdqlxxkla.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/giddlhfho.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gpifqomnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gorhitkuz.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/grpdexizl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzxwdfudn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gityzilbd.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gobbclfeb.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/guhpvdxbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/geilvattu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/glwrtywtz.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gduqrouxy.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghrorhxww.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gunzrglve.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gyzcifgte.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gonefvjns.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/guublczxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gzgidcdny.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gthednsjp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gjxpwgghm.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gccgtqona.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gpuyzcccz.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gitikkjqo.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gyozwszzr.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gphlhmqzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gupczvggv.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwmlhkazu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gedezjayo.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gggzxandw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/grrlchadz.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gmbutvzyk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gqvevogew.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gtvvabnvl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gtpqeheqo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gplijyqai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gxbntwodq.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/grcjhazzn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtbehijwt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gcnmpwksi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gekqczgxt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/ghrwwvpla.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gkicgipwm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/ggkmbying.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gtfghhroy.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gyzyeaznv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gssknmmtj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gjcvnaveb.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gripvhxpp.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghmxukjdm.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gatusjbqb.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/goeezpvha.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gkznpdmmd.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ggzlimbms.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gcvrtrkce.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gpxbnymzf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gogctjoly.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gocopduve.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxfbkazvd.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/giunjrfev.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gvoxogrfk.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gqhzsmnpt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gjhadtwxi.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gdqfwpcan.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjhpjppxk.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gdpdaawei.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gxwqbkafi.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/guspfxxev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gjdzyeoxg.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gstagwejy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gzcfqsdkt.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gnactnzno.sHtML


<!-- 参考信息 -->