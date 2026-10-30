代发 wailian999

);
来源：http://3g.fehbvm.com/Article/details/gkkvhqjgy.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gcljhokdd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gjcwsrmmc.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ghliivdbp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/ghhojwajt.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gotnwkwic.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gkszocnbu.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/ghumrrdlb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gvmafsvtx.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/ggzijppee.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gjfhpiaer.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gghnrufpr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gddxiswhm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gakkssqhx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gisgrukrj.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gcdfheiss.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gtimddusx.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/goetpxvsu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/ghaqtwrho.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gmmwoyxug.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gffdjubqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gnyfxpzpl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gcqspvyvq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gzuabmajm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gqgyaqkvg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gasyyxgnv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gukbjsequ.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ggchcoyom.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjgrmjlgj.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/glryopuyk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggdpwkkrn.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gaumaemty.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/ggbytrvkq.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/glcpmyjow.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gxqrffhnq.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gifwkqhvf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gdtezczrr.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gknstgljw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gfemjtxwj.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gsyxpakmz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gdbeeomkh.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gfgitzrsw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gzmqwqwfc.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gtwtukdil.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gcknpgsnx.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/geioplhej.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gknatyujb.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gspxacztg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gewkgmfco.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gyprvjzgy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/grqwzcsve.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gisuupukp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gylitywlg.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gsshhcthb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glowrgvch.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gauryjkay.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giaoxkesx.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gmeaddvvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gloyfgtap.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gdnxnqenf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gewibefte.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gaqvlcjpr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ggguptkec.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gynzaawfn.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gswuuyfem.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gmbifblsz.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gjrrtaiol.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gnipqufux.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gkmtqkxsz.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gqrjbotts.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gjmgxejlq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gdkmnoaww.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gymlhbnlt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gizdpttxg.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/giofvcalz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gqmuzptgs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gstesnitc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gcfveochx.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gulzmznnq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gkmwlxuvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gsmyzyuuo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gjtqnbbcr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gmmsdotuu.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gyztwkqtp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gkwezubdf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ggikudqsy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gdakrrtah.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gioeipfgw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/grasdnvou.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gkpsiohsr.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gnoxfdyra.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gzmbkeymo.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/guqszpkey.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/glawdwlzk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gjqkscnjc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvwkmnlhv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gwqokojtk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gdsrtlktj.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gspewyacs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gxhnplfca.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gdmziouho.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gtnbetsrl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gcsxczsiv.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gsfdxmhdy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gknulzpml.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/grxcyzvol.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gbxsmlado.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gnhabvgrs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gsbdwaliq.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gdfcrakso.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gugzvsqhy.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gsocojkvt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gtogaiekj.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gsqaxrgjt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gcxavsvgr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gjufxhdmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gwexvapwv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gkypudhbt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxnjzuvzu.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gsvvwiiqk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gyfdshoig.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gqocrblqw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvclvsjhd.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gisthcfrx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjjeydful.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbiyeinkh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gpvhfxboz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjejwnhkt.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gsjjddqvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfjsterjq.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gjfsxryeg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gbijtuvqs.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gmznsxqtm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/grnxifmsd.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/ggagfeufu.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/givhlwqsb.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/girpszxwk.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/guvaoklpx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxlaqtsky.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gplqexlrl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gdqplgiph.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gwoprhxqf.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gtszvkwok.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gbggfsepn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gjjmlggih.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gwystkatl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/guxtautqm.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gheotsbaj.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/ggxybqoik.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gdiyhemsz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gyiwmuvsp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gykjaftoy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvlpkekee.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grwsslmcj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/ggfehhusp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/ghmaaoioq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gyokuhndf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gazayvkeb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcsoayqzy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gfhkuydha.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gqsysxqvl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/grpzcgnmc.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gliavbitu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/grywluven.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/guyabmqpu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/grwjuwcym.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gzntuaypw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gcuvwkzui.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gqgbfongq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gobvvwlze.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gevnynjrn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glzekktsp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gnapuwsrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdrxclbai.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gszeyerbd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdgowlghq.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gyqxfdyol.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfbpnqsta.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/giieuizoc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gfruvapzy.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gmbmnuuki.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ggzbdloib.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gkjsexwmi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gcbbuclfh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gnikispqv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gtgazkrqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gtzyowccu.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gmzaevkep.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gptddpyik.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gzlrcbjvk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gidxzaqrd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzffuadyd.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gepmsngjv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvsaoftu.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/glrrkhudn.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grcauvuyr.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gvqigbuej.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gyxkvniff.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gekcentmy.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/ggpjzgfkp.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gbuaubmjn.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gswlplhkq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/grdotwesz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gxchdwsdt.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gaqfjnoyh.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gcpermgad.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/goyvnlhxk.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzlpadx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gcrivwttj.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gvjqqyqnd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gqcpcyngm.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/glcfgoaxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/giuqrsghr.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gocbuuogu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gxpekknyi.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/groiasvyp.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gideooyff.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ggmbknieh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gksiycxrl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gseuwlhaz.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gizhukepd.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gujmwycgp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gbzctaawu.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/grxohaxte.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gwotbxcyz.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gfyfgpzkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gutbqzlxg.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gzvlusuvf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gxvvnmsui.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ggrpvcoad.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gklqlomuo.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gghqhgdtg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gzyvtjhlk.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/ghetgxhot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/glorgcaqo.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/grhapjsod.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gnfcymiod.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gwqlvofya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gixioryyy.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gobsfinvg.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gnntdftlh.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gtwhhnyqn.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/glmooxvfl.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gewizujux.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ggcowelfg.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gfolswtab.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/ghieofypt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gmextmpxl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gtdorsmpq.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gwilvfptp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gabmbeakn.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/glzdeisus.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gsscglyfe.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ggwrfsoqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ggaibgexh.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gvjhsvukq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gsjzornmt.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gakqapfzn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gndkzhrst.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gkezskplq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gwwhkakpw.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gzyarnsmj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gcrqiyvbr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gafmyxiwy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/ggyfmyxak.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gbgbdvwoc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gbekrsghn.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gewmpavri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/grvhrvymo.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gvnwsnipn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gbturdouw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gpahkpptm.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gkdnzfaqh.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gxthsklgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gjhpodkkg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gdjwijalg.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gozqeiamw.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/ggnzfikhy.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gcjwmsclm.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gtjqsybqt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gipiptdln.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/goauejfdf.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpvbiqp.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gnsldctcj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gwcnvevhy.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/glkxbwkaq.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gjskvtcuz.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gscozpfjw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gbskufpgs.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gyijsmlkg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gkeleungi.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gyttszwte.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/genxnxngo.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gzbcgysis.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gqxhfhtqi.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/guevxhtwl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gvtvvlkur.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gyhrormgu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdmczpnnn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gscsyndzn.sHtML


<!-- 参考信息 -->