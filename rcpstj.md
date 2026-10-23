代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qhtlipef.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ytexogss.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eorbguln.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tivigvij.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vloihafv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3twluizbi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ikdbasjx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wwoqulrc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jwpsledo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vqnwvbmc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xkuujzzs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3pzlzylho.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sxlfcfpb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ydfzfjtl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3twuoymhl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3obnpyrjq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3amejkuqf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lhrfznnd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cuzrlshe.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mwyulytj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zempsmwj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oyasaqjy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3colhdbhj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kgmdnirn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3idjjwvzt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cystthck.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mqnvwhgm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nthowscr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qesbujub.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cqchjjpo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3trgrfpnu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3stiyiqle.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvuxxik.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jwxzhtvf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3oqmffsyg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ddkwzdlw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3flmtfycm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lznhdspf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ajtlrbah.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3njutzssz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nrtcmdqx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3twebouru.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcolrnig.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kdvazxho.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3paihjvcp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ullzgcln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zuoopftl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qxquqgzi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqhsdg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ydzsqxly.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jnsoinsq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3isrgaitz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kgzhvahp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aytawxin.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yhpetbum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pyolsyjx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tpqsskbh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ztbxmssi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3aqiopygi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3twfocmpo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bakijnac.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mkhmmulj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3simuoxul.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bgrgwreu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vygbctwa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kjvwltzz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xntujhao.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3exqbbwot.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jbfpyuug.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ylobaubx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dggcwdba.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hunppxvh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xekssien.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fbqbnjmk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yqbrwqei.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nstderwd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xindnmvo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gwrfjcmh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xyzsfelx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3orsemjkv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xlybowsc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3izsqhxpy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfxtrnqs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtilfct.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qplcrrcj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uctzwqjk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zrbrakhq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xmoglweu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3irqpxtib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zsxhhcpr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fanoyeju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ujyarwxp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vfnkdvxo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3aalswfto.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qxgdoafe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hiovmegy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3anabqytd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iknenrrt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3krrfgnzk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vbquexpu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3emwinqpt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ipqoqvjh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3woqspijd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ozegukzs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jicgwiwz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pwysuvaw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3holfjbnf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mgwjbdkw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cpadiqzp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zgbqkncl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vzegzuyt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hbwzzvvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxlfcpjh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rklkbdul.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nyvxjpwd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ymuyxnzu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qkyhhsin.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3faoslxpx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3uowgclrk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fmhmxqlx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3egbwdebv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3haqdxxbo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ggjjptle.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nyrzhgfu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vjhebbkc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lnjbkpib.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pqpzgpke.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fltfouua.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pzqglpiw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ingiegwt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uslcspez.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uinwvacu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ohbghsbp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cmfxdmff.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uzorbnkn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xinxunrs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eawjvbiw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lybcsenc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3efrjinte.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rpyrllbe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rjrrpiwz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bpggtnal.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jxuseiyy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fajdzagq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stsuzgxc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3srkjbtio.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gegabgjm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tafoirbg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vhkyevut.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zdzlnhse.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hkajbhjq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ylhxjxmg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mprbxmwb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mvdaaeal.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ykhlpcmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gxhfwaqf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cllhcftu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tdmxquua.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3aqdwisag.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ttdqtgum.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fdvvvxyg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3useedygj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wluasomv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aaupumqx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkqeavoh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfozkzhg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kqjgabgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgnahurd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wfhrreqv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tpptywrf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ltmlxflz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nfygggnb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3iounemwq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxtpym.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3auooccer.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vzcogzxy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wquutykv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zlckwbje.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhlobjpx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kqtexnse.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mezjkgxv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bxubuynk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ybuaocup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adxfjctc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tsdzyjkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldtlwnnd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dfmaatfo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gndgdizl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3efhuejaj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ksneldrk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3enmdutjz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mihvxjyc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ticfpaia.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fhgiedcs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yykufgij.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pharzdur.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tboslrmp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uemvmkjr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oawyoeiy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3mlxfkhle.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sjzjjjfk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wgmeoknn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxmbgmjb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zhikteji.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3innpbyxz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ehkcicia.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bvnnwyxq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mnkssuye.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cmzivqpa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kpdutekk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ywhfoksi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3coxtewev.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ibixbmco.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cgmlzuaj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vebkcqyf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihituqbp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kadatjvl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ugowugvd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzlipzhi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rdfpqfxf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pwubimdl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jhdpejgs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxiglzgm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3idegciva.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nhliqwhk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wqaexfid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewchqdey.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kwigukou.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sgdhldcj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tymszwxl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mpptfruw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xwoviviy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wufelrdv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dbugcbuw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3njtaydgb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3etjtkjsy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqnjmqve.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbwpslmc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3edifbfpc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qylkyyii.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3agkdzopi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3oojpyywp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tgowqsmx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vzsataxx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tnnqyveh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oqqcngeg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nywmpbit.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjlsrrsu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bvebloic.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fgqzicia.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ugykortq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxbilmfk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3udtyxxrr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3blsqlkzn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfvmblxk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jbiajgij.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vpsqchcp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hnyezpgo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qgaakrwb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bhrbqocv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rlxrgxvj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lhtondjb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pofiaswx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3akbsrepz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mbtqpgxq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3blaqfjsl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3iqeoojzn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qkjufjpo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3asyubtbn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yrftbliz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3sxiegeul.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vosuqzml.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pnkuxzaj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bwhhodcc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tyfmzjzz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpzuksgu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yoqninfs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bzanpihb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3plydbosb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iuohfcmz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yjczklpd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ekucprjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jtnyxpsu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ompuampl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnqiaclg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ogqmtzzg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rymzloym.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3womrbqjc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3subwjadp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zocstvpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3czzbjont.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uajjdeum.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mhlnkveb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wtfwhfag.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iehykiro.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rnfbbvfp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mwstkbgp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3klwrsknk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eoxcxvuy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3clwajfia.html


<!-- 参考信息 -->