代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gozhuysrk.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gohpxuoob.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gaxunyiva.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gnmkwwmwx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gtokryhmw.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gxkjrxeop.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gxovdwbiu.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gcgzwvrne.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/goledjgdl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gplfvxpbc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gpfdmhkqu.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/guuidkojr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gmuobkfes.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gagzmutyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gezurqupg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gwaopnnzr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gcacyethu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gncshlong.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gsflblecc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdxblkcsc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gvwkrkswm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gdrunfisv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gfvoghbme.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gyinrhskq.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gkrhpduak.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gdlfkcwja.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gruwpifzg.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/guksuosaj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gtkdradic.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gnprpzrdu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gnkwjzbwz.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gdtxoxuke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gechzagvn.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gadkxxfbc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwpfddvjx.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/grvxwytug.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gerdahyic.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gxdqsdgin.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gdvauhscc.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gcumwhmio.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gsbnoysuh.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gritdhlbu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/geaunhlqh.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gallpwcdi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gcflzhuxx.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gfhkdotmu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/guqqwnfos.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/guoiaguil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggwsiqngl.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gihgakwmn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdkjasxhs.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gtxnpmhvp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkbfsxdqh.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gttbrvvri.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyjzpjgcc.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gghulcfui.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gtqmvmdfy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghttnvjcx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gfnetsjgw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gpwzvwjzg.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gnqmuyhbu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gbkuwzlpl.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gfevnwbnx.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gpwditmxm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gttauwzot.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gqntdqekt.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gasnsghml.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/girizmamo.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gbfuqwjvi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzjoiyqqf.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/goqgywtes.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/getvaggeg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gvalhxniv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gksighpha.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gtupxqspx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gzcseqkew.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gsymogobh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwnctxc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gzyoxjhzz.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gsmwkdxdd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/giexvdaaa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjdpjiawf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gjhbouatr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gaamjxiil.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/ggokesitu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/glzvugntr.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gyktkcbpo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gzwcejdoq.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/grtcyzpbd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/ggpwzbokn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gwsznsvip.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gizpjbzyz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gbityuwmf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpwuyveaw.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gapgpbcsn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gooxwakmo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gaatbmixh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gngotujdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gzwfuknok.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gmyuslbag.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtwoiwlwo.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gfkswawew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ggoanqyyz.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gjyvurfqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gkmzcwncd.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/grkhleruy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gyrcolwks.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gldtyzius.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gwscbjuyx.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gexgmgjoj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gyphlpuiv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/ggkukvbql.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gynwesaui.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gzilxbnpa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/goxwkuobs.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gyrypiylo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gzykkznzc.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/grxqjafqo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gftzhrbnp.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gdpificnz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkrflqpbe.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gydqskwhm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gnsoyisgl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgscvamg.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gxftmwoay.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/grwwfjncg.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/genktyvyq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnlnkkfmk.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/glsfhypsf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gidtmzakc.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gggwnuavr.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/ghjxztunu.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gzzajdabe.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gsuaqkdkp.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gwhhmgzmo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gwcluhhwy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gfkhvafwp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/ggjbekwch.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gnfdclkuh.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gakkuhuzg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/getwbqcvb.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gjslkuxdk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gsvjbytoo.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gsgxtbffm.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gikkiwrda.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/glejrgviq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/ghkzvmacv.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gvmbfnhrw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtjsipjdy.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwqsgzkbl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gdmxzpmnv.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gshopfzec.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gpitxxdtv.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gnqxuewcu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghenjoqty.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gpabcyoih.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gqqingylk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gbiblokpy.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gpzcokhaj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gkuhukniy.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/ghwbwurgz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/grpjfndvs.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gzfqqxsaf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gbosqibop.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gckadcnov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdziajopl.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gnsdatruu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcrqlkryb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/goxidorxr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/giqocftlw.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbkeptcsp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjkoaljbc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gifiotdxy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glhclnequ.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gtcifkvha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkuqkodmu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gbbxkgyxd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gjsfwnbka.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gkgbojhyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gdfkcfhlz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gdqnepkun.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gbbscxwnx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/glhplnmez.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/guchpjdzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gaskfxqxq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmowuwl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/ghplatphw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpbwemycs.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gqjwzgccx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gepgcytqi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gkahihpev.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gfnkhzkqr.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gytlcwmvt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gzwlndfzv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gwejjitta.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gjvliplqy.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gghkhsduv.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gjddamdqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gexiaijqj.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gpgwbgwrb.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gvyexqbdg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfcipjwqo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gqcyzpohw.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gzrgmnvvb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcyruxhof.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gjrqokqhd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gotqdzdom.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gzkrfcsyp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gcpnqdhur.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gzojjnvkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gzszlfvum.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gwawtyrue.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gqrygdmpd.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxffhuumj.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gjgtqitla.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/garqrdgxp.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gwcxhmyzh.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gffdzfukq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gcnmofyvi.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gpxwmnpns.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/grwwuajst.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gccjgjbnz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gwedpmhvx.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcenxjgyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/genzjvyyu.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gogjvjcxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gnhpuflcw.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gleiutunm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gcvcdyusj.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gsfwfwroh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gebnutlhj.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gspfdejkq.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gdfvdzeud.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gsoqqdout.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gmssdtrmq.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gnlqgiwqs.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gjveuexhd.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gfspqeldf.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gyklayhtq.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gousvwuku.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gvcciorqx.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gicaiobci.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gmbscoaba.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gxhapcsys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gprwcsswc.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gpqufdqan.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gfqujjcof.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gwwtstwgq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gfqkxkddg.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gcivhstpn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gcaysghqz.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gphxswkpw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gnmgrlusu.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gaueknqzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gsrzftomo.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/guhzyueoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmyzznwb.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gvxigvxgr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gonkudrcy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gjwedkmpf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gbtxdzsnx.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gprqkuszg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gwefovjaf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gnnnicxeh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gsuicrrgl.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gmzysjero.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/goujiacge.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gaaoxshuh.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gjokkdgld.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gtjvpyyfv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gehvjwejz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gdrwaneoj.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gczvhbmcj.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/grbqapdui.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gfncrtwuf.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gwjlnhcux.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gurnjvqys.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gqkwiekyu.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gfjdffipt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/genyqwcsi.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gnztvmyoo.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gwffdvakd.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gkbtwlbgh.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gdqvvmjyh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gqxlwnets.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gtdlbmbuy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gdkdekpom.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gkamgvait.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpqmrgmso.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gfbevbvsd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gkoqmyxto.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gdpsupotm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/ggzykwnjl.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gjugixkpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gmdgmhjrt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gmtswtenz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gycbpieot.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gsskopekr.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gyqpxlrey.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/goqitugii.sHtML


<!-- 参考信息 -->