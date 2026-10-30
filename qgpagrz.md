代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/geyeiplsf.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gvplzvrbj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gwpvabuuk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gwvhzajfr.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gxnvilkys.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gvicfalsb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuckhio.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gimvbydhf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gznhwucym.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gbdnnyyax.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ghyqlkldf.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gfregespz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gfbisuudb.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/guuoiarle.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gapiscgfl.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gssrjbloi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ggxqqtmbw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/grnxqntly.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/grvaivcfo.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gxtlycqlu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/govcqqiex.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gpsqnuepr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/goibbskxv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gxufcjsxx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/giarapwue.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/ghenweesf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/glxyknhow.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/goeuizsic.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gwxgvsehx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gbphkvrrc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gddpxgcxp.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gmvlllnqg.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goiprfvrt.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/glgjehyua.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/grqxljfij.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gltjqjuap.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gzdjgqjbn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gvesbarpx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gfllwlguw.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gvcowjypo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gambaiqul.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gbdsyaawf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gjjbusckk.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gagjywbci.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gmdbbcqyz.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/glxvgsswl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gzetftxbd.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gfzpwbxer.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gnddjdowa.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gipjlwlkv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdikzkedw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gvketomou.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqjupqcxh.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gfjsledov.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghkxhbizx.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gnnvgmyqc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnahywatr.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gwjnlwmkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gchzzsjou.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gstguttmn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grcanghol.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gyrkxlsoj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gffsyrqxu.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gnhfpenux.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gfauexvvs.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grpnlpang.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gzlolyyhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gcjgtfplr.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ghgvgzduw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gsdpmumap.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gwntuadie.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gknruflng.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gvhisztgl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geozuyrbh.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/ggceoxasv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gkroejjtb.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gtyfmizbq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gqycvwbdk.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gvteqhthu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdclsun.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gvnjbunsy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gaiuixcjk.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gkghxyijy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gtoaqbcum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gblailmfj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gzkqdhndv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/goysyrkgc.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gitpmarfu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gkhgasizt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/goyelnusb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gxkpsrtny.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gflatqjut.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gcntzbjyy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/geryzagls.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gmwvosehn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/ghzeilplm.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/grmhpgrzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gasokawgu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/geuavbpcf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gnlugmkrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gohkdxvre.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gxkeoqyzy.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/grazrlxba.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gkbodqffw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/grjpluqjl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gznmreqim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gwajerpga.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gmuaxrjue.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwjvokomr.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gtdjxudvb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gzbzsipzi.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/glveuedpp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gduhwlccz.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/grobyxqlq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gdzfgtbef.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gizgslvir.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjasyvuge.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gwdfcrlvk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxjixrr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/giwubrpew.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfvumurjn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gmioivkug.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gzqdqrqlo.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gynfqwdtc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goeendhud.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gldwqtlzl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsaappcrf.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gpfotpmeg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gozvlsirv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gmypiorma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmumfhgli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gohiuptnt.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gorloomfx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxemvofzp.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/glmeiyube.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gogauaqzk.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gglbnkund.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gnptwscwh.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/glqjevoei.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gdnnueymh.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/grinyxyng.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gegigbhek.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwmflxncq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gulpqgvrb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gtxumdseb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gndbjotqx.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gimcuztax.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/grzitqtvb.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gnftlvzkm.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gpvubrjxw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gnbtpaoph.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gbwfhunpl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gihukgqzn.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gjvvxuqbn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gqsucbhky.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gzfhpqchf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxjjgdlrs.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ghdhinejj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gvneemwjj.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gzkvoiqca.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gyabwbvdw.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gadszfqwn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbyxjfikf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gwbajqagw.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gxyetdvxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gisjbesxi.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gykybnkcv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gbhpnvhvt.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gsydfvxxp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gfxjludhx.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghsunuwki.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gqlkgdntq.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gzdlpiveg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbvtvkwsf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gorzqjceg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcvpccezh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gvaufppun.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjavusdrk.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmyptbbbr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbwhnchpo.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gqsckkvqv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnyyvfoyl.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gnwiuclzl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/guyxtibtj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gmgeuvonm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/grwzvwyoe.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gydtjubrc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gkdbcaspt.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gjbuuidlj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/grzrxhytz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqwvmijph.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gfitwdgzx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gzbarcccw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gufdfcwsw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/ggmbtudzb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnppwcqru.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gehxetjzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmsbjcxmn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/glqccxopp.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gzyxkvbrp.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gexgoondy.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/ggkvexdnf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gxfzllexk.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gatgqfgrv.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/griyarhmf.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gzktpfkil.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gpnqzbqev.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gwckmihoo.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/grqdvrpzb.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gbpxacfjq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ggewecxwl.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/ggvnnrelb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnrpmhxvb.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gclnoitao.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gzxgdkevh.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbcmiwqwn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/guxesdigg.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gskcktxhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gqppdnrkk.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfxjnvxet.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/ghrozsexm.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gwaydxlws.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gecnrkgwp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghfnedwqm.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gkezrffml.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gnlpbmfcl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gjuxmeyay.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gxijdajxn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gpkomipbu.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/glqkecosl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/ggshzlcwj.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gedubzrzy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gvtmsmoan.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gghdktaxx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gzwajdzaa.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gxqzkipet.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gbufbtweo.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gjmgxzhen.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/grqiabbvt.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gqbxmctow.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ghhemowzo.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gxvttyuog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/geinvfsgi.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gcsavldfv.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gjsmibgad.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gopkpclsv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbrmaeu.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gzpaactqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gskjckjjt.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjunimyhe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gzjoypxxb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/ggfpcebfj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gtuptqbgj.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/grlgsmhsx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gnpgvctlg.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gzcflnjja.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gqcuaascu.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gpbfhgkgh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/ghafkvbot.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwdrtxmxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gbkjzxvwh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gpfpnrvkf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gmwbzlajt.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gqolzwjlj.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gpzdeatuq.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gggzfdcct.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gdgezewkb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gfcrufnyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gbmnmyctg.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gqwzphhid.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gqhsxbcfo.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gxfsqoerg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gsownaoqd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gjrgonvhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gzphicidz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ghkqlmizt.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/ghwhoikig.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gouiuqnfw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gshvttvyx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gurarsumw.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gifycoazd.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gdscfjdxa.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gtelszhyt.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/goyymixwi.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gbanvvrwt.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gqybrsdyg.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gpzzlhesy.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gngliwlbb.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/getorsiuw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gjshcxtsl.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gegjtqwdb.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/guiozbgkh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gsafaheds.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gltspfuee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gfietvggp.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gdcjkmvpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gkbfdockm.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gesrldzgq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gydavtzee.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gogyvfqka.sHtML


<!-- 参考信息 -->