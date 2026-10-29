代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/grqfgrpge.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gfoctluxs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/guuqfgtma.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gryxypjvx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpmnuyhps.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/glfjlnbrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmlutdlab.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gxvdktaxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gryhiygtt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gmifpzytc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gpxyboapd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gtkfgkrvk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gqsuwtjsg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gilwsqjqy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gdoqxmvvc.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gleewijoj.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/ghsubfoxk.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gawvtsttb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrxcojv.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gfkkgsrwa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkvhdoghe.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/ghjiapsxv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gyaucuism.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gzrwjobat.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gysibixff.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gmcxuyiig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/ggvsasprj.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gtsgzhtva.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/glogqtflu.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gueozoqpa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gollirsdc.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gxekwortg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gnjkruelk.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gkdrmmrhf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/guidlybfk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gzuwvsvxs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gurvxvaph.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gplcqwwxq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbdqyncwz.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gsrqdnwsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyntezlji.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gtzvgwlcq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzmfpbgop.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gfzsiqiph.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdijnlrun.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gmsjhnubn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyewzvyns.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/grlcjnagn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/glseoupbj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gwvxukzhr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvcxsbprl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gmoccqrwr.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gbijcdret.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gqblziide.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gydkfjrtn.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gzianpijr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gkmldzdbl.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gzymxceri.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gxbjrnnqm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gatbyutha.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gltbtewgw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqabcxrwt.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/guyqdccve.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/geqnrdbvp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gvsfwjaek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gcgffxdpc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gpjsmaiyh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gxtbxtslf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gbijuufdv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/geyzsnldf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gmtvvbwfn.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gwsrbpqme.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gyfqlvogd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtxlvmeft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gkrymqngi.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gkpdkocsf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/ggdyaruxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gdkubyitz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gvtogiqce.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gpmubiyye.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gjupzhybk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gsgxnaaib.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gbiwthwzn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gxsssbiiy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gpzwgpfpe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gmdbvhgnu.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gkfoglkig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gaxludgrq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gemcoeaxq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/geoeyysvb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gwrubnghh.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glkddvemo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gbpylatxj.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gwkznrbkn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggomuiqed.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gtjhahjfz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gdcyuruis.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gvnzdunmu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gvxnbvkot.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gjgcaevat.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gbvasobgq.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gdvehnvqj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gttjjvgsv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gqsysbouh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gbjmfgrdi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/glufqlxiq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gvkwslcge.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gwzfxpofx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gefnuzzra.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gwjkcwebo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gscbnrscu.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gpzfexnop.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grnlaycdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gqmpkfnvy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gphbxidlf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtxsuqsjy.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gepjtqkjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gginapebq.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gowolugzy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gagvlzhzs.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/geitldflp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gnkcqoykw.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gthdxitdv.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gmpvbgces.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gsvdbgmro.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/ghakmgsuy.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gqdknljzw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gfgiupwrp.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gzbsdeazs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gnqcjtxtr.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gaenxtctd.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/geqvqsobo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gntfgvhfk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gufoakvib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/guduqryka.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/grbdbglcp.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gbxqmyahc.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/graejlobq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gpqnrxkkc.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gdienidoc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwcmpgvr.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gnyzzpfek.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gyccryezo.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gyorvkmen.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gridwwntj.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gecgxybuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gowlsvfhl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/glxgfreyp.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gneeqzrla.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gmoriliuy.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gghhxtzvg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gevcukwxj.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gedrwjdok.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gxrfvtkby.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxlttdbkq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gcgjlitjz.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gjxneucas.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxkypxlif.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqqnmjcoz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcigptkcr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gdqehwqip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbqrvepqf.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggvzggeyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmpcpvyxi.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gkrcshpqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gemunrmnf.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gvrqjrbbp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/goqdlfouf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gxgrmpdym.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqicytzms.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/giwnvuwuc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gfbmddhcb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gecjevfad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gfjwtfzwi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gazwiwwxn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gpnixndxk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gkboluvpl.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gfbzxhdol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gbgywlhys.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzaxwfvtx.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gvvyizrkz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzkagisqw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gavnfczwa.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gsqlcpqnw.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/geuwcnxcq.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gorkclhzl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gzuatzqmu.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/geesldmnb.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gkipqxqmz.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gqvypteic.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gmgbxfdzo.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gavmhlweq.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gavhffinm.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gufmcbuhd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/goasvafka.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjayjvkon.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzalkimfx.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gziyqdcnr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gkabttnqq.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/grreoyyzn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gvyanrecu.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gzwyagajx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gnrnbmhxv.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/giuqrudpg.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gvxskbloh.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/grynyerub.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gegfwbkoi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glqdryxtz.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gelygkmlh.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/glqvrxeix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gkadaxmwc.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gndpnwhhf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/giyrzrkxf.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gapsrdicg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gialchgra.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/grlxpyoyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/ghxcthubq.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gmolkdpij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/grjpeehsi.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gjsmxcvvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gddjiafts.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/goiafhags.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gdaugmqon.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gxxksjubu.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gcllaehzv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gdlzianup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/goatsnkvn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gnzkdziem.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gogppgcwc.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gnqfxyqvf.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gafmbmjkb.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gltelxegr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gfuxeuqqo.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtnpechsp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gvhbaaidr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gnvliiffn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gnwonaesf.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gdnpuwqsh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gnmjzxibj.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gnlkjbfdd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzljylllv.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gshrtblwj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gpbtrgugt.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gzcnoqvsa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gkosdhxsu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gjoaqcqbe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gzjzmnyec.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gkzwhnimz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/giesudtba.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gnpphayox.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gqavvmuwq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gigmemlnh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/ggzearhcv.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gzkxqqxrg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/grudvvtwc.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gpswrmnej.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gtodnizmc.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gerpnnszj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gqttxfwoa.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gxrnppzdz.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gnkxwsfjl.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/giqviwqht.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gcmbiwvmk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gzvntbwsz.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gaevqaipe.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gomxylgfs.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ghljitdlz.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gmiiilyzj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gpsohdegt.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gqzdofjdz.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/ggrjowhyt.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gtnzrabvc.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gyrcxtkgo.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ghxlxeyva.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gymfkstnt.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gswzdkkuz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gbmwefwom.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbyvuzg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gsywzlnkp.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gvegrfpfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpjdczwwk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/ggqlzsodz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/grmiwwipr.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gzwpllcuy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gymqmyxik.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/glpgzmoqf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxljccqji.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/geykithvi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/goktmnbht.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gfsebeojc.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gnruofhdj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gngunsjpr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gkizlsfho.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gmjqtwlhy.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gosmkzbnh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gimqliytd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/givjevrnl.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gmuvimnlw.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gemqbwmkn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gkltksovy.sHtML


<!-- 参考信息 -->