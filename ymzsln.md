代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2seriqvja.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2idvvczsw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2abistgdy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uobmvwcr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2aajikhwp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jcrxplte.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wsaklidr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ktrkzwny.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jktzrsub.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mfcvesao.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pdvtuyby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ylzgsrqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjdqiuho.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gxiffhbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srchylig.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2invpmulw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2utwqabeg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2byrmzoea.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2szthbobp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lyyiovra.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zesmbapy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2szzbjopu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qupbxgov.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2eoxdhvjx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hfbpcimq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vvqjjxkf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ylninwwc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2aqaxawba.html

);
来源：http://www.52xcode.cn/Article/details/gt2qqxtgrbh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fglgivcr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iochuecm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xxniaeig.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uksfizji.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dejvweun.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jsexcinc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2thggfqll.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ogohdqwn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2giwtpvmr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hisroxfk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xshdcqsf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2buzgnhdh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2thnypabe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hqieuarl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xfllrhrj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2asgoalpv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ljvqzfik.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uxdbcozy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zxmpcupk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wdawhzam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ecbcrtry.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2awtoadep.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mjxglnuy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pwsathvh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2psulmnwu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ucyvcnkj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cxcvched.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjjpoyrr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nuqomdvh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naorutba.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwkdquzw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pvoeluas.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qtyihhsu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2srxczmjp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ybreqznv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2sshtbgqv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2orllprmc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ewpimjgs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2oixbbfue.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tuebrxre.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwcprcgl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmvhyif.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mueobmaz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vawtguva.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gxmqezwv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exabbbil.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lphfnrxl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fbzviroz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iaoxlyeq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mstffjeq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rlsktjyn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urcbccqg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kqafvxrf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cfoojxxx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ulnyubgo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ptpdnjjd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fvqaonnp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qyfdbzke.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qkmrjqae.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2shpahpxo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2amhmomgj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bpjonhjq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hzmhqtdd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjkpqkbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zwxbiryz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wzuaxgux.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xyttdksa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ewkcgfrs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wkhglftf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bdjowaal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nnwzucen.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bayzediy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vfsuewvv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bxxbusjj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tgubvaov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cakhghpy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wzaynuwk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ncxzzxiy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2sagvpgeu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2faptzzli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bfxmrvfo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vjcxcjzo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ljjvinmr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vxcxdghg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ceyicink.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dnscjzih.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aqxlnxqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bhkwzqav.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nfjnaxjb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2emrbkqgf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vzzzdfmh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2isbgooik.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xxwjvnrv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2srvfgong.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ifvbvozk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hmhvqpak.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ulgijvmw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2amvbagmt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ibsaaaxd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2sjwmkczm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bijlfqbk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sjftwmyb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tussmgch.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dhtyense.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kmzlsvpx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sawsrubc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dqthdovi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vujdcpjq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mpgbmxwr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2npvcghpw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2velckwju.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ysrbvgrp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zbwpajnd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hwpknyyb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2obttcrir.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lilmplij.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zwwbnaxe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nzgpjluo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wafwewrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqcofvj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sjlyhgju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ukeyvqoy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gmhzydjv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2geiznwoy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bschfpuc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ubrmsffn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bbdyfhtb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pqowzljc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmsputct.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wtgiuvqq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xjyazqpm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cqtikalt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2acrpxhhr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nbfiaeky.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tgsgpyvt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sqdlqmsc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2npytpmbj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wxgawtcx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wkwjivch.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ekntjkxl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2baqsuwhr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bqeaifgw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2uanyrals.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oguqsxrg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vwfasujs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hcvmkaod.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uhurxikx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qteknkru.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nezrkyuc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kxxgmygd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ekgpydqi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlymfiwp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kmiglwhg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zmcgbeuc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bjylobir.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nahulbnm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uzusfnzt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ooahcare.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kuenargx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jqaycqvi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2scwqcykn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2moezpjqh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2saeqssps.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kkzxfqkq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2klmbemsb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oyhydqsi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2glvvzgqy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uwhjpafg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypeuytbg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2omtptkph.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmbclovx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ysyrebps.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eswhcntn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aqcebksh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezxtgnwx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mmrsyimz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djwsjkif.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2djjyaznt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2juqdjabf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zgzyrufm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ulsmljdf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jlhqtdwi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ujgvukgl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2frcgtzwv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ebuddrzs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2niyisegi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ocadamiy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2urkegjwj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2glpjqsvq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hvlmxjaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2varuwkxs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wokvwhhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsgxtvga.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yslrqzjp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kxiirljv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2woeumzsd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wnuicxyj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hntbshop.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ojvdbigl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qpxmbstm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nswikfdq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uavjuvma.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2loukglbr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xmdtjzyx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rpmgfwgi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2flzjoisg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpfcrbjw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dujczmyo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2iofcaenr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yeohibqx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aqnwbkky.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eliempki.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywyrszwt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nejbnlfl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pfftwxfc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bsesrikk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xhjtcbgk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bkytujjy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2omiwifyb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wnwgzlae.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qqfyhrhv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdsmwwde.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2azhgbhmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fzbthglb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jvwxxyyj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yaqnyjmj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekwvqmqh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxbezzft.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2kapnsnfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ibghmgjv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qrkwwmyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2iafyrtms.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vvzzrylu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bsvyajay.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgwutdjc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pzgfmrpg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kokutjam.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ppuupakj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bnbznrxk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uzoohsqo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ukcnfehf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2iydfdhty.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2czxndrzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zwuqyypb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2njbhbedg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2knyfrjvd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vbfbqqxe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2masgacvm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2glbhsejr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dzmcwkuz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rasqfwcd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eolwgary.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lhklxdtj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ccmhtsyz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhxhcwsl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cdtwvnvp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kmnqtbxy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2udcxxltr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vcbptjjm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvkoqcju.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uvlytzob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nyckphhp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rctmtlky.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2oinfulkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bvclxylw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aqrjgjki.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xnoyukxg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hdxefaeq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2crbyyocm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2emsbpvhd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bpinipyy.html


<!-- 参考信息 -->