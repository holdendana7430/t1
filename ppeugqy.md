代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grumrmgao.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxbblej.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvuhvyxn.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjnqykss.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gppzvxalv.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiwxjizc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydzkmypu.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/govjbjkbg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspmgazub.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gteinledu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gtapxyefn.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqsazvv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwbrmfqq.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdlzuqo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxvungyjp.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdhcjifz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxzzouzy.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gebuqrivq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtdlrcov.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/glenctozs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmmmhlrd.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdntxldgf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztqkqwth.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhvnvva.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzqbquwj.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gndnkknto.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwerffbo.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gbirdolpn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfiqxaaq.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvxspvgdu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfeivlql.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaehpyadg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkynglevn.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlfikrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/grkalhtsv.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gouqmbzsa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyilhufib.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gddhgkgcw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gppwfhvbq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gcenvrydg.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtukpivy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gpemutmwq.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/glrpxeeuw.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/girdwphrp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqkituly.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnusxmujr.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gzlyuoghg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkugyjcwn.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknvswoqi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxsjfboo.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gpiblxwyn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghspxrdxe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gkhuyfieg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpsiwvglk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbttdjzdo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdiohtno.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdsekkyq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxgpcqvp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gvqxeijlh.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkphstczp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gqfqfshcc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmhrncqb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gntotoaxm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gajgwahni.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gbvmitatt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymowpvyr.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxcqrwji.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcdkqynb.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gerspcdcx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwifsrgh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhvxpow.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gptenqaui.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkdnajnnn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfhzntww.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjjgnscvp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gprhtqxtm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeqojsfy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gprrajatm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqechbjoo.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjuwour.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwtscjc.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdezjihl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gohdjzzuz.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/grovdeehu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmydxti.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnoroswb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtgfalu.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfteuxisx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gkfkbopnf.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gozkomxqb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpnjluoh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvtipsi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpwkbvgy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gihlydcaw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjsfbyvq.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhmzmqfz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjewmthj.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwbukxu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwjqqtej.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gwilqfxmb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmohmatko.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gpbcvwtqo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gonxnniua.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grapnmcma.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkyuwrhi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkbchuuh.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpokkwrw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzmebhxk.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmvzporv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpcisdwg.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwifpotlb.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/guykczexi.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtetdjcvf.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfkfhcil.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gvhepdiej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfzsypi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywqxushy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwqxvfck.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyvyvpoj.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gswvzdjdx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzjmqxr.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gdnvbtjpu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gjwwdafmp.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gunypsjmk.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkedjsiu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggordicee.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfegpnlq.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gychimgsq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gudtzulge.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gieceyrdn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghyqhttcs.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrgfrhfa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrpfumnf.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gfijaoffg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfmqvbno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzzviqov.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcsmuxdu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glaumwfjq.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqtmqnou.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/glvlkpohf.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghopdvldm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvspbmkzg.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gftzlbunz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/guhhpcmrs.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gznnhqwpv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdolaxlz.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbqjtlao.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqgyodfj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxswibz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnapywqo.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfhesvuk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmtolbo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdwszyde.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzprwfjqu.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdvxfffg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolelkmv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/glonfsteh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gghdlaqrj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbncagdu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvyxtwqd.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gzqlvsnlx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gtayjhbhm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdddyggt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgyjnavz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfipjemmf.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gmmzlfyzb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwcamgyb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gydlsolyc.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfllmcask.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqkvvpu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gmquqgquy.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/glgatyayx.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ghiewckqt.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gfntiwjmg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geowwkiwk.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcczjctyb.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gelhvxfsc.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxhaizt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gzlzxlcxv.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzmrzmqj.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfcpgniq.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwtglolvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqdhuyve.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/garikjbww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/greuhfeqp.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxypdhxtq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfgawgttg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhdqtdeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiuiyhqk.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpetmrlj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkvqhkqi.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoadyehg.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmdptxkk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqbzzbem.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejnyywqm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvitpiqai.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gaadkofxt.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gghdvjboc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgdkynyj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmhciebjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzldcni.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/grpjukssb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgbvcipk.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyvkvnqqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmmsyyrc.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gppeehvvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxugthtn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkjehch.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbmxddkk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzzavra.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnlcdyc.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgaoqubd.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtduuycr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gicifwyak.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfctqmlhi.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtocbsfuj.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrcioyey.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaovzshq.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmtammyo.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gttbopjnl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqashgpho.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkfowvnt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkygicl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpirajpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjxmtjk.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqynwsjm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/goohkvjec.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gbvwxasmh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gitawhidq.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdgvkbpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genfakrfe.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbjzhyqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcycipyp.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grwjvpqnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gijguqdfs.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghtkqlqqu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gycorjrye.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjvcajvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdecvuqln.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gswdqgxrj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gytiiehve.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbhswrwap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdgktjsu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gaenynmqw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbljmvfe.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvdhzdolx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsqkfkfs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsxypzkez.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkrmrdod.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedclauod.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbzfgmex.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdzbcfdm.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkmfagvxr.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gfseburhy.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsepfeydn.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaozmura.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdihnfipu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpykibusc.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwgxhtvig.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpohsfvxc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoscvtpj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdglhfjvh.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqaoxvy.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwjzqotz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ghklfzslr.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfstsab.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggqlzqxum.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyruwmybf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmdcwopd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdlihxhl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmftvaoql.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmzaapy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gadlvastm.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsdhfnp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwoishsx.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpowezy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrgncewx.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gcslaoybo.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gatrigwip.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnufnhjrz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gowfotckr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyknepdm.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gemcyqnyb.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/giuftgkvk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gatnyvjrc.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnmyrpltg.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gwsbwioik.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpvdgmht.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gncivasxr.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyknsvbzf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxjseegh.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwcrtwd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gesbsuxap.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnfikwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqflsaimt.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfyhzjm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgqzpen.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdvdabfr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxbfvtf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqeawcrw.sHtML


<!-- 参考信息 -->