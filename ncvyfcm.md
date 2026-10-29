代发 wailian999

);
来源：http://blog.hesvh.cn/Article/details/gnfrmvfnt.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gcyxqqzzs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gbvkdjuig.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsimufvri.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/grhwgxrbq.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/glcrvlcon.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gutezqxvl.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gvohnkxnn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gxtndnfdh.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gmtzepllv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gsvaczgmn.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gjgnpldgr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gvcokeiqa.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gqmtlvnwa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gvsgrkaha.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gdpawzeau.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gvruegmiy.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gagddwbon.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gcfawprct.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gffvbkldu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gmgftrswb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gicmhrclk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gjssjbjse.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gqookqgnl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gcrbawtvy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxrxqxtao.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gnhkymdfp.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gmxdwkzgx.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyxqwnrbe.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gggglgauc.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsmvilfzj.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gxpwihtxo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwkzkmuxi.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gwzckswgg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gvdmgdcdm.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gpbiazowh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/glfhtrwyp.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/ghofkfgbb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfnhthtbr.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gqtcpgqxi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/ghncxuxzj.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcywkld.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gyvskhgar.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/geasecayo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/givdzayul.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gymrybfom.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gygcgoenv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/giivqzass.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gsaawlavt.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gictnkvjv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gahcbsfpg.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/grdlirqyi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gozyutykg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gctgpclpq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjzajltnd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gdeybgjpc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkfezqybq.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/ggjtmtfau.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gvpfacrpn.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gzljizcjm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gwhydumqq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gffnoaixp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmkqcrwsd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gipqfxush.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gmhyhxzvu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gqaxwpqrl.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gugeapiww.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gfjxnorgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gwaglteoe.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gvilwkpgr.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/geggkfdvt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzddbmawz.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/grusgxuqx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gcfhpjhxr.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gkzprzgfy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gpabtadhw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gbryahdsv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/geumzzlql.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gqcascwma.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gjlkbhcao.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gztksunre.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/ghxttswlc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gdfotnjsu.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/ghjgscgpp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gjujzvkln.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gdbuwkzvi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gohqdgvvv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gdocxcmmq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gcikiymmi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gawissucu.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gabphkijp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/ggjyjqavy.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/grgvcjotj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gojvqkpek.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gsdziwnzs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gquramqse.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/glskwndjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqifletiv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gmjvcdsdw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gitdcqfgf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gqngwqioi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gatlrwhld.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/glrtitkfm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gmbcaiprs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gnttreipg.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gqsqsyskp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gxylkbptf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gzbpenkqk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gonbyrrlt.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/giknkunsk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ggruiuhvs.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gvxtioplo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gkldhmexx.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzatcjtxp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gezkihtwl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gxnwbvvyl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gqllqckdv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gsdlbtouc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gchwpvtjw.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gltzovaif.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gigxcerms.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gzqgtcnpq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwmsbbpnk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gjdbfzohj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcwfdeezg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gnaujfwss.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gcqmykjzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvkdcynoc.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/glcizrkos.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gekklmxfx.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gnlaahbtv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gwccotwbc.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/guinseonx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gucmfafbw.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ghtxrzilw.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gfltmaynj.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gujcnsyfl.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gwrymsnak.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gadwrehhy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gppsjlogl.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gxyehwpif.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gjbceybwi.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ggvzjdofq.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gprfbbveq.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gklatmxyw.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gutzxuxwu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gdlftadki.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gfhggoyph.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gcnksccgy.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gbmawzeym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/giwuebrzb.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbyohnnvf.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gmfkrzfmd.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gzhsepxai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gsletecby.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/ghnnoemjd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/grqdumcnx.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gdiclnekp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjhfbodrz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gjnzjekel.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gnrdketpx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gpmgckpll.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gwgrrhpqd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gokjdpupr.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gjxoenjwc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gihqnyjkw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/grbsqsxjm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gnwgjpyeo.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/guzsghatn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxnedugjs.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gapgrfbxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gwstoovcv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gojolipwx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gllbwtlos.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gnwkhboat.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqttfhc.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/geuwgrdpl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjhzzkstu.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gaziidoee.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gqlahdxwg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/ghhbevmku.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/glrczpjhf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gxcpesmpa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/getialquy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gcfgwzvmp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gdpgpadgh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/glphtoogp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/grjgzusnh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/ghekkcwja.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gpppjxigc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gfwmzkgub.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giovkamnx.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gnoianxqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geljdxuwu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gehspwhpa.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/ghgevfaao.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gaftnptyz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gdhregaqm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gdjpcgnom.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gqjfnpldl.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gcvpfgshx.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gdivlvvpz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gtyciklzp.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gpsagnyao.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gwoslracx.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gwctxgqzt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gsmemzcor.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gcirutjod.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gocfwgcsk.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/guispsyio.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcloqduqi.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyszcmxrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtjyrxzod.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/glpfmszus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ggasrllog.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gaodinpxu.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gnnebvizo.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gbhbdjzks.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gwbojoqcb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gqssfncuq.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gjxjbzokm.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/grbduyxrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gyzbjudra.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gnnqyzvuc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/glvkvbcsl.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gghfwzkod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gpqhyfabw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmbynaywz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gjnwlxxwl.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gjusebnmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gdaipigjl.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gfyrtsdyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gqltieiim.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gzicgyfsn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gmjvdlmhr.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gpbxhssex.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gllkhkfxy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gedlpfrzo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvevxeakv.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gicaqtzbm.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gziqwecsp.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzgxynjqs.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gjtlzvxft.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/grsoxgnuo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gtohlcets.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdhgzxvlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/ghoxjqydi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gtzlmsgjr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/grsdhuqlp.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gxergqvkz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gictvqywu.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gsueyjkug.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gdujmixjs.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gcsulmdsi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gyxuoozrd.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gucuvwunk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gqavnivkh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggabizrbl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gwfzsjeye.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/giioyvyvd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggtkrsoja.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/glnruxsey.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/giywveoyj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/guxpqegfj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gdevcamjc.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gsitaiekt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/ghumlmlrn.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gjrtmfuwx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gplynripw.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gdzvxzvxk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gxcekppro.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfekqmjqr.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gjlgytsol.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/glxqiszzy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gytsehhdh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gfynhzkvr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gufrhvewf.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gnnnkyyfn.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gmbompdbo.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gjwzisaks.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ghrloszgp.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gemhoymwx.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/ghzaovskr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/goagasilz.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gzirmbkvo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/ghxwixrme.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gcccjzcci.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gzxlwbomb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gcacvuajg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gwdedbijq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gcoubrlqb.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gyajmsrvs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvtkysgco.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gbqkkbbco.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gauykimjy.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/ghbvguyqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gcevhkzmi.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gvtkfcjie.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsexozhcq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gnjjprybx.sHtML


<!-- 参考信息 -->