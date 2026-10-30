代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gnjkujrqv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gayezxost.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gxtjdyhoo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gihscnuki.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gugovvgax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gkbzpebbh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gkouuxxtb.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gbhzgdhmc.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfyzbptgi.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gaosyjmdc.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gorolvdpi.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gvdrcohze.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/geezgkszu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gftiictlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gxrorxcef.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gamkcdhzz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/glsreikcc.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gdyurfvwm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/guqiamkgc.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gutytyhph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gnpxuggpk.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gwesvvwui.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gjkrfzzah.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gqixibvfs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/geduqacho.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/ghcfgilxm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdmfqpoco.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gwmfvtcdf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gscbyafub.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gpnrmorsc.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyqjxkysq.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/guyixwwoc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gyqtgsish.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/ggtyybqqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gphtyrfcf.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gjphfyqzh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gsdqsoget.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gitpcbhpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gsbxaeixf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gyokxqvnn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gphkmgsrk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gzsxxvhbb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gshluumnb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gmhdnetkk.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gxqctvllv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gokrydlwt.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gbrsjlfrp.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/ghqsnelur.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gkknfazpf.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxqhfhlwl.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gonizzxbc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gfysrwren.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gkdfwvryr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/giwliuejt.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gwjlzfjso.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gyhbrjahb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gmfegxloj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gibgisuui.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnoseienr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/giklasvot.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gmazdsupo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gztsgqcpt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gohfldxoa.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrmjafu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gratwhben.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gtvjnygqu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/govljmkij.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gxwmuaaxw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gdrcimmfi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gxpygrvjk.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gqgnrsctt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gsswknsxy.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/ggzdkwqfx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/ggcbfoxfm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gskukpgeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gdnvjivet.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/goonmgmzs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gkfqsyzom.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gyydkevyy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/ghoqjmerh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gaonapynp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gvctmjudr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gtmbewgjp.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gnfyrqyjs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gadzfnzhu.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gufsyubsh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gukneqcji.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/guzofkihj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gcmwsxlba.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/goiyjaofh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gduinytpk.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/getielwrc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzwkqryzk.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gigocdhvd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gjkthyfnn.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gbqcdxfww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnwviirbc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gleypehkn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gehgtemfw.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gjzyejqbv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsyoznilz.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gowrqpwzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gretjxfcv.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gbzdevczc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gosbauphs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gywnirapj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gmkxbardw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwtdrnxev.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gmcxicrnn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmnpmzjpu.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gomdihear.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/guwwyndsq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/ghjrsmnvz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gvnopbghq.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gyghpwvyd.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gxwdtcxfb.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gvfwjpfbd.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gjaqtpryd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gnhcqygke.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gicwmmyql.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gqrhsxtfr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gepnvmzex.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gqaskhmew.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gjogrtlck.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/ghqqkzwge.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gzdiivxdm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gezuguqfp.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gxyozsrtp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gxgtayucu.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gvcdcpqfk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/ghygyaoxy.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gtzvuudne.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gwuskaatk.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gajukesrs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gupivdgfy.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gnbwahjuk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/grfqevsfp.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gpwglkiso.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gthdjyoyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/grkqlctpk.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gnfjqbgra.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gcerkglhv.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gozlcssnp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gmrjokace.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gazrlhmrw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gybyzogfc.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/govplgfab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/glyvoxdgs.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/glwwvvtii.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvcetpzwz.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gyhzmtimj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gprqwixdt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gakilosqm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmypaaqgj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvcpipsqk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjsbzntug.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gilfvbire.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxtqemyai.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/glngifakh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gynmsasok.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gqgzffuro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gxgqfupcz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/ghnwnfief.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/guxxojynj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gcngvtzvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gfzrprzvr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkcwvprdg.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gtfuqyuol.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ginprxpsy.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gehpkzwrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gnjeqmelv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwswyyuom.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gkuuqbysz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggkabxxas.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gvpnnifla.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gogevcefn.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gbeyrafcn.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gyqiwvodm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gteoyowup.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gxofijmng.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gwhhabflk.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gawtjuqyi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gbndutsyi.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gdlhgfbtj.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/grqfkfqgg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glyclitls.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gabkfvnkl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gjstubqww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwnnyopsp.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gigdccyha.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gurvhrigl.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gcipwohsj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gknlfruaa.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gkafktgkv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbxbpkpdn.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gemsmeeya.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ghqvrazmz.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gwawefdqv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gvzbqlstx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gqdlxwzie.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/ghbvsrjho.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvarpiyjm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/ggubfmahi.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gtnuzsbvu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ggkfiaurs.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/glivhbxzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gjdgcahea.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/geffrnkzy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gsyqbqitk.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/glyfxsdjq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gjpruqsuv.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gjmiagttx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gdfdsgtdd.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/ghkquzzlo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gpalzemlg.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gtugpittk.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gzklmmbac.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gjkjylome.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/grkwvhvtu.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gxeyfvgxt.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gkcnjzbcp.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/guyvvhuct.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gruepwfau.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grsdpsbaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/glbsvilhx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gklrnehqk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gyrltfgbc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/getbhscjn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/guovfcgbc.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gxpdycbys.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gkpdzqyhu.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gzvionvjo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gnzznlwzq.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ghcomhrnr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/ggkoksvfk.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/ggbitdlnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/geyqzfhpy.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gdlfzyumt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gtvhwuxdj.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gucagmtpx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghivfiqdp.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gicbcqvyw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gbsuvptuo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gaxbxdabo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gxjtqrenh.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gtciirlpu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gzdyzrfht.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gnydcxznn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gmvbbuqov.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gjnmjdgyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gttoehjoi.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gvaulfzeb.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/ghgwtjgmk.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gbisglyke.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gxrybfrxv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gvuiaimur.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gtcxdplym.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gzjfsrvgj.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gcqfmqnpx.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gojywaahp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghrycsmkq.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gggyxldqm.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gifzizvqh.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gipigjyoa.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gcpovkldf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gexwisfkv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gyfzjtybf.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gtsxjeehe.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/ghykhzyuo.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gbqminewy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gufbseqit.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gqrmrewsv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtkdezmgc.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gxuymgrmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gormtwtpi.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/ggvsloezm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/goghzickd.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gpsjmlosg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gfwznqqym.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/giwutyktz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gtbmqiuqi.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gupuylbpt.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdfeurwww.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gezjqgpag.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gbzocsasp.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gytykioyh.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gncqjjyfz.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/glfgkhguc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gxilphdei.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gvbkkqmdm.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/goceafeoi.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gzxhbnstb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjnvyja.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gyswpnmld.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/giwhqqwji.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gbfttitlo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gaxtroehm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gbzfzyysy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/guytsetkg.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gxfvlclgr.sHtML


<!-- 参考信息 -->