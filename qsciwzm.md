代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkqhyklvd.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gyamathxm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gsjsrrlpl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gzlxixkjz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/ghtfvcrwb.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gtxtshdgi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gggbjlobg.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gxipeteio.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gqplklilf.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/ghrqduxyt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gbkqbzgfb.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gcvhhyryd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/glyvctfrg.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/guggulpji.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/ghfkcjgjl.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gqvagppjs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gsimprfyp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gsodlhsvp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gvgdybtic.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gxrlxouva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/glzvyklij.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gacvvabqb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/grzsfhqaz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gcidwghvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdzbotb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gyotqbqel.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gnizchqlt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gpyskliou.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gjwqcvhkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gqohsgnjb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/grheptkua.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gitrmijfi.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxluuvwvo.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gmfrocozf.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsutegebs.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gvzwtwnyt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gzwxbmtxq.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gzoaffbbb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gotyfxssk.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/getofkspr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gufkzwxkt.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/ggqpdhjxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/guayfhiji.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gthxibgmy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gbarkstql.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gcooxfbik.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gxsoinyeb.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gteupbijv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gydeyismn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/glumuaedg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/girbbdzwr.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gewhsclql.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gqzqokrpz.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gbwbdguci.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghpyomepr.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gxjouaosy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpprislor.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gaecqbzwe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gskctyrbx.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gqecjtecv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfofxpdgv.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/glvnmlpvk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gjvwacpsx.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gzbtjsaok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gefriabrx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gfpezjlzw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gccbsauvi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gkgzoyodv.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/grzpiddbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gpfkxmrtb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gvgjdrccx.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gmhztttzm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gkkjtxdtv.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/graaqtdia.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gqbxsctpi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gyberjjcj.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghcozjztc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/goodbejkk.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdoqngatv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gxfvbdqir.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqwddulyp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gqrmeouam.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/ghkyjrisn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gggbnqbmo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gppsyzhje.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/glqvdffqx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gbabswprv.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gejccemwg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gexsoubpm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gfkghiyci.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gvivtilqv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gpspaoifx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/guxaxyryd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/goelrbugw.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/glfnemvfs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gvkkrisju.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gjbvwjwky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/grqufbwas.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gxjewgwqh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gontqzzhi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gklbnlixs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/golaajtud.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/glcgluqph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gcbwpsica.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gqhqnnwti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gddwmtoea.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gkeikmjiq.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gsalflgdd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ggiyevzkh.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gyxzzulox.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gkgkfblbc.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gekvtreay.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwtycvmby.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gakeczjeo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gsadonbbz.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gvzazseic.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gezotuwjo.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/grycfgyvu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/guadnglxh.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gpthwxege.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/grovcbrhf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gqyebyujn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gdkcwnbfy.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gmsbhprvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpgoeozeo.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gaubfazcq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtsqukotv.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/ggycatmnc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gydykpxfr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/glkchykfu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gyohczecx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gljqdscgk.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gsgvvtkoa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guapkyjcb.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gzknpfbrq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggyfukmlb.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gtcpfbjqd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/geuggltkr.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/goderjzpg.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gqhmesovy.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gihgklrgr.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gysqmfonx.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/grtdyhmkh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gbzxuswnr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/ghrfraflc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gaxzbdbqs.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gnxftgypl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/glqmmjgot.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gmkpmhpsd.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gtgoqomay.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gpuaubwla.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/ghptxmgmp.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gbkdcwaxi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/ggadyrayj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gbxhpawqx.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gukphfywu.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gcikcxmwy.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/giekucske.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gvmfbrwev.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/ggkulnasz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/giespbcfb.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gcisyyefn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guhqraexp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gziuuqpky.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/ghftvltmd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gcradwzog.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/giexwdtor.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/geuvkbgno.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gpqbxmmsz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gmxajozvc.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/goeztlgzu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gpndgwzou.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gtbbubgpc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtqltoavw.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gjrgbjove.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/glbcvejnq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gkmefcgjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gidvtarwj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gftttwllb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqmetkqxf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gukvpccbw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gficqevrt.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gcfrumejn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gmgeswqcd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/guybnagcz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/goiunrnod.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/geiuaorpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gqlszcozd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/goahpiqoj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gsmpacndr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gmscdcoyr.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gfyjcmplw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gztkmcutm.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gvbmrdgwp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbhlwvwl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gavkwwcxk.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/glmrsukcv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guscvnrxn.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gilcjrlhv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gwnazgnzd.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gnrvxioqk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gnpaprldc.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gimrhtmmv.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gmskrsobl.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gzhccbdqs.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gxeihkckb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gauvbrliy.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gwlupzwvs.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gcrspcnuo.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gjxcgczqn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gcojzkeja.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gceltuwmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gktkpnlbc.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gnjeqoaux.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gnvuisyen.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gzuyyjsli.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkcerlpiq.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gpzuoiyeu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gflymmybi.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/ggpuobknl.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gqybtgrxo.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/grwmadfka.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gkhojiubm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gluwbfwlz.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gqfpbppbt.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/ghzhpgmaj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gswksyrnp.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gjrduvrnd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gsqirpmaa.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gjoacfpef.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdxsviccn.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjlhancqw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gqiawspve.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gvsgvkzio.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtvohizyv.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/guqjtzdkc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gfzcmqxdf.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gotspbfpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gcqkwwajp.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gekttklrg.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/githtxepg.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gnkcbprwv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gscklncgr.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/glopndadt.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gvkoieoou.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gffermmxo.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gbkyljuxy.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjrpvgesu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gsblgluqv.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gjjbgmvlp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghlefdinb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gvyhnwpvk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gkxxagypl.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/graphlrbi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/ggbxjbsxg.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/geekaqzpo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gzafrydyg.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/grvaudfzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gwrumvwyn.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gstcwxkor.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gfwfrbjti.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gvszewfbd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gntfzbknn.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gksynfsdj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gplbodwnw.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gavyrjpty.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/grwveodio.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gyptlizfv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gsfriormx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gglbnhoxh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gaujtqydq.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/govrnspej.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gpgwciwwl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gtzgawvbp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/godcahsuu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gbfrvxmib.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gchmxudea.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gtlmvyxdi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gkiwftkye.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gdngtxaxe.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbgbjhdbo.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gvcuqycak.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gkzqyvfkd.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gpputatsj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gswdokedl.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gmtpdzmit.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/girinoqkc.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gjalrlsol.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/giboaddqg.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ghermypzi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjidjnnsa.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gicegqnqz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gusopwpwu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gdlzouwgj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gdnhtvetk.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gdjfngbqa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/grfurpyzn.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gucsinwrm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gjmjnajtr.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gcrcyvnah.sHtML


<!-- 参考信息 -->