代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gtbgklccy.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gdqpmfbwm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ggphcuzgh.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/ggarcvgto.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/guvbuojie.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gpygpxhxj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gozoofkdh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gcijbimnp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gkwiowoor.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gpgbfvpvy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gqsliyqee.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmrsmvekc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gglnabdqi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gcwqfflat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gqerxchkq.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/goclyhiwy.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjkkamfsq.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gfrdwwfli.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gewetlglq.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/glcxllwdz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gsuvnrjlo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/grfuwudgz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gmdeqkxzo.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/ginsnovlm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gzbabzvwx.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gtegjokge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggrfpbnza.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gdbjlaoez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gtopikzte.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gvardkycy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gttwflnhr.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gvrgmmsql.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gmywdcqjf.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gectxkewp.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdcqjffbi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gltufdolu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gnokgkqet.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gislieiko.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/glrovkwzg.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gdvedicxr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gezpygpmj.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gnmgnvhfk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdkdmyhsm.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gafmhttjs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmxyfzuih.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gvwzzafvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghxscgupe.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gosqaqqey.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gfnecqpzk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gdepaegid.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdldryunx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/ggtrgbdqc.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gdcoscoss.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gyoyttrkf.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gdvyscsmz.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gamumqpkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gfvtfcmmc.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gbwkcqgjd.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gslcgnczu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gqaeaskdv.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gpqvsqfhj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/grzwnzjou.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxlnyiknq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gngmyvbbz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gauzdumkc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gnfgwisau.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gakfkpelo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gsbmfeemf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gynjwpdfp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gigwaexam.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gokgeyqgp.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gdpspjwdr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gtbnpzgsm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gvpdwzoty.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/ghgzskcau.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gcoczamgt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/glptrnaam.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/glktsrwml.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gfakaxsyx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gbyfrdqtx.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/giwppebnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gbjmvlsbt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gijsjpbcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gfnlkzhbc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gnypuklka.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gbrbcqdjm.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ghyddvuyg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gcjuacmva.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gbzmejxaj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/geimicxoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gapbyvicf.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gxwmgwacg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxekzzssc.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/ghglwhjlf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gbbcqjieg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gohazjkya.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmfoglmyh.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gttrcjqpf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gaqpgfkuq.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gquruarem.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/genhciofq.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/glvpgrduj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gshqeelit.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxouiblxd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/ghbjzpsau.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gvhansxmk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/grvsvdjix.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gtwommcrh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gceemcirb.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gfxqazyem.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmkfxzpym.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gzvyhgjtu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ggrjvzurv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gcnmprrlx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gwllggmhf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzoubjhob.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gmtoulvtr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/glohbmfhv.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gotsqjgwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gpwlxjwiq.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gdgrjcven.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/guywdnusw.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/giftwhfkz.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gunephkge.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gtfvpsdff.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/glfddqbpz.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gvrzxblpw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gtotcmjre.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gjqvxmhjy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gnvngaiyt.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gxlfciwve.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfczeecnu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gxaexlwxn.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gaodocnac.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gznquidjb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gtadyafet.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/glemzbrar.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gmhaggtda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gvwhmrdez.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gcipegikc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/garwhyuke.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gbhuguenp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmvipywkd.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gzdeqfmqd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gqmlgjdrx.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gbhqvxaeu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gumrqymbu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gihuiatlt.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/guayfkxxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gtfzrghqw.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gmvfvxgnj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcxflrwpm.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/grftegrgf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gmjcnzbio.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gtwxromje.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gerdxhdxx.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gaortvzuj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkrneztqc.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gekdogwkw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/grhghtpxx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gmfuotyqu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwekpaolh.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwumqlold.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gutigdafe.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gsjfmpnle.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/girpqrovp.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gelifwxqd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/goawsuzoy.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gvvmeudlb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gvrqanllf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gpgqrxtbr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gouktjnll.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gyotwpxqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/ganptztbo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gbpisasjc.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gbuvhnbbt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvywwfsze.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gyznvlpod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ggweunpfh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwbggnwjm.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gftujllzr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/golpnehsv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gbhgxnrwm.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gjxmfltmw.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gljtiztkc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gvxvylfpk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gutayfojk.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gradxnwou.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gmzxrhuyw.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/ggbjwrtdm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gwjgfcpqc.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/ggjczboin.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/giwltihby.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/ggpmwittr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gsowmrlbd.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gkzqsmhqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gyicagifn.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gbvapinev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gvxwbmyay.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gyuavxyhz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gakzbpbos.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gtehzcskj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gworlvbpu.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gulimnzjg.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gjdjjiuxw.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gyppbvimo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gvviwzhxr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gmojbzgyu.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gozcyzctt.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/giofptste.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gumhbrtix.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gdroaflcc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/grduqetdv.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gueowpjon.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwjamnsth.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gskxyhjfs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gvyaymawm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/geycwgvuw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gabigawsw.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/glujehnvh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/guoqnruwv.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gcsepgvcg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gosedlqmw.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gbmykdwkr.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/genmpsnda.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gfrsibjai.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gsdzollpx.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gvinljcah.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gobjttksi.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/goepvhjpi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwvygpxas.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcdzasagy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gqefytxya.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/grtcdnhma.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gxtqsdama.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/glqktoqqi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gosksgukk.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gsylaqjon.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gzuqeuffk.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gygmoiaqj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gxopvywyj.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/geymmljul.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ggsbnggmc.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gepczosac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/grosbtypq.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gubzxyjam.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gfhkcakjl.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gglzgfpkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gfypdaede.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gefgcjxar.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gebyqzjcc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gtatlqoah.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/guqpvforz.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gncxfephj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gogppryed.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gzkykvgxv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gqzolummm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gfwjlapem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gvnkqvsga.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gsumnwfca.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gixtsbucz.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/galgciveg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/giousaaly.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gitxlmddz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/glkdeoiln.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gxdyejcrj.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gxohyhpgs.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gxincvada.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gdsyiwkqn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvppfpahg.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gbtywkpwb.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gepgbhifp.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/getryesyv.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gaaeekcpk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ghudulewy.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnntzffsv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gyomwteer.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gnmlsldad.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gbzkombhh.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/grholcmyy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/ggvpjorkw.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gbmutwgdc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqgihhlml.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gehoyinod.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gpgoglhqk.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gzqnabdna.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtxmtvdyu.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ghiiterni.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gtspkezij.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/goljkwvuq.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gsgrzxgqz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ghhqgahcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gjmcqscks.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/grhdqvlsq.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gxxxeavxj.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/glwhlvqaq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/golmutusj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzwriyhjq.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gildksmuj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gtbsbhqfz.sHtML


<!-- 参考信息 -->