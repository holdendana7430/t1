代发 wailian999

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gckcujzxd.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gjcqxgvxa.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjglihqq.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gnwpovnge.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswlaklxv.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gihqchhsg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmeqsvhw.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glzbiqtsr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/grjngrhjp.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobuudlbh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrffbta.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gplnbkdjl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gunnwvzil.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gikzcuvni.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlndanri.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeyvqmzc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhiwqze.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagukpif.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfyavcxd.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gbkpaqmtx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gbbbjrwvm.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpoqpjrm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvozxgto.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gguavjyzs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdphzvbo.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gpjdpyufh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszoxaxyh.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gxkucpozo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytgbpphi.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmikttcj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqtbxbyy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejumnef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzepscxtv.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gaqgnnzjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/giffvhrvt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsunzhfm.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbjrihhy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjwjvwua.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/giiagsght.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtsplloa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyealvizy.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glaxiasth.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnepcdglx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwoajock.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaovsiww.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsdijxkr.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/goqkvrflf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyfsqpbl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gitzvizht.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpsoclin.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gojperwum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/grtbhcgye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkyhever.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbjarai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/graltoqit.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtrezkcuz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gpicxgpwu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gqzphnhla.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwezulzj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gubyepcqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gvulqeneq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrmrjeg.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gspcdomjb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtojrtzxi.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaatddaj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gterngyou.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxfzlswhp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gktfyakvz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvknyoby.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwybyejj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiehixik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gommospzv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxtictjx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gupgxhkee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/grppivmqs.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhfplzq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxvqctb.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gguyjkvou.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvrclpin.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/grapiksjk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpamuvntd.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gwatnjoue.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrpuiljc.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwcyrwn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpzajrjd.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gtqlzsxbo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gunwolmma.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpuiuflx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlamtqyl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gjsftbxis.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjutbqdg.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gfahhquud.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxbrrisc.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwzjvwfr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaaqttne.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gwclzadyd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggzezpglt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayjczwr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gbfurhtsn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guarzbwqv.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyegmmao.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpkqkbnb.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyygipya.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnsnheyl.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdhjzuwfm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gtermqyoi.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjiibts.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/grugznyxc.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/geomcbcma.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/goeimahdz.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/geqcaihna.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gueakepwp.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gdnxxfiab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvarmjgm.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfazomal.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gpthplyvr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqvnobny.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/givooqubc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkziykob.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdgneek.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhzgsaxt.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gblqcqjqt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfhzwhex.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gycnaphde.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtvdtpmc.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcnrrvfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimchffl.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grckerjur.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghicjvzwo.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gefemskpo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpobwkuvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gftdeqkhk.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gcavuofpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gigzgfkkd.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ghwuswgzf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyqlhkqz.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhxkzmx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gagqgpbhd.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmzokpff.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttvbctcq.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdgqnuee.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmmvkau.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/giundurmq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmorsjayj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovtwlmo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwbtrmxk.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gddihwqbj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmdjgafp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjruhzcy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/globdvape.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnjnsdkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzkgexai.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsomhbnt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgncoptb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghnhqzmbw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaygkntpb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdhhmnlk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gvwtpsosb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzduxbtip.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/guhwhdwly.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gejmlnqji.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gocvtajjc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpbvcjhx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gijbtofxe.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdqmkoyxj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmaylgkrf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/glizuxhws.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gdczmjnns.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkgaiejl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzlroumf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuwqccke.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmdxpsn.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gfdreizlq.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxilirdn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gidfzergm.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gcvsdpupk.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyharzzxf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/guajdddcm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggppedzkh.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcdbthfw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gacvbvycw.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmygmsqu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guoyspwgf.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjlplwurk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpopowrci.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grjxvzjtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpnazyfeo.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gtdvdgige.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gokaosrts.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnavvlqxh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugwvopgc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gausgqscs.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/golharwbl.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gugltcndg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmvayynn.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gamqvktut.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvpokrah.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldnizvwr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskxtfve.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdybhqch.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glbrcibgx.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsibxrzrq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gashdzzfc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gveffbono.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlkknljw.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsaupokx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmhttew.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtstbqkjz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfozttffu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/ggycsacxf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbvenpcv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxctlwlec.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmgoqqaoo.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwowbhkn.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjnyakoi.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvfwkluj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqvctas.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzncajzc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeujjazh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gonbljrkl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gopbxbdkt.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/grrmppfmr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbyujuld.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gdpnfvlvl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwgzwmf.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/guyuazffo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvrvbywue.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfjxidoff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjszeaxvz.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gppihxowu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gsjegdjya.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatleilfw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvpxbwopm.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcrbcekz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaskoakvh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbsjtdaz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/getpoqhec.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlprqanp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxwexso.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gyykqkrsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmxavoea.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenfnotn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnnhska.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwcbuzh.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsvoxcby.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grfruktdt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/grwgycefa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzgoemhr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxflqcmb.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpoaypsnj.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gobfclvwl.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/guslndgqs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbdroyfgw.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkyhhylp.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gezpnqejl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppxguwqs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnugfld.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyztiblj.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghdhrzxqm.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gucncspbw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwhyhpww.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gxpfanuhl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gnupbccwv.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gshebvkip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glwurvdfb.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdxdrpaz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gavbfqhsj.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrtjtbej.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvllebbm.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfzamgky.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgohsmyi.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/glqxsoyxn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gjovaptqb.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvrzokx.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwewqeohm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/geqesdxzv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyrkeiav.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjjnkqjz.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoblhkjf.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/ghejwizqw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/graisjita.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsffczxxu.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gdwqpzkty.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdspchzx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmbftqv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gatpnxjtu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gbnftdnkd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gufnzslxx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzdiifsmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkltdllrd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkueylehq.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfkwbzrt.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gjrnrotos.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwtyqopwe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyevdgza.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmztuwqr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxenhhf.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gganinmii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdeseepn.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdoxriona.sHtML


<!-- 参考信息 -->