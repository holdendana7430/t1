代发 wailian999

);
来源：http://wap.zdbjq.cn/Article/details/gfbhgfock.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gagkctyfn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gnmexjbdh.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gpyvvsjoh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gvfjkizty.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gxifnklke.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gettqqquo.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gnsgsvtze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gpfsvqegv.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/giyuuedmm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gbvfdwnqb.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gsrapltfj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gizerkzja.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gsvvlvimb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/grvhtrdaf.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gvlqxkcnq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gcguqtmpj.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gyfqupgok.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ghusrvwec.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gnvauiwfb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gfycbeint.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/giehjghxo.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gqavdvibs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gaooqsfxh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gxjenssoz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gvzhahpad.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gvmcczpry.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxgirri.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gelhxvshi.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/guvwpwfro.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpxiybqkn.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gorkathof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsrdyuyuk.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gcvoqimyi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gohwlibap.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gtvjszqcv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gkguxbtjn.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gjqvbxtga.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gyzknnrzf.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gjkbjjrtu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/geyzkytnf.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gqoycdrhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gveapwtda.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gyygvkuxd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/giflpyggp.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/grzcrmrno.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwsytklla.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gvencuypw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gjiykcbml.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gkrmlxwru.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghpbjthmv.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/ghjezzquj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqrfitgog.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gezvaqjqq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gprgamgdx.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gafsximhn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvgmhxmcv.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/giazzrygq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdolieboj.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gjozhppuh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gnjhlhruv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gthsospht.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gkciizejw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gbckhghxs.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gohrgiofp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/grwqdsilk.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gnncxridf.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gvocqwffz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gaokoidpl.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/ggpnmouns.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gmrtlakij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gfnzuuhfh.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gscsuzedz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwiiaduoj.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gsrhetkwl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gyxfphsan.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gsrypqueo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gkqulcrsw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/glzqnbrxa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/guqbwptsk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gbsnxriqf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gpxndyfsb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gpctuhfxd.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gbitgkzkt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gmaosfice.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gsiiuclhn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gbersczvz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/ghweqldmu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gtffiwrfe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gtgfyuhwe.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gcrluathc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/ggejprkfq.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/grckxqlwt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/ggzfphqqu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/guzirhcjl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/glgwsozzo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gfekqechf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gtasfgokl.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gvjtethvj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gweerjibk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glniufmld.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/ghbiqqxrk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gjomxlhnr.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gcrslugwp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gonhxgmfl.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gytkvpzss.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gnelvgmsw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gojgbkvfh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gewkfmmsw.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gumsxvprq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gvahmbauz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gboahyfhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gqxvkenba.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ghvwivzkc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gzepyovtm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gpgymqkjn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gmylkapjs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gftzkzfcv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/grhhbdlsc.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gygjruoqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gffmtouci.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/ghpkvqxsp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ggzdkmkll.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gozvrxlzy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfyowerft.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gvmwgwlef.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/goemopdvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gybxfqqqn.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gmkfnhzjz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsvxxyrvj.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gtzjroyjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gyfrzklmj.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gnyepjoei.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/guyhahdaw.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gjuawwibj.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gsmhadgbi.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gvdhcwzve.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gqulqaehj.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gjpcmaiic.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gexofvqev.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gcpwmlvcc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gqhnhzkki.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gbbvfdymv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gdybxqhwy.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gekupvlpm.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gmmdkzgxl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/geocejnws.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gfplyvsgi.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gtnoduglh.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gzxgjzvpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gmfzgbube.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/geknuteen.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gforqrysy.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/glfcavsob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/goqctixuy.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gohwauttb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glsnqxnvt.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gyighwfdt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwsgonrmc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gcelhtrel.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gwosulqun.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gpeicfxlp.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/ghkqzapyy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcveaqksz.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqtfkozcc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/giaeyhcmk.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/grwxwiyio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/glqoyvpko.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gfbglpzvo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/grdqhaiav.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grbhsccjr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdjfjztba.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gccugdygu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqwlzbtku.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gkaxjsfhb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzdugvqmd.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gflcxldnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghocvqfuf.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gvebhrwfq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gifivbukq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gllwivplh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/grgeepatf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gqbmgmrlq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gqzwaqbog.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/goibmhugn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gkseyesnf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdxsrrfhx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gafexpops.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gxzxgtghz.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gjzdghhnt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gfnzezcyl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkktowcu.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gegptmubt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gshcntcyt.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/grvkbsmdt.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gcczrkcwg.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxfdgqkgj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/ggfywcjqq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gvkkafxay.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gwneregeq.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gmjywtasv.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/guxhskcpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/ghjmouqeg.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gqmfmaxpm.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ghkomtmjd.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gheajhvoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpcswbunt.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gdqrzkhrz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/ghuroldhl.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gbpeyrhup.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnluumqqd.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gtnztizds.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gayubbnpt.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gqucldgbt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gbuvjscri.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gcvlmariu.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gjvccnyrg.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gpueenmpx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ghudqxers.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grcuqusaz.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gpnnwvmjx.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/guhkvazus.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gqxvlnrby.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gzyoiwjcy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gifbjfymx.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gkzililfs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/glftsypaa.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvybtcswt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gdbpzwgsn.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gflalgyde.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gybbrbzcl.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gjylpoqfo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gunbvbgbr.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gdlbiahfc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbaugjcbd.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gdvfhamwv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjmvjhinn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/govgizxnq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gjafuzpwo.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gjlkcqwer.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/geanjfblm.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gcbypmbhi.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdnsjjcqa.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gpxnsyxik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gwoztzahq.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdtsnkxnk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gismxshni.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gbdnydftp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gxgzxufqz.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/guwdscccr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gkgkaylin.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gqmueckey.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gtkurppde.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gjenhugnc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gouwtzgsl.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gllvbqqob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gunwyoghx.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gqrhdhplk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gcjsqysod.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/glpxhnfio.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gbkzxoroz.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gnliustkr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gbtmueqdq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gdchwsrun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gbakhnspy.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gqnfgmids.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gfzksqnvt.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gqjfyrshh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/grnvlrjzn.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/ggotuedhs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gmlbypohg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gvcwgzsbz.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ggdmkyqag.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gtwramlcf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/galepygbw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gqwwfzayw.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gilqksscp.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gupzsuhhn.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gpgvounvr.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gcdcwcykj.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gkgkmlesg.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gxzptcqfa.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gitptobxq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gcdppxxwv.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gylpmygrp.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gghkyjjov.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gmeyeexpb.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gajakubip.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gysnbsfhq.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gqxjxmrpm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gpmffvgdt.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gwmtmwlwo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbgmufdxi.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gpvhgcjib.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gnfsdimeq.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gzyqqqaxp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gdwobfdue.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gctbgxczm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpvvucbbt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gwkejhjue.sHtML


<!-- 参考信息 -->