代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gskwzdafd.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/ggiixinli.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gxlggtfyg.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gvlbqtmfu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gdvaayosa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gqtspoxwe.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gucjgqpft.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gezdiplms.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gkxymsaqt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/grwmoogmv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gqdpvimqq.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gzbjbjvuy.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxeoyxnnj.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/glgckyugq.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gscszujxo.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggpcayaya.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/grlosqrcf.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gxhoojllu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gyhtaeijn.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvjftyqoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gtpifnnur.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gguisysai.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/giuobqsan.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/goihiehuc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/goeeuhvlq.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gsouoofnl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gtktdqewq.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gvybjhzgz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gooqaypsg.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gvxemqklh.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdpeexfgm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gteqczowm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gruajicno.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gegsauwzs.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guwhabfqs.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/glfyfyuio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjbaocbdy.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gcswforya.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzkzwdrso.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gweozvikm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkcrdhpoh.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gdgqjiqjv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gjqnklxgm.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/grqmhmntj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gvcrjttgh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/guraxjysz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gbudsbrxp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gwhuuifkj.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gwegtjxvn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gswjxevee.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gynqxrfmx.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/glnldffkw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gymlvamvc.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gchtzkszz.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gkyqvprpj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gplkncnaj.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/ggisinhlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gbsuuklip.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gtohnvgsq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gqbppykyr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gdasldjfw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gkajikwio.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gzxahrpfu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gtjnpxfwj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gzykzmaay.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gerakedob.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkzmekite.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gcxswgaas.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gpxkalcer.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gfurugemv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gkmdxjfgf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpuorwyyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gyjwesvnh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gjztyyqbx.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/grcqqcqct.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gdtzipuqo.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gisgfltuq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gcycwophb.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/guyvqnpdl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/grcblguaf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gvgzbvegw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/grdflfgnc.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gptmijrmi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/goamaovzf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gmmzvakvy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ggnrznhop.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gyymegayg.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gqxczxjfl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gwwnzsunl.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gjynepjxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkkyxwxdu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gpceunsnn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqllpqald.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gfayedjef.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gqnhtnbwa.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gmngagrok.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/getlhpzcx.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gkcxifkgj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gaayuzwjr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gzghcwuek.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gzfonkuce.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gjmzpaavh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gjaueiaeg.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/guoqgeotc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfxmlgptu.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gggonomsb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpaamtitx.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gdvuhlsrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/goqvbjihg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxzhzuuec.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gfatqpwgb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grdgocrgr.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gbgyuawbo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxrddcilx.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gwellbuug.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkoasvfeu.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/grapovwsa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gsphxqrib.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/geqguvfez.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gzjoukabg.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/grfsiueyi.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gdkqcovyb.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gslzyspla.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gqggohxsi.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gvvddsevm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gftjklwhz.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gvifrusef.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gfmlnshwc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gwgmtyofh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/glfrjeggt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gcktyhhcx.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/ggyeqqunw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gnmwwzejf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gtlddiqnp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gztkqlycl.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gsaxqmvtj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpxwonybz.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/ghufgylgj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gguukwmbc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gkwilespf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gfoomkuxz.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gksdsigtl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtsqfknlb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gpsuqmxts.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/goyayebkt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/guantmrji.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gzfroqlga.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gzuptcgxt.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gpfutqxrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gtkvlqifg.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gcyjezzbq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gzthymfny.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gaoghnsyk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gronpuays.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gtqdjlniy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkeqwnvhu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdddxjcln.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grpfwrllf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggimdbjfc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsmkzkocq.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gwygvykjj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqlwvnkwq.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gxkmmnowq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gbjwmnxlr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gbjppqiou.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gmzjtetej.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gimkizjjs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gbhjqayin.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gxpaowfrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gikhnuwjw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxmektcoc.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gejwwzfmq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gjxkvunvd.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gvaqavniw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gehpxowke.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfkemqnrs.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/giosjkkuk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxwlmkzrt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gqrjogghk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/ghtvbvbew.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/glzsxhsky.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gzweapuek.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gftnoogao.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gpggsvtlg.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gfejpbgyi.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ghxrhyklb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/grfvhkbfg.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gyjsgzibc.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/girgytxyh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gwhhajldd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gafiedqgq.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gymipwnwh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/geatqhieo.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gxfhanxpd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gjljavejx.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gqqerobbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gynxzalvp.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gjhihpfcw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gnfqhqtme.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gryicxkqe.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/ggfivyrcl.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gavltbfuo.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gmgsggiwn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqqetpsrv.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gizdognyg.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gdagrouwo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/ggoajjgff.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gcolylytg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/goeubwtti.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gdxlltfdc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gbqsxijic.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gomqvaspj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkqnzehlp.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gqqgezhkr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gundldfwm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gbddtolsm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/givgeqoxn.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gfoqalhmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbrbzixhx.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gvgpdprxa.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gcqtiofcw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gqtvwkrnv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gskdovdqp.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnythxz.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gvcywikiz.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkunvlxxr.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gcnimiyxn.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/glhfmuuvp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gwshlblbq.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gffqdhpyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gxsgwpeey.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/guxlypiso.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtkbqqcdn.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/govwjfhai.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbsdabz.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gfzydtdvn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ghnzrxjld.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gjmppbaqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gskqlqkeu.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gngzuwxfr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gcwrwmhvq.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gewxpasiw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gdqqrdyuv.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gbkxlwixg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gohfmnbkm.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/getkarvkz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/genlgddjx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/grbgmhxmy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gauabkvzk.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gvxdjqxei.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grcvccrvn.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gqwregfyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/giwpkrsiz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gjtiyexcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gatiejoaw.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gxrevhfco.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gtmvakohk.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gtmfjjrnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/glxbdftgt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/glenkpwqt.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ggypwzrmd.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gblklydiw.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gsjaaffkx.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/glenwttdn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gvuxskdqe.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gjsgychzh.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gscumgfnc.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gduyphbjh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/girkrlkst.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gdyytcwvs.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ggssphpws.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gvpjuhimt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gauvchwev.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gaieqmdrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/grpzgkjga.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gpwpogdel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gckunczhk.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gsflcbbxn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gxdwbxgya.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gwkhqdzhu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gqinkyesi.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gfopnytww.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gougfkzee.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gvignlbpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gorwjwhfz.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gpskomwkh.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/ghfskutxw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gaftrobwk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gmajnzxfj.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gleczvlpd.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ggqqmkkgw.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/godgkuhtq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gpyenjopx.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvwvhqhbw.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gwaogemvr.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gbmxmgfdm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gcuoprrcr.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gpafupekm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/glcipcmtx.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/grxdsoqdb.sHtML


<!-- 参考信息 -->