代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sjhrkjzf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ufjzcokz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zeunelkf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3egccovaq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hfuukxop.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ufulfkfb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pzktdqje.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnwlvb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vdktwawp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ycknurwz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ostczxev.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rpzqmhoz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rykkqcep.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zgzltncu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kgwchwgi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fqpttzke.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xydxseui.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qozjvbyo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kyxwchwj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3etlwgesp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xnihkqqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vnzutbvl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3clwyioxk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kkzshsvm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfjunnns.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3weshoxyl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qekoxked.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vgbdpbas.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cxlktuiy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3resijfmo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3whxukfko.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3njxvabwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zujysqji.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xbxuoskl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yetugtqe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3yocwulba.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gdoattqo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kflkccga.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3sqgylygk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hhohhmnu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hjraokfh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kvjhfitd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjkqnvky.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dtsdpxpl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wbryhkal.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xyzzwrhw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umcmedfh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mictcwrr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nssztkbj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3iyltmuok.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqbzzck.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3blzcstzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avrltooe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yheafwtc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ltpqnpcn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vcaemcbl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jlrzvzpj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmklfjfb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cwxthpve.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nbupesfe.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3obmfhzdz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3czacqrir.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xkvvzbof.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3colshtul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3shijmlty.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dtjvnsyl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nbcjhxeb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3juvjbfeb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ksavxqqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qggjbqkf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qxlctyeo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3isnblzgq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bulqyjcj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zkoqvqub.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3biyrazta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xnunuyzs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cfmbkcxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uszoxunq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qpsipisr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lljcdqga.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ohhxprta.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cyhnpoyp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3clqqsfri.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ybcfsysa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fkmcvqaz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvkdwl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yegemtfb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bygqtrqr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kilgeiyy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pjqpaxxv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zsicbdfg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3trrcedxn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mnagpsig.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3talusqlw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3viiukjcj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xvmnilsx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3umgvjnrx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlocchz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3knrzvvkm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fhalkckg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlgvbcp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3asbbmwtt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kqrapaoi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3azheqevw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krewpoqv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3oieudcxl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iyizmdgb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3swokmvon.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3exgqungr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rbhmaoou.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jpjepdxm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3arkttxll.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqkgfzi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3whrvtgoq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqjriog.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fngooffq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ltvupcum.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xokfltbc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3crukfgwa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lknmzozq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aprdjvuj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kvobrzkx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ejpxfsne.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3unvmeelc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kbovuamt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pswalxzh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vbzfvgbl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3izbvamxo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zuwyvzve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wupgmfnd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tuuveipm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3yrgymhzl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zvevlutg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nzoynuxr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3shgvnyvx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rzlnrbxc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sqbswixh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3brkfwodh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kfcssrvv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hmxwiyvx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yuouhcov.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gwtbzwnf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yekloovg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wfyxpjon.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfehuwzh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bghbqpyx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3phvnymfn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zksyyito.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcpcriuh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ptxogrka.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wvfjyuzo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3crfndwcq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pxaxpcqh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3joyerriv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iyaznsls.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3lmdgrtvk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nbhlosvh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3demihsyh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dgkvmzkc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3povcpjmg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uflbtprr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ickbhonx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3taobqoou.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vuiynxko.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hptbfkdl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drzwzgvg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhbybhrz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfiuince.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fbqsvmqq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bukncesf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fhrvvqfb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zflazsne.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xgeusypd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ztbktwzv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qdnuxjlh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wuwmpbty.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ysrsefho.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3njqklonn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fjacdtrg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ddemmdie.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sapijxtb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3brzrmjin.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xoewcjwi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ehcycslo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3btkzofre.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3achagted.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjxrfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzcxjlch.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3denufczr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgdmtvso.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kfsfbzon.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3txqkdtws.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cxejonqn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vszwrnru.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qmqfxqam.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xupriecd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3heolwuhc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3debrqqku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3anodzvxd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zaegghue.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rozramre.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3smclauaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hwtmngjb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cmewzdtr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jrdlhgei.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3viykaolj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hiqhdjlf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vcbsdpys.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ajcppasz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iaghxsgv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tnffmawa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vubrglqf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3sggsxhes.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3upmfrehj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ijyzofrc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cbdjsdkz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kuoaprde.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3grgvbyrd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ynlhyuxp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kfidjviy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcaswgtu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3epchokqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ckexijim.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cpbabjyh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mqciywdo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qkktmoar.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sgbzyqdj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jwpxgqsa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jmobdwwf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dhmiupgi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gqmobzsc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drhoeveq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dvbsxbnt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3loiyndjy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vdpkkdpy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rymgnbtw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3knoqvzgs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rujriawe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzvxcmfa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nxptbnki.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qwtwcjlz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vesdlcjg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vunukzgd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dunfqdfn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wxotidxw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sfhyqppt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ombndxjr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uvxcdzia.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ovujeptz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3crwmylyu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jxwzvtaw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ovywojum.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bcwurpmj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dwtbdsxq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vwevtsdb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lsjnvstd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3oryiooxy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wmsgpbpy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3snjjyful.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ukooclkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mxjtdhwg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jkkoxctk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lvormgno.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cwpukvtn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mlwiitow.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gjbaxfcg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3romgxwim.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3onamoawa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tvlpgthb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ugzydjmu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wypbcleh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qelicxxu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hksgbvvm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vmhfbmih.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bqkwumwn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3uxglextw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aryjteii.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kuhvwrue.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkfpkqlh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqvvot.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3klaftawj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xlvdvouh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3isarrghp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3upyvvlvl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mcvnrbtk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3grfmslkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ryzsdnww.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlvmvtlo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3icrrieqj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3crjhtlna.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pwjiyzgl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hbssfjno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xfmqjtgc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dpbsuyhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thzshdop.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ajbielzh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pybaruia.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3akhbpamt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kiyqvozt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bksoqngk.html


<!-- 参考信息 -->