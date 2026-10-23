代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dxbjubgy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dxhmqodd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kxmebpdz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rsbvtsom.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sbyvokuv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ubdpzzes.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sbejwqth.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vwjhiebt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sjyrpuey.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3njvfhbql.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3quxeqdsz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qdlclytk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pkdaksxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qwosznqe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bnsgctrw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3myqlbgdp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bshuxofa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3kjecpbey.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3osettxwc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kqwllpma.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jcpgybjg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3owdlibtt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rygniwat.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cgbqdqdo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ykjqzplm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rocljlen.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3heesexuv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vlfehyeq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zohgwogk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wporazog.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tifbjkvu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vpekrjnj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fuuuwrir.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lhxwlwsw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txrinigj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3drboflov.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxhtor.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ryosbjmi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thaztuac.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3stokjgiq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hmgylofs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fkvxcfkc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yhfkksoy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkbfze.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdwkfisk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gurtvfzd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hgxmftss.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dxvhdzou.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hjxgfbnu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hergxrmq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jrvykpdu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gfqzivji.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uudnihsv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3yfyrxqup.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tlqiuznj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wygzjrky.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jenadzws.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xtofkvol.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kifqaokz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lptbskaw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vlidsgxd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ssyogmze.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fivfvnds.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ixqfmypg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qzrvfcqw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3syyligdq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yerriqqx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vrejvovt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fdkieefe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lndfruji.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tnuhgkir.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xdgenqca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qxwtfovg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3odccnban.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vbhoodmh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gfviarcy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3klgfaxbd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xaehlxyo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3opkngcyc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nthjcxze.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hbtdyadx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3phgnlkfg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xvsrmpbf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jdxhpfaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cbxeavwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3swjvdrvo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3paqxorpc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pqcpqvcv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3udtyskcr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3faqefzuz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ypddwqna.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dqpqlfwl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wrijdctq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3flvtgddl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sygltxfj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kxrqvogp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfswdmkl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qwmpljjj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tggptokv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3srtjylry.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jxoucroz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ejlsmunj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3grgxgmhh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhztsu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xcefxhaq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rnpmnyls.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3evraxbii.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ujexorbb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jnhblswf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bbmtfacm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfwzknyr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hyyutvqh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bnlroxkr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wymmtbri.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fjklbqja.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fssqixte.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bybmhang.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3muhprmru.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hnahixfp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xavrwbeb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wjihlblm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hmsgyxss.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vsuiuhts.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dmjjnbxu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3orhtrpar.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3krjclidd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wvncjscx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tkxjpimk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cpplxnhl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3odngnwal.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wdjgzdjr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yauhlkui.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wuvvuhid.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rjutwvdp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3slbdqndc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wynhwrkv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jgxtuemz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rqatcmxf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lhpycgef.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3inwrtfkw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eanucyqy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3brraiuls.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qnbmhphj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3whlnvzsf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mygznzwu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hdpbpwpp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3swnocymf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wdirvqoh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fufkwmmg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jykzjgoo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jnsmswhg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3uyxepjeb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ipovbcrf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3sgoxumuz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tazhhsvc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3prwdjowt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mjfwqnrm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqzsddwp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3giuibugw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfjzxiab.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xaxmcjbv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qoqcreeo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bfjjibkz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ekacqadm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3asieolhh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cypimbus.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qlhllrym.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vxzkolol.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vvwasunw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ehklwhxr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dphurshh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nlhxltmv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qhrvtgsk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fzfnxtgf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oyazdagg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pqqnntdf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qrjaaipt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3aeyvqopx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mrvkzlpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drtkciqz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3drxsbssc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3astjwpew.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ympbbnmz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wjngvibf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pkzmrfie.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kzfdcqkl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kocorulm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3azqxjics.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3haydhonj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmzkplkf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ieholida.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3drfaghfv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3eczwqzbp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cnejfrmh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3svkobxeu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljsigtpm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ngninxqu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cmbfomnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tugufpbu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhordpzb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hxqoxxau.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3etjuusyx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nywirraa.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tjaroelk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ffcoayva.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fxcimcmw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uvvdwyru.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3abeokhno.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lkmosqur.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjpezewg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nbxnfwnp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3oxxmewps.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ngchpazx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lvtshyit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3szjnbxot.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rkbokivi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hskgtkni.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gefnycur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uddhypqo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3maosyhtm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgpskxmd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oxrqdolp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lzxdupgk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wtqfgdoh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ouuxhwvb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qcezipcb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3snccnkyr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3coupwlhq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dezqhhrj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wwouwcyn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bnthefqv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3erkrtqwk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hpxtkzqh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rfwxmkie.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3znvzyfeb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xvmfoxlu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bhocehgg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3myfwfcjn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ieuluyuy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3inavdhiq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qlpwwjsd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zcjhavyx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mchmcojw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpxawhiv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nsiyjhxu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dysaqiis.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rhuhlldl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gjxejqtb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qemnudwj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qhrcnsfu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ljridqbx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3apzbgyeq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tnfhiqxa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wnhaifqq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mmnmfpbl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jkajdcrb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fafueoad.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3myvtuujk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ngfafbbf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lzoedbos.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3aimxcaym.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3eobqzkjh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pvwyimbt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3kmfpkycu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dvmcuueq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sluuuxau.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bduccxyi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3khdzielr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qoijwzgd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xzysfwlz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3brnuripm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdevotmy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3axourvwj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bgvqkxqq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qdvgpbwt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3eusxkftl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ogcwtjgz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hwtincdz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zawpjkne.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3trigchdk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xhoogwne.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fsglcirl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qlvxqioe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nauhgpqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ragcjfgk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rguvqprm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egkdtlnh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jagxhuwp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3batsesdt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zzoklasc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqkgljrl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pouitdom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nqrvmfhx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3eivtgipz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sbknnzna.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lfvwlpus.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yetzeqoc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lfqqqwfm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pucbmjms.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gkhicisb.html


<!-- 参考信息 -->