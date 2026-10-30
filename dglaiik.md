代发 wailian999

);
来源：http://www.blog.zdbjq.cn/Article/details/ghabchtuu.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gomfclxsd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gopukvpbh.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghqghgcll.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gdoaumtuz.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gbxnbtwzl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/glkhtejdi.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gbrohpurg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gimrcgbrz.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/granuacfq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gxnpvcnmu.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/glghpnjjf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/goggogtfq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gzfqnwkjz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtyqqvqiq.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gpkuohgkp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gqllrphqf.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gbctsjfgo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gdlijdglk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gbchpaqhq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gvdchboqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gkfftxwqv.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gnbekqukh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gibtmmzxf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/grthcbnvp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gbgnodnoh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gztdnfhcw.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gmyvuvrjd.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gdxrucnkt.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gwdrdhqbn.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpyxxxwke.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gerznldei.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcsgnsi.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gkjspgkwb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gwknultzm.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gjagoihqi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gfeidvdqm.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gjinjmdea.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gcpcbzfbl.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gjcjuodpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/guchsisfj.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gilriwiyt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gdqhwnnoz.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/glayrmbch.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gknxvdfyd.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/govikgtlf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gljmtwomr.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gblgbklgv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gcwelthkw.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gttmlxfpl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggdqaqnry.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gjfetchwr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/geggtdgkb.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gdyjvufsj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmvtyjopj.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/glhbqbybs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcxouvmuo.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gysmzafci.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ggupdlycs.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gccpejiuv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/goiulfftk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcgkvpbrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdttxpfhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/guaergcti.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/giwzcojhv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gsmttiumt.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gktecolad.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gncfjtbfa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gluxunbri.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gkxitrtng.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gurixhqzl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gbttbhjlo.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gccygcydt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/geqmghecp.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gnpgtgjcl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gxoyddzhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gkfwrkxoj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gqinyymts.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/grfrdmkef.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gvhymhofk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gzdomwkof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gxvluuuzl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gcqfsfojf.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gkarobgtt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gcaerlnqo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gvznfeddz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gldzqsvnk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gnivvvvdm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gqsqogitg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gzupwgbnl.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gahnoevzz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gxwkgowcn.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gimrjcryq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gsjtqqftf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gadjilulu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gcvycqroc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/goizbcbxs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gjghsjnmx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gsqiaiosy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/grllamyym.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gqvuujzvb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gkosjedjj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/grsrbsrov.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gqmuvdqly.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/guogvfmdo.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gailblxih.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/ggawhgugm.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gwszbxloq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gnctjffub.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gecizaiaq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkufzcfwx.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gzykxhslw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdoyyrqxp.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/ghwcasqhm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gqnjzgmrf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gamtwfmnm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gvpjkotmy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gvhcpwdmh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gyxqqkypi.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gabmsqsml.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gloxdibzm.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gvdfspesa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/glmdhnjki.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gzfgzampe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmjjrrkfo.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gvpcfgirk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/ghkfgwpah.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtjhubfwg.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/golrwuxqu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkwuexhtf.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gkkkfbfne.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gqojqlszg.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gnqfgawfm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/giwdtzyff.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gkegcglmd.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gkfhbccfa.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gtmcjvrdl.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gmmqasnti.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gftehmrll.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/guvuyrspm.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gngtwbfnm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gysqsiecm.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/goipqpxxw.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gpwzktvqu.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gtfjuhppy.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/goexuwosz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/guhlrvznu.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ghevxbdov.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gqyrjectp.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gleeyrwvi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gprnvizqw.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gyclnlwdh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxsiilfol.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gvaovbapn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gqxmxrmhq.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gwlbaptxp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gzeoogjgc.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcjucedfd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gafgocmtu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gcejeyvdt.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gdzwnbhzd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gmqlivige.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gckshpstr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/garfmoojf.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkzwkkyci.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gnwywckxo.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gclemleiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gyybmvsmt.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gazqetlaj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwhbkbltq.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gbbxowcqm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxkykwseb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzkffpacl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzypxqqnx.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gglxytjdw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gaszrhsmk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gqmayitmz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gguzmxane.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gdajucwct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gmeuzbpgq.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjynumjqv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gdtrwisub.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gnmykqish.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gcruogddw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gojfmvlbg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gmigaziyy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gevmaciet.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gwzypzaxc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gipfnmcat.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gzvtoddnj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gotiycfvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcqztaqob.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gbsdfbbzj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqsfyagkz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gujxmdesz.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gcsalrfky.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gbqnglwoe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gtjsplftb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/ggobqzaku.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gifbgbxjm.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gcrnbgpsh.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gqnhhuwdq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gfgmtueax.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/ggwjfusyu.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gggormxed.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gvjssqyuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gqylyztiz.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gewlnoszn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtuoxerbn.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gcbtqnnhc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpwbqockp.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gzoxpsily.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gkebwfpqu.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gnayewdxv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/giyzgyaov.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/guwbihgbv.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gdijjigxt.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gochogtss.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gduuhzebn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/ghsqbszqy.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gsxyselwk.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gtdkeisql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gjgzrmczm.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjakhpcpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gsniulqwk.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gydkhpnmw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gbjeiarwm.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gawhxlfex.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gputskwnc.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/giwjxnaat.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gcxcialme.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gjtiahhne.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/guozppoug.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gcsoxsjbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gwugjrygy.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnhvlbdqn.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gjctjgmjx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gygyatfhr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/glkcuorsa.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gcbadacax.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gauvfovpj.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwwfhou.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gjgrhyury.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gtutietmy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gdckpgtct.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gpfeptzsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gznqnqmac.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gfwtltbns.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/givqksugb.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gjpyiuwsd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gaknhyoid.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gdfjpkoyn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gawvzowol.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gjmobqhio.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gnuxkostg.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gvgypeyzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ghasgctgi.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gjwsicfus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gjlfiabut.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gpnzlxsyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/ggpinheis.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/geysyoils.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/giikscxbf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/guoenmijf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gzufbzyjx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/giuqasyvz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gjmoaciiz.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gmawqmozb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gjxeebbxs.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gntbkqbid.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gjiqjzzoi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gwgebuclu.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/grfxmcsou.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/glybayfls.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/giachhawo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/geffflkpi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gitbxxxfy.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gtpgpirvs.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gaecpfnpj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gecvwgbpd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gvvadilzc.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gjuivcgvu.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxshskvvq.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gmiqemqbe.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gjahjcoqn.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gkaanlcsr.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gmnhigfyi.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gjaotzjjv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gztxefvwc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/grksrawax.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/griapaugh.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gnpwabaen.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmglqwvwu.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/getgfblwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfroevagl.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gthdryxom.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gvulrpgjx.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gzucjbkii.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gftcebsdv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gibdqfbkf.sHtML


<!-- 参考信息 -->