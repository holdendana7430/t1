代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gknhevnly.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gjkcdnkea.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrxbyjz.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gtvoiaejl.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcomkuqu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsedkrfbo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebmkpbmb.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfrhxjgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gavgmrxcz.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/glmlhtewa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmxqasax.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvkqsdzh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwycutag.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gscwwbqpz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvktecxq.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guljevphj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpduaiiod.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glvjjpzhz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimychgq.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gcotwhuxf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujszavr.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmvhsukk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsboyubh.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gaztbdzje.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gngvakygn.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/grsuplktd.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfruxftpi.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjxznhy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqvitzeh.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoyyvftj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmtagebn.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gduylnfas.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdcvyrxtc.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghllfzigk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggdwinfn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhlxhlhh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdngzjnyn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhkuhqkc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsshrfkxx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gzppbxzzk.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gismolcbx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gihzuwvqm.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxuycfo.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcepwrml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/giggywcgv.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvzrwqc.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzotongo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbgglslv.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrstoupl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gvqkydpbc.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbryrqhx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/glicduuro.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gpvkgydma.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknsierog.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gskdrqwjr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqcgutf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghntjmfi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoiklkhr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfulizyi.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gudvesxgt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplzbqcx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gttqqdtoi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjruhbys.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqkowfx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkkuxahx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gygrmvqft.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxzcihkk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/glodwqbqh.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gatdxkgkf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gtcbjwyan.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnxwvtoes.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdrbaknh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gaoikfveg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gaxmukysg.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gszcfuqvc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gyvkfusxp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjzsgyuqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqyqgqbp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gixtpegzs.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/ggdrmfxbp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnyqekjm.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/ghdnsraew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gwixtxeeq.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/glcgjqjlj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqwewwdx.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gnpddiqxy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmdlitsu.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxkbgsbh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhaxchfr.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/ghggkggxl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gheeffqmt.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwbyzplt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgpyrewx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvszoeyic.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gfqyflfyr.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gubbbsexw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtfxmtjc.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxslbhbnf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjghlecez.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ggagjtygg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goceiwsyl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxujzgguq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqkdcqlq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdmkdsvc.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gkezdwtju.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gavbsvioc.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gqiylakpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzabrnlx.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpttxso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmduawq.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gapujhshi.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpuiugnl.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gojpzokyn.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/grannbkio.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gftoqlvch.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gsgwzfvmr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gubnqjilk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gdzpuwowj.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gpbrkkaey.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbmmbwzy.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gefiqzvfq.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gksovzmpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjiifmup.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gdzalyqro.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaxjjtcu.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gizkbnqfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gfwtvxqrh.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuqqwzmk.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsklydzye.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gamobfipt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gttlkcomh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gruwxtjxr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvqbcyqt.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gihbfxdbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guuybjedo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlkrxyle.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gsutnvfzt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gchmrwron.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gagfgcpux.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvldgrsws.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtyrkqg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtklojnth.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gnkjifkck.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmeplcpg.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtstjbkx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvtjcxpw.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/giosylsjg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpphgpqgy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfexzrons.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyybetitw.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxwyumoq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvsihfkrl.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gvpbzfpbp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnsosurnb.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcigaton.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gywsoxnlr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gkustwfyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/glkygvkif.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwxcfovrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdierfka.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ghfbxqkym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatjesfrl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnrxmbrk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzohblqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/guyhdxjft.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaofauol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrnjcsjt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grjyhacmt.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemwdipt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gohflbajt.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gxldoxzie.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gdusrkvdl.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltqoevdz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gltqcbfol.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrfdyftb.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyrgezys.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfwfmpzf.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmzndwoxt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbsbwcz.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/geljnwmto.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glqcwunrn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxtebax.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoljpnao.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjnxwvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtycpdvf.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjznegvoe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqspvmkui.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjwoxba.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkanktss.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfiaimgx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfxvtehd.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoezmnsw.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbkkmhig.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdwxigku.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gramwvrpz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwxtfozdi.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gldsdyyln.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gplglhuoq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbdulhp.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwnivefbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtamhgu.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvmjldbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gowyqkrhx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhtqmiym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoujrdqk.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatqwpisz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmojnipak.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwygywywx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gturjwula.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gwngrmkdu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gadvveyyh.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmnyvklmn.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvfifhmd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoaxyivc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahkzgmpu.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwctxhisc.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/galthtfiw.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrfhbgog.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glenhyhul.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcqpppvtg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/grhefleik.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gciygulys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grgnormsb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gfubdpjjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvnytyrrb.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfbomhyq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkcxxmqh.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/ghxyzvwze.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghioscike.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/glgvbncpb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurvnnrqu.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyynemdip.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvduerpr.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhpebfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfttpcfph.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzhuzkvu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrgtpkrd.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbcoocwk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzcgiaym.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvubwhznz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gjayuylhz.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/goxrerxph.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gkrqymayy.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gihtoputb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkixjurc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gctnqpgdg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgkscwve.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfsqklso.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/goeptowsx.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gpepcxarq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gswosdouo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlhzhff.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezadujr.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcchidajq.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glddhmxnc.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjgpqevig.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghonpcmlb.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukbsznbm.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsmepnh.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqorcxxcp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsonmeway.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbjkdsn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjbaghsb.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gqqowcnwe.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gztuawpez.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsogztra.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/giphhvjhi.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyibrnet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfnxpnqq.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gncacdyja.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gisryskhu.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqosfdlhm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gosumicqv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgpjkch.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdbobawpj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaknievu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwjvmelbn.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gnmuyszyr.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmgqeezo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gfqpqxoie.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gknnutphi.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/garjtlkgg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhnrzxau.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gzhgjuqzy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzflmuci.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gmofoaphm.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gnrikmmto.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwszavm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsubvlgy.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ginfmugqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gcujaenvw.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gnhnyezvq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywrfkhmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqtnxwjr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghadadklj.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfzbwgy.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gguxisgow.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaqwvpwe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouqjohut.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gpvixgvgm.sHtML


<!-- 参考信息 -->