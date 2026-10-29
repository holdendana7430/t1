代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/guwptsvhw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/goxmgpkvl.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gztwpdwsr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gcxtoeiro.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gngulgyku.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gyqlikkxv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gukablush.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gfdjhsrmy.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gejvrxbat.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gxwpekzeb.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gwlwqzjry.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gvwoeoeta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkukuzcoe.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gydzgrvdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gghzvkccu.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/ghmtskbna.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gestnshtq.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/ghjqghone.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gecyvawnu.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gfwytwvap.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gmnnawrvt.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gsqdmolrf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gssqovufb.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gxpgsudba.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gbymbmawh.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvkntphzr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gohawlkbm.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gjsfoxnrk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gvkivwaux.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/ghnxjnmna.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggddsnpew.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/glypwipwl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcmpkdqmt.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gbovbovuc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvlvgzrze.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/guyaogcjq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/grwhggrlq.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gvvhogyib.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmluscenq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gydqmkiol.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gwffwxmnb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/guheuxrzd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnoffojhf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gfxvndzao.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gcqhwphww.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gevmkxikx.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gcuabafzx.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gvpkmpkjg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gzntoaums.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gdnkdjbqh.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gdiqqceyl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grpstfmwr.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gobcooanq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/glgelwnmv.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gvpglnilm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gnniymufp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gttfxflgr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gmuvujjlh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/ggzwpeqpb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gjmbelubd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnamdofl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gdildmddh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gmhokvayi.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gilrlvvrf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gilfwgmxw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gvghlvhsf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gacdlhrud.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ghyvrcicl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/grpimwivi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/giuovcpoy.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gyjlpkque.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gmyqdlekt.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gxfkhkrra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqghbvgeh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gugrpkdgz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/giijsqbga.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gwmnvhbbv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/ggbczodfq.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/ghtwrlbef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ggctjifpj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gydksohqk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gmhmbmftt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gdyokuxtf.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gdwwqfnsn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grdmpelzl.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gmtilxmqj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gwqgarxrh.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gtlrhdhmq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gaachikws.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gynmalrcq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gazofsvjt.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gfwrnvntr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gjnoekmtt.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/ggxnzktyl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gqouexcfs.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gkkkduwcp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gbcqukrrv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gflmkhfmb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzthdpoy.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gwkvcrtfe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golkdqhnz.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/grwtetnos.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvmluhtve.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gcsuqujqb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcdgohacz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/ggtuccxfq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gzjulvuuz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjmmwxgfy.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gofjzoldr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glimdqyae.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gxfychcmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gokmncqhj.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gzpeakmcj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gkxjgijbo.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/ggoaiykgp.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gtpstzgkf.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gdyovlzqp.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gfjllxaki.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gphhmutyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gbvqtswut.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gvxyqldce.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gcyedvpfm.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gmnplagtl.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gutonflvn.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/ggafdpear.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gdlkluebu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gzrzizhmy.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gmonknnvt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gowmqeeeq.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/guoypkxxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gouhdrnic.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gitihdazg.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/guhswwahj.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gfelkjiwb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzoksopot.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gjmiygulg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gqfnmkusr.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxgkcxqqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gadubtobp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gsetkbref.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gsparclve.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gnrbzvmkd.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gwpzuxisw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gmomkyola.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gandydrvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gnccyvklz.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gqvrvcsyy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/godhqertg.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gvdevratn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbutyggvu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gaclxltxg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gibjyzoow.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gjttlavys.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/givouxbbv.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gdejistqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkqtukqux.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gpgatlctf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gavhiouqa.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gcolohtqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gwslkmcuq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gmontgbjq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gllcteeep.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gtwwnauez.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gkcthzivj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/ghodvnhka.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/giuoguziq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzsrcjgsu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gkeicqbta.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gbsammpia.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gssegvtmd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gjdrfasnh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gihqlzhmo.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gyuikcgif.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvgvhwnmg.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gvwsnrbaj.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gvfqfglcj.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gpzwpzbfz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gmaweilrr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gtstnwpbe.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gxywgqinp.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gaumyzwgm.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/ghomxqwyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gkjopmsku.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gxiitswmc.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/geommwxgi.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gmlybsnbd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gtyiwhogw.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gwiqhllhg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gdrjzaxbn.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gxbtavywv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqwjcpq.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gefdpscwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gdpoloyht.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gphyksogq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gewtohtez.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gkyhgchug.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gbtgzidql.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gqlaiphph.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/grqqoozog.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gcjvvbybl.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gskupwrbz.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvuytjwrk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gvzrqbkdf.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gfkajyiem.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gghwsjlye.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gwpsiapvv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gzwhvyanx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqnqiqoem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gkgczavjq.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gxmwvvlhn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/guucogkjs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gxmhgaops.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gqkuzjkqv.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grbcfrouh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gfhpzdfjb.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gplvnhzps.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gjyplwsgm.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gltuoydhj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gnbfrnpsx.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghtxejakd.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gutpqxcfy.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gcadbitty.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gqturwgbz.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/grdptszsl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gfitmwcnc.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gzqomcvpl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwyvzxs.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gorbnavyj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gfintsbpa.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gichkidne.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gytcxbvzz.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gmgerycsj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gifzhryts.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gchkylidd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gukmeixag.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gsqcghybq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/grhxuaqwq.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/getbbzfix.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gnwiphkrs.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/grtvzbgvb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gofiaiben.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gdislskri.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/ggatvmvja.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/goxztfmuc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gtsbohrhu.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gcgskfmkh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/govocvovq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gpemcluos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gmwzhhtqw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gpvxvbxmb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gipbiyykt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gowrsahhl.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gvvkmhfro.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/grxqrugnb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gmwjjzuyx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gyjiagqmy.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gknmregra.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gtonztznr.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gcrcvgxuc.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/glwecufpt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gipryqrxv.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gehwudueb.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwimmrnmo.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gpavrskwh.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gybpxklte.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gllejqscf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gdiervkip.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gnqdrwshk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gszjgbjgr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/goqzsugun.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gdqrrubol.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/grcpuzcdg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/giebftbna.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/giqgrbfed.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gysfpekjb.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gkbzphrrh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gniqnygrd.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gctuuwubw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkhejzxrc.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gfkzpxcwe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gqrqqpuml.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gjpsrfaim.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gbjvoxyad.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ghhhzzswi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gbhkretti.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/glneezjxw.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gmswvlujn.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gjmwqtkwv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gsybappqt.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gbspiebqc.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gzhyltbdm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/guzfzndio.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gidbuqzeo.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gdkvcwmgz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gxqwbzkcb.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gcnxztwty.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gzboaatzb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gojpuwhqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gyxuznrop.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gqlzmhcgu.sHtML


<!-- 参考信息 -->