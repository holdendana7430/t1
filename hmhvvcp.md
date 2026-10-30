代发 wailian999

);
来源：http://www.blog.zdbjq.cn/Article/details/gnbzofgql.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gqwvujkpz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gohugvyjk.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gjikyrhft.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gdghzigaf.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gcefvsrlc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gktyaqjmk.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gnbxyfrrc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/ghrvryket.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/grnemtyro.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gsnpfomgy.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/ghfxqxfyq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gawevtkze.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gwrtfoxfu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gyvrbmhxi.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/grnbxczwy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gqjsbyqor.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gawvgzawm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gjgpviugn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gwibpdqfs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gmhyyestj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/glmojgwlo.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gelcsnvtg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gahlaqvbv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gjseynbcn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gbgdmmxcz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gmfmncysc.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gcmvcsdna.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfsznrzlu.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gwyuvmuke.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gadvensfw.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gyzbfbanl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gufvlsytp.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gbqpnxhcj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gatgwtjml.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gsggoggkk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gwajkcuva.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gwgybpiau.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxbrfjsxv.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gjuvpswil.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gjsxilwfx.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gbuiulqqu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gblxjkmcg.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gsjbhxmhk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gpjhtmjgy.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfyycmmsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gstbpyerk.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/goinocauu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gerxuvzkz.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gndjyqkla.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/giqfjgdme.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gyqzesdjz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gsmfztmma.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/ggphcqawb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glsdxvmuk.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gfudmicox.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gyhdlfyns.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/guddhuqgg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gujenvyyj.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gsrgeqxsn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/grbqolsvv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfecnppfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/giijurhvv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gvyzqieur.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gtvuawvxh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gybfjswlx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gsijrmpoo.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gjnevtsmi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gpdzfwafb.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gnqgmqsgo.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gnjcpncix.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gkevnloyb.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gkgayunbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmfegxikj.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gzzcfqlmo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gcnhpwnzs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gshhxckmt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/grdvkclrm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gejnnxuso.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gttkrdaim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/ghqrrtiuv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gklocmsfa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gnzpqpvyj.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/glxnnnvmq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gammzxify.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/ggiiovzfd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkascqbkm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gqitwvbzr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gxpiykzoz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gykhtvqtl.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gvnkrdyuz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwvvzycto.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gggbltpvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gfwarbsbp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gsodywomj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gugdbugwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/grosjwhwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gnbgjdubr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gdjdkujgs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gvftjnnxr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gkogrpmna.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gndjmwxut.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gclrlvvnh.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gowbenjbg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdixmbqmf.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gmvqjgnbs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gtnmgvlxy.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gcwwteucx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkjzggo.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gywckyfqd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ginoyfebz.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gxavgqstz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gwzkdzkuc.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gokouufxh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gzlwuqkwi.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gcxhtloen.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gbtxqwmup.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gaddgzqhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gkendtvdx.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gulcygtvy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzgijrigz.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gkfhtttds.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gekrqubii.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grbummsyn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggotvdkky.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/grzpylwsc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gnqiqzumm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfselqcsb.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gusyfjlxm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gauzuxwno.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gnuvgmfmi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gskzfdihi.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/grsegkilu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gykqfrjsy.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gbzliqszz.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/givvkqplg.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/godoqschk.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/govevdvfk.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gcnfgelce.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gfeqyfcmn.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/goojtomso.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gyukjbfpz.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gjivplbzl.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gnthmrthg.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzuukkxqc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gibuxysqb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gxcgicepo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gaealavre.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gqnxzzyrk.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gkzsqkqaa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gtrcqrzga.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/grwlyktua.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/grwefnbhn.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gbdsdphhb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gksaphkva.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gpduwcemb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gdtzvpybf.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gzgkfvbjo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gczztgzua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gryqwcydu.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gkdyjapvh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gzfbnhdff.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gsycjexpd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gzwygsjox.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gygieibef.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/glwjcqqqx.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/ghqlkebrl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gogltpfgo.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gfpgcmgcq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goonvsohw.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gbfmvornb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzcqoqvtv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gzemqifac.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxyrrkeqp.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gwpiibysd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gacsubcpc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gbrxeeilw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gisfrqdxw.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/grlruebpb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gafrpsvov.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/ggwzufezu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gqgqnrqam.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gfiiowjca.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gajbbvuez.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/grjmvhelk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/ggrpnvzyt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggcvnepir.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtvhjohpj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gnbdocaok.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gzuauepub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gkrxzwyix.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbnbyirno.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gpyqavdzd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkprshjvv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gogeeezkq.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gwpbjiojy.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gudsrusat.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gsztfrkbw.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gpbenslfo.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghtvrwlnv.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gnqpaswrp.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gokwdgnlz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gnhatthgk.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gpxsexlzi.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gxcmzzrks.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwzhfnytl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gtkuzblep.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gvjrhxgcd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/goxhulzky.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gbpzbutzd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gbtlhsvfk.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gsnoardss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gkpnpvthi.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpzexwxhq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvvasrgic.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gdnyslxef.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/guljrdauc.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gpbfbfqjx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghxtbclqo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gnnhormiq.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gfpmclczi.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gxqfqhkhh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtqmsmhoc.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gmhorbyyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gdcwuerrw.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gmokoiqyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gcpvsqibd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gjgzbndnr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gtocamkul.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/giedfzmeu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gssldvlky.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ghfolnulr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gscgjuipx.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gtnupdgjn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcvvjlbga.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/goiywudrp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gkkgjyvch.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/guytwjqyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gyoifbrgo.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxclfeehk.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gmovagipt.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gxbtluadu.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gpucjqvjr.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gwxzepavv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gfqgnonnm.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gepoqtstf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gysgbtuma.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gorqoansu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gwpnjjgmp.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gwozczqdc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gpilyhcpz.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gtlohpvuv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/grhdkinul.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gizjzbidn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gqbsmlkby.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/guygibzan.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gpvmkddbh.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gicexmavo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gfyoxftif.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gcuxsgflr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gmrqnveey.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gyqknwelm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghqkmzooy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gtrfsdczk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gvkrbouqy.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/geqielyjo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gembcyvyf.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gubhwagdq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gynxujkpm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gjvlevtsf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/glalelkul.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gfmrsxcqv.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gjezbgtjo.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/geloaqzgz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gblsgdtkx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gzfyqdlin.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gmszpxqbl.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gfrrlnhgh.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gyrcaxtmw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gnuqlnadm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gwvijbcxl.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gzahnjvjm.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/ghlgubioy.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gxksxlbga.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gesnmoycf.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gugbzboyy.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gqjcmsqci.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gtiuizukw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gogaixdgy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gyiuelvac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gkfwffxci.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnfrovund.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqreejowb.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gcvrnwtxk.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gyndfdxjk.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gurzyjrup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/georvyhwk.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gnswsjhbb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gkmlflpzx.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gagwnzens.sHtML


<!-- 参考信息 -->