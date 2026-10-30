代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxnwshla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawusafx.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gpjbjwjts.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gnuittxqj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtidcvlq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcyepwth.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gypsokgix.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhqphfiq.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtabpzpts.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzmytvse.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhqapir.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvoedarhb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gziqzbcav.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gcijrlgod.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gftoqfeud.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlvholas.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/godylazhg.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gbeubkrta.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggxaoyplj.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghimmmvyn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdcceqkf.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyhvvrry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/glytcqexj.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzxycjg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbqxyual.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpdfkkal.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gezkfqjri.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/goeonttka.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/grlgyvzcc.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gpskqupga.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfctian.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/ghabybklq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlfsmyie.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtpqosus.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glkrlxweb.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gwfvjbwhi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtbaycbbf.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxvgkjlvn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmaacamd.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gfcgxwtau.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtycjlwcs.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpzcelcnc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhzsirql.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gifpryzfl.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gwwdxjstp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gftwavpeq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprpijxap.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgizorks.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gmrcxbwgn.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqkgtkb.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/giyamzydx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxaxbpmi.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gzpigncut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/glyezsnhj.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhuxfws.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrvfvodk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gglizwmav.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlttigcs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkkvxrmq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfxvurqd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpyobiihn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/guzlsqxke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gopvnmpnz.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjiyexfzv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gbrpxifpf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbkujkes.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdopnpka.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glgxjnoxq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gqembrpbk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/glwqnrkuv.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtlunmfod.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqhidxer.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gnccgtrbv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxesuyiv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxmevgjby.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvyxlvaku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gciharime.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsclkhhtz.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggfgtbhrp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcmhfxqu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gceqjbyei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gapatfhpt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrcgacmb.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gwwoqxtjg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsynwgvu.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltugipxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvecdjbcr.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/guhhjffgh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhwzpqew.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhedltbr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gogcvmatw.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gisnycliz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbncdzpvn.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gsdrneqmh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbpsnfq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszluebhu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjynqagns.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gnvwyqprp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawtrlgga.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwpktdvp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmswljuay.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredwynft.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gukcmevli.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnekafyx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklbczvkr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxyznmj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgbmpeoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhmwvggr.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxvyqip.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbtokhcz.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gqzldwchq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzopxzfk.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbicwfo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvldmzx.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvunkhvv.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkiwhrah.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelcdydsv.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtskgfomd.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghjzcgezr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdukwucz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gablawleg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gduubeqpz.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gejvhgafo.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggslmrfsg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmkuvrow.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhdrdinl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkywvlxak.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gggvjpwez.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gurxjpthf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauzonjf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gebgsomql.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeylainq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guudtjfzd.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/ggfhshtov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmzyuxek.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gidivpflp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gwixwhsna.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grzmbwbwp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppeuzmha.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/ggmfjohfm.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsisuikj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpsttjph.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gkmzanhku.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gumzgixop.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcpharpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkmxrfhu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrlbzikt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/guovqcyae.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimyttqvd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnlvehaa.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiehekvw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcoshbhld.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefecscpr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsjcnkm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthkindrd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmmaxfhgw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzrrlwq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvrxvigmv.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwhtdcg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxmtdygl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gvhykdsho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuzzrmih.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqqaihisv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmsxjwic.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndkcyil.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gokdumbfr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gefhhkkye.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvpumldw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gshnsrdbz.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gifcbeaor.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsaixruk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfvljbjz.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzqbqrlp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gahwrchzw.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gldlpevrw.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gqhbhhwmr.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbvxtdzd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnllrejfa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhshxmcq.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmipqyid.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhlxxgkq.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gohxnaktj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gdruhgmtv.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjereoczl.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/giyxpypqu.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyaovzmz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfuupfdz.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqehphusg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtdghmxi.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmerjnaqz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gixgcosbr.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdzqevqde.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdscshq.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhztmnoq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkniuslmi.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gjqccahks.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gpgcmidcx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guacynnqd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtseynzt.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozqhjfts.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gkkqqepal.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjrfftj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxntdyjtp.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ggsnczgri.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvxtbieoj.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gczjwccrh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvvrmadu.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmidtedie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gursvziru.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnbugqkvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gthecmgfn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gydmkvhpn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gomsljbiq.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzfkenlz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghwbzaerf.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/graxcyzjm.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gregqymjc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gytdbltdr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoxucige.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxijdrepf.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpiyffam.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ghhscrbjb.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyfwxfxuh.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gezmjfezu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsuyjcjzh.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaesrnnyb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuclmsfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gmbuspnbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxbryoe.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcuupec.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpgfozow.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gdqxpbsrk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqzfpxd.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/goczsmgjb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gbzcvbtcp.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrallsfr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glsxhobzk.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxlsjiuca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gwkriuowk.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glfdshdjq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnowvfqnw.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gtvienfmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpbogdpq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/glbyccfhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmlhfynp.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gtvarfldz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuifgrqm.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gakvteahj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gpfluvjlz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/govfwqyvo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/grvdjyuvb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfzwycee.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpvyndg.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gcbzjmpjt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqkenoiml.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfnymzcu.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gefykaxhw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpnnjrve.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnspvkta.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gueryahmg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/glyexjccf.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpitpwip.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsovziqem.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxtetxcwj.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwauetcx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvebhcnbk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnztyzcvj.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxsnxjh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqkruwc.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gfgfrukyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/goihiroyx.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfobfcolq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtmcbwpfx.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gejqjmbsr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/graluzgyc.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzliavttf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzefjazn.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdmmuixq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbmbjdj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gnrytohxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciopnsgq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbczbgsvc.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduwgwezo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwepscze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghklvifft.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfnkbwjd.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdsvdguq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwwpemqw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmjofhzo.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjgvdsaqw.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gqnpememl.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/glwnxcjuq.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gbaozlxrg.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqyffdtq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoiicxfz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqjkxcf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrroakyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gjiizqgib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gbfcugdhy.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwmroiaw.sHtML


<!-- 参考信息 -->