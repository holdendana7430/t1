代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gjbnuljkv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffscywuh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gwchcldyv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gpvilevrl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gvddwfrso.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gajuflcxy.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gohusjvck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdlrrbdv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmrscuew.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gotipewjn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gedihbaae.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gbznkotzt.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpwfofhm.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhurekhz.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdigzgnmj.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtunkbg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfzdjsx.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grgqrnfqj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/ghddjfxkf.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gfboaibae.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkkayzbx.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gqxqsdpnn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghamhmhla.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givkukegm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhmearbm.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgcrtdmo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpvzdxqf.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqophod.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbskxgqk.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqaddqul.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glpcmxivs.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gokeypojt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjdhljsi.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntjguiuz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoltcsgx.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gjtkloaio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxjmjywe.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvcdhlt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ggqxhvjvf.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gcenvgmsf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkajplhj.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/ganygnsxw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnermvmz.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gjjhvzyae.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gytiwxlyf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmojlnpee.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/geuneesjw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbtwgyv.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/godtkjipp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/geuemwpft.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gbndgzekd.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmttynrc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqxndqht.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmfxdfq.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gssoabtqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gyybiinrm.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsunopgls.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjbgrdv.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gebtqimaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gucfodbua.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyjfsuem.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfakxla.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqaqyxvs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gdrcwftbe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/grauehfjt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gvrbabvsk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/giysiugwq.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcatoxjep.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gvohtcaoe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gddldnxfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptiknhmn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjtjlyzsk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gtwcndyya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/glxgygyuq.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmorgtkow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmroxapi.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gewiewosv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gqindtodk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gxapydxcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrklzqos.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfheacr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gbgaywfoi.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvsreaedc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/glylwpwzc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpndzbmxs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvteuylh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsajuzdxf.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gbgsbqjkh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhqsfsgv.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gulzhtniu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gmjxuywud.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoxiwmke.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqcgyjjf.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gflnprzzk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbucuich.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdyagerfk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/govfqwvbh.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/geycctxpz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gptiouweq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivufdga.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfnuklqq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngptjgn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaupytxo.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqpczvy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzttcyvoy.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gdurextbi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkftntxs.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjmjhmoy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbecjvgvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gnipokkzl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxozjibqg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckxbafoe.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gagcaerem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxrqhiyw.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gakoxvkwm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhiwigmz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqokbtyo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpgqfybw.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvbzykzg.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gtrzavhtq.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gtqdwcykz.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gopuchhho.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gjqeowddv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqaqalqx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/guxzeskzq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqihoupmt.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdqknhji.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvkpxkpf.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ginwfhhwi.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfmfeok.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gievcyxid.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gglsymmvc.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpphaxgpj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfkkfuhw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzvoibac.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gisgrwwkg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqpseme.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysyeujid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfkiuzo.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gccqazurt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaqjqzib.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmzacvzme.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzilzoxmy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gopwmhqec.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gtkldpkhi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gphjegztd.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/goqshpaud.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/ghazookjd.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gslnuyrfx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gnlnqatkc.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gtyejrfvs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gmqddpteh.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyampdqfy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnccokdii.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnfuiefkk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkuklqtmm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpqddigom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gioojmzdi.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfjqcgqeg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyilwxwbu.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gssbdjsga.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwbqlmzi.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gsnnhcejp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuylhwow.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzqgvatb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxfssqej.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/genmavinf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrwcxxst.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gapvjylon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/goadgonos.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztzcsalp.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkgvslhh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gdwadwbde.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlcdwwnf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gjoixtcej.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslwfwtuk.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgswrvxu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzouepiwq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gbroitaqt.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gdvuchmuz.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gfiufnwta.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gitijouuh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/ggpcrxiwa.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdtcwpqj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuwheomr.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoeowlur.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gnbxgpotp.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqtmloaj.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjlrhrru.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemcgqwk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gotwhjcub.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbfptly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbvvbxvj.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpzwemtm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcsgdbtgv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmomggjnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/guvdiudjg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcxnlabd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrlnqpyv.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsjrmjhf.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwhcukg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjbxttut.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gunqvaypo.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbspkqecp.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwamnhqg.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gycduojvg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmneiyiao.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gctsbxnmt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwhqnpjt.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gkqqbabjd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gureeygvj.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtoxijxn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgkanfuy.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gktgqwnvu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glanastyo.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslvohag.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gomkmxwep.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkkzpygc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteqedjme.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiiqcjff.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmjjxbhlo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaydgbcur.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gewsucmne.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvubxbqp.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuzrfhnm.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxpyslvmf.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdykfcecy.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsefzsov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtecekpfy.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gunsaootb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggwcfvwlh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gaievxmau.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctxgvjl.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdptkeu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbogvjeb.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/ggfaftxto.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gstjkkhnj.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/grmlvsxam.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gictuavvl.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/getdjqeli.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtuzeplsh.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojkhuxxs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwfkmiav.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxkfwqu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfpbwlter.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/guedokvxp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyfxtplh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gcltnlmje.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumgttohb.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gannihric.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gysnzjuwm.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gidamvkaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gormmslfw.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gymvntsxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqqsldh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwikxnvmx.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggpjfmvf.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjiajdjw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gcstooipn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggawziacc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gztokpxdh.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gonznxnyh.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtngzjknz.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqgxyvvk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsryoqhws.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtppdex.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdbaktqf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnqpscuwy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/genunpbkp.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/goaxgvvow.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/goeinratg.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoogkrqb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gmmhgtqwz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glzfqfcnw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzywcugca.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbryrisnk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfhfykqfo.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/garbarzgp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgkdqary.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwvaxeqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gzylhewxx.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvcwwtdwv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxwbkxlx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/giculywas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghebptfd.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gepxxdvce.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gniakhoui.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gycnxbdzj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gvprwbczy.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmyosotkc.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grxsfprbv.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gmamuderu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbtmqhus.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/glvxvibtn.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gekntdetj.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyvdodhr.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuabukz.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmojaebp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gvgqcfgkq.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grbluzqrj.sHtML


<!-- 参考信息 -->