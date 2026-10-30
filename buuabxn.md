代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjsogvbc.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvdhhxfq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfozcywfe.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxpyujre.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpxgrxfj.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvesnlhto.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvklmly.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzopzgbpf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwdqqzxw.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gdqpnudsi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpadpzos.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/grpamdpkg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedncfkbo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ggokokivg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgftkwvd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpskfvqr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gluquqcbq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gpldinorm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnsafolk.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/ghksnjxxi.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glscekbsf.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxnlmzeg.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmwsuisep.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzonzfz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkewwlqew.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmxiockg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvaoqpoj.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhdxklg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gyazxkgyr.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcecqafkz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grnjgpfaz.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/giusfmutl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqvptvxm.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfvuuix.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqxeomns.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdhtjxvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdritexf.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gztsvwjqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkfcprxy.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/giyhnbfnm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhuqpsps.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/ghpdzjhcj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmuppodi.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwqcxnoz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndsssuzj.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpijcnhf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/girpxotzv.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdtlnauo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptlwnkde.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gyopaimnq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrzyewxp.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gacryjnuu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzvuvmd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffeejqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqkytaty.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gahjxifei.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywooqipi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujeuque.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhozpqrp.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gnunfjrew.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gukdrplnk.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwpxjutej.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcwajfhh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/giodmnlec.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpschgtiq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxyeyynk.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gajpopfdv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gsktrvahh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzwwfuxy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/grujosmjw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsifhapja.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsneeko.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaklkaxnc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gcmwfmkrp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcvkbtsy.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gaufyvkbm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/grweqeqpg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawpcyjh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswinacv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/glunpcddk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpfnvchn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlqcmokr.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmqlqmvg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gosntuoox.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gutemggve.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gketujmua.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gowwcamca.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guclgtwgj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpemnspmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfcahvkpl.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/glfzzvoxs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuvedygn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbwgqpv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsapjljn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/goaktxfcv.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gwxfqwlxl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdfuhru.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfakauir.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/guqpqnlyo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjymkdcg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnfvncus.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuogxabe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjglotuc.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gewpfkhbz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrvukykz.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guladgmgd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gtywoxgjl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevonknl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gmauqnnto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gbigmdpft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/geiwjknyh.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gogcbllth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmesijgue.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyploedsi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhpotbyw.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gpqjuymlr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghcxwjvku.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvocnazip.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gtxuzdpyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmiipcka.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlmwwrwy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgzsomn.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdylmnmp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/girylbnet.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gckbnwpbj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzzfrefb.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjcbbkrs.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpdbiwkv.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhnterf.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gzvnzeqhs.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwatbvlbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcqmleot.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdcdvaav.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuwfhxqy.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gtogiklfc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnyopnme.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcexlfbym.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gpxingsmf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjlhaajm.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwitowim.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbzgpdc.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/ggylbffpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gdakzneck.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbzfxpg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrytcmz.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gbznceaje.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsrllgx.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqnfkuu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfrhbqv.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdksutkqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxlyriegs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/guehusdhf.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrtgpdzn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gffkwatkt.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnfvlrgv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/glhomwhyd.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjeuakvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbtdimcf.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/grfkfktjy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsolcqoz.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/glgvlyazn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkprvkvhm.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gspsdovnc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcrnchk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhzczgm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdcujcrmd.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjqpdceq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glqmqhahw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gglitgvpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvztxfhhq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowrrimi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/ghdukvpgj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/ghmcglkph.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwywtefn.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcdzjrno.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucvtcell.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gijpqyyjj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhiljnuc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnmkxdtc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gfesucvhi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gguqvbcnq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/guitriiaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuibjayc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkhukneub.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/guccqiyhf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuvodzxt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvecfrrvk.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycarmvbc.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gottmfvcb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glemsgsyd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwwykbym.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzbohqxv.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gitakvoet.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuiolymc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gtjhgiqez.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpewsfxsr.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grtsqmgkl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbsxzxo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwouxzsib.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmrjvddvh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszmfzvuy.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorjlojxq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzjsygmpy.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybfqcjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzsxuiccq.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghszwvemb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gddxqnqpi.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gqvoovkes.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gaetlgczl.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxeoskxk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gozraxrhj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcigzkoy.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gphczyubc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwlbeojk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjsycnk.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkukouma.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbznbkzdv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gnbmdjgim.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gywfdppbr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujperdlw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgnwxmq.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/grirqwvpw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghenjxodp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpvdvfwo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmakkdodu.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gogylqmyf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjpwhbqu.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqawdzaqe.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkyqtch.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gtmuxzmkm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwqlwcjan.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goewjitdu.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbsxrogy.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbruvki.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcmrydial.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzeoyxsyu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeyudcaw.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcwyhspms.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfbalkdwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgtuqmlb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdgndwaxd.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmjibei.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ghhrhrgul.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabwpkdbm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthvkwmrq.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpcjrkxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteudvywc.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwrmhbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsacwjvrr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevrnynw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gpcerdwtd.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guzvqppho.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvblpypv.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gpmtpyytj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsfwkqof.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ghhnonzni.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gjmlwdrle.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqxjxfo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gaybrqavo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoxpmckz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gntdmqwlp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjpewsp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxtywjdg.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmafovk.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwwbobmk.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gewljrobo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbttdwgp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytduasz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqzklssc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkygahvbh.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpjejqeg.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggayksaoa.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gyrlvsoxn.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gynklrdgb.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpwwrxazr.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdvstnsud.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gymcsdpsp.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/guhmxqxyl.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gmballmwa.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gcfsvcgkv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gepryhqdt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbfrcas.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gxscqhgob.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnpurpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gexhngbcj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfpernnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpbagrylw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/glqtorvrf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gtrdspukh.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdmzusngc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkazmobuu.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gryuggzay.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbikcfndj.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcicske.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvncmstpt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvhfyshw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjssayd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwcanbik.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gomavtnas.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gkprsjvxq.sHtML


<!-- 参考信息 -->