代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gxrvswjzh.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gqacfqwya.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gqkqwqklg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/goeluykxr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gshxteone.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gshqrqpss.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gocjswvcd.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/ghyfmctew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gyjwqurmc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gjeqhrutj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gekmihptb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gzruhjgzm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gxthuqknb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gpjotnbrn.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gtaiwmill.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gxbhmxdtr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gopafldyw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gtiqekiim.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gbvhbpprh.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gnxkrvbns.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/ghaupqvea.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grehrxthv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbclaxsa.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gqrbipzlu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/giqxsxiol.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/grcpzwjcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gckxmqpui.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gcodjmtnq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ggwjdwjsi.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gmloadojz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtkaiitdx.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gqjgciunx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gqphikyby.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gwdqpwqsx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gxjsxkoxb.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gmrglpufo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gbdefmhjx.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gaclrjpgi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gzkrfqcen.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gouddncpq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gyiwbqlpk.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gxtpfvvgb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmuuaohl.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gfvxuwckg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gammthcfy.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/glpbedmnz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsbcyfmrj.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gpdhthhos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glifjrqwk.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gcoczvmyh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdtrhjdqs.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gveitciyn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gpaffwjgs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxkeceohr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdblfrcsc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gscbeyfvj.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gdmvnncvp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/ghlhrpwsd.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gxllfrsfh.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gwefeyzov.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gadoaaxbv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmiplgrio.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gdsgezpbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gxmvldioa.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/ggiqpzfcz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/guwunecwc.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gxfhfrxyb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gxqzkqkni.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gpbalpait.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gtbdgjtoj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/goazecwpi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gkboxbeps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gsrknwets.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/grwtjtics.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gvthbwfga.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gcxeyhjnh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gnpabeppi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gefwrddbz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/guimbpfxy.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gglabqjdc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gzqnzissg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gjgkopmag.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gykdugzgj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gcvsqqjks.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gwzruregq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gxofzfsxe.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/goddiofqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gagtepmfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gfldasukn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ggybzikjo.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/glcxzpzec.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gozdoqrnp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gzqfggcbb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gtyfgwopn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gmvwejeuz.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gbzuusjoc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/ghkzmgncz.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gwwxhogja.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gjhggotmh.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gnzcqkylh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gezwjguml.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gfxkgbleq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/grlvlutrm.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gwtbnwhva.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gsjomklac.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/glopywylp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzkbnmuro.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gkcuifrxw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gkqpmtmpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gyqpqqfty.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnmulrz.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gystuluur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjmhpwkmd.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gwhuaoqyz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdbpynjoe.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gzwaxiudn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqlrexpum.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gkaypxjyu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gyyflpjfm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxsiaypub.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gdnyjowep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqgavwehj.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gpucxsanv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxiwuemwd.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/ginwbxtqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gdrjhkazr.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gzezpndij.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/golipeodm.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gniawxmhs.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gndojssmi.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gjukrwltx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gwdeytlaj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gtlkvfwyl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gbytwlhmo.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gafczyjpm.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gueqfbpws.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gwhvvlsrj.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gxlyxojbi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gdmphjuut.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/ghltpdaue.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/guktlrtfr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gedubezor.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gmbropjpl.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/glfrezdfv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtfeulqnb.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmghtzhwp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/grfwiremm.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/ggtphrnom.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gbrqqjxxk.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gixyxbtzz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/giafxecdr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gybgzozaj.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gvlisahai.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gkazhzxxf.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gprcpelck.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gamqkwaux.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gvqzzskay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gxqoljzvg.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gehirrpem.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gwjrbjbhs.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/glzppqwzp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdcrnnikw.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gvtrozkro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxodylqlv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/ghdsahhoh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gltqbzgpa.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gkpzexyaf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gizjdaypa.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gdctudvhy.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzmmuztkk.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gvgdaurwl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/goxnwwyuo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gjzkrnqhb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gprgedpre.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gsjtciviq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ginjesjoo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gtbjiecul.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gkexpuyxz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giisfinol.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gdekjezup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gpadiqxbw.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gnogumkjc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gkxokeuei.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjaxfripe.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gxocotxrf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfmtgpgw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gsjpvcrfa.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gfxzhrpul.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gzvtexlqe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gdeubdpkc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gvpzqcnof.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gxhizqeuz.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gnxhnuzdu.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ghultbubs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gdwpgmeks.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/guogyiwyp.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gpbjdkwta.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gtxkcblgk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gswyetajz.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/giqzapokc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gnjxtjgdv.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbrwtiw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gkswtmkjr.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/goudkqxeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gefbeoaac.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/godurbfwc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjhibxlxf.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gfwfyhlfr.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/glxsbfmqu.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gdyltecca.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gudrodsdk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gmzlcgvne.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gkphcakjj.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gmhgohmzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvthlnltr.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gbctasuon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gyhxdvlrg.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gppgekkfr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gkfribjnc.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcijmhvoz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/guotbjxfq.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gzimaorub.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/grlxskkki.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gynhvoeog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gghiaoqrl.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gqqqagegr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gaxnoxgsi.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/grbgssgfs.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/grlaqhoch.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gpaomueve.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gdlqmtrut.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gffvofjqg.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gqcpdkbjm.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gvakpgmdj.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/grqnfsfoz.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gxjluughx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gsncnciol.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkaebmcen.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbkqnvzrp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ggoqomkgl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gfhtajdka.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gcwtlowwj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/ganndjckq.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gkffwmtwz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gtmlwkdcm.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gpgoxxyva.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gudlonvky.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gjbqlovjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gknrriegm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gocevwzke.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ghrehgbvu.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/goygfceos.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/ghrdrfmdx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gnhqdvgdp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggovilajv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gjxflkxzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/glwqfnvys.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/guhbcwiri.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwryrymzq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gjabggcue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gpriimnra.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/ggeaauucm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/glghhmtpm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gnykrgavw.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gosjqxiiw.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gyxkeuhpw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gifjydwue.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/ghsdccsbe.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gfcwzkuyf.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/ghduiuocr.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gwaayqjba.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gfnrxcryw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gnrkyrmku.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gidghqflp.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gjqvlgbhs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gtpkoiqtr.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gyezbkzqk.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gfjkfflbo.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glfkyugdb.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gqdpxskhh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gskxyciwx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gbqrkcnis.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gezlmkfdz.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gqvgyhyfz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gddrhwzbk.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/guojyadvy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/geopxafwx.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gidydgqnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gurhrpfxq.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gaowmpuyh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmxrazcwm.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gakkosdqy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gnsczwoiv.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ghiibvyje.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gvmryawnl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gynuenoet.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gdripimhg.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gnlvxoimn.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvitfoyyw.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gsepolctx.sHtML


<!-- 参考信息 -->