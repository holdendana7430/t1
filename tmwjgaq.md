代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gqoeobopd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gmwskjgwo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gnspkkqoq.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gkdpdysti.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/goowkvdys.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/giplunxnp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbozncnwe.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gjwtgzqct.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gudqbgknf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gnpbmxecb.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gfmvgqeyj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gbglezwko.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gceknrccz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/ghjhrbuqo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gfycsbpal.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gvofpluir.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gljgfxdzw.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gvvzmzuyw.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gkdknxtcr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gcellkzpr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/garndnsuo.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/grkzvygvr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gpyniisqx.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gjzvajaxf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gfnykgtwo.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gnawvwzaz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gdsrbmugb.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gektsfoan.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gtlekgxxe.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gqfpvyrca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ggphporxs.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gmrdjqsxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ghzzjdfhs.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gnkmbaaig.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/glqcyhifn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ggreqsvlw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gjpsasmhp.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gchdmsxuh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtxatadpq.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gqvgammcf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gmpqaerod.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gtczmatmu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzwdkichs.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gundpwfub.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghnjfxijx.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gepzutgxm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gngliuyim.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gqqjuecmc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gprlbbydy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/glpevgthf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gdvouzelh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gskkwzdjb.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gejmewqkk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gxjghivbn.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gcrwdnsec.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gjausspip.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gsncjqufn.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gizplzodm.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/grbhtqolf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gcjxlktdu.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gfrofeqhc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gplodgwyy.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gpmqdytrk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gajeztvsg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gnbohlcjn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gclyjmxms.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gjmulyvmv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gsepvozdt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gwtlpcswr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/garapiraw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gygumgupn.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gevivsmzm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gcktddfow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/ggsitrfvp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gcvivkcng.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gugpmklwu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/giycikbcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gjdqmcljn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gucxqxtvg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gkyhpjmbf.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gehvxicwz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gylpczkqj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gxznvhehs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/geupqlhnp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gfncocumw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gfywlzlom.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gympjnpve.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gytagojil.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/grmdavvyx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gkvyygubu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gnuwcwatj.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/geqavbwpj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/glxknbyxh.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gicgobvfy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjlayfd.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gaqrrjqjo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gpgvgowdy.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gegyytife.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghqnlbzab.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gnhxrtebo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gzcttxymd.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/guzvphqen.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gwyfdimcy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gkorjfzwh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gevatiruk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gctgweavy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkarkkixp.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gkpqezuhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggngxnolh.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gdstlgcsc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjunytlep.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gdpuwaozh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdogxfvtr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gcceoyaox.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gwgsbxilq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwtodhgmc.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/ghgmspsda.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdnhnjvos.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gofzvdayd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grtqppdfl.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gzusvyjdw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gzvbiphzx.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/grkhdxxkq.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/ghnidkbau.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gtjvpkznd.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gsiejpbut.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gwwaxywhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gacslsnff.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gmevkuabh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gqcfetxva.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gkriomhdg.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gwhkjaccm.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gltolnghl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gtwaadjwo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnjtmcnpv.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gbzzbvxwf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/guzingtwk.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gsykdzkut.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gkpouwnna.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gbrsokdpy.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcngccdfi.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gdgbsrqus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gtrtkhfra.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gkappyevw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gzpikmcyi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gycqcxaou.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkdyurocu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gkczryutq.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gedjntjrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gmkyiisaw.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gckheiptu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/ggjdckjmz.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gtlbrcdla.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/ghhqdnhdb.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gcigwbeut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gmskxvtrj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gadlursop.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtxrloanc.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gehamxism.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdbzcbkal.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gowocjghm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvmyxcbvo.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gdjziiirs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzxdqiuet.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/ggznssjpx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkcdmgmxo.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gcgyzovgv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gnjlhyvss.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gzubjfjdz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gxfxhimxy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/grqomgebc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ggobpuvyn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gthyctpoh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gezbyieln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gteikoyns.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gmhkwgufu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/ghdshwlnc.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gfoulynes.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gccgidygj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggrkktlsg.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gvympcgzr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goyacgddo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gftylkjpk.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gvvokvtti.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gzvofqrev.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gkgzcipwg.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gtcyrzups.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gkbyfozzz.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gwcikzofs.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gvajrywqc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gtnuhujbf.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gapjijinn.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gqeyghtkg.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gsoxkuswl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwngsazdq.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjqlqzifm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmaqhoriy.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ghlbhfecl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnwhtuygt.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gdjzncegx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gwihvrkwq.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gllxiijfw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gdctapzwj.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gyqftvwee.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gxaqyqmcp.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpbyqpily.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ganicplgf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/glormqgdq.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/grntheoya.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gopvinynl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/ggrguffgd.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gqxjyxupu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gudqumeys.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gydckzrai.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gkuingpob.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkhshyxbg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gjasuiijt.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdvwcywtj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/grvlymzhz.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/ghcodoicz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/grnexscqt.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gldnqmzgx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gslnrnppi.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gspnxiscm.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/guzjvfgxr.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gtuxowrag.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gjcymbalk.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gwtzpwjlf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gxqxqrcxu.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gzxyjlzbg.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gsgdbqoeg.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gcevzxprq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gaiaqfhba.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gtcwsukdq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gwarqqssa.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gseukfznp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gtfsjwoym.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gxxqqoezf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ggrqmuswh.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gtjcxpawm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/glymiclia.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdoyggwmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gnyogtprw.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnhkdrnbn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gtqntigvj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjcpkkw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/guzclpotf.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gubizgorj.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/ghfaibvps.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gkfmfjkkz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gpbrxhpnz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gzlwsvaod.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gqaulplfv.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gykyhulsp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gmofxmrgk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gfjvivpkb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gcgzjkyin.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gbczuwfzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gcmucnhfp.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gayevrnfg.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/goxmmfizu.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gevefwmpv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gnsjhwahu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gwincxsrn.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/goffpneqq.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ghlsqfkva.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gonkauwxb.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gjvypkwni.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghubutusm.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/ghwsvkhin.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/grsgjkftm.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gubtdpdkl.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/grugreoni.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gdvetfoum.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gajhfvpbr.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gfotjdwwo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gweoqtpjs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gdziowovr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gjkiahbat.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gmsvdrkbu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gsajmeaue.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gevkepcrw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/glcqnmgun.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gjzrdgubi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gtqmriltl.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gjnzvaavj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmdfprwiw.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gxtatgxpo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gxealmdgd.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gsmvcbfkj.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxshtabdp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gstrzxsur.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gkmkfirka.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gsatyratn.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gbpnwsoko.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gkcxsrxkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/grnvzziuh.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gpvrceiop.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gmuzmroje.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gvajbrkhp.sHtML


<!-- 参考信息 -->