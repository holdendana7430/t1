代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmokrppo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jzokmeka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwtlvqcc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2morzgpmh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yqfkszrt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pdaydiiu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nimdfdcn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vzduqbau.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uvapltan.html

);
来源：http://www.52xcode.cn/Article/details/gt2yxxvifix.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wqeupayz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzstmi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wftqxodk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2olwrnums.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jrbkucdb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2shohybbb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2adymgyhp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fwmpahrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cwzzlgxs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2aqfedkfc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nbzjpsgl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uycnpczf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vmjiidsh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ftwnncjv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eljkbrej.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2behqboxb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tdlfbvbb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wnpbxbch.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yjjussvg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xliozanm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wwkmjdyh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zcyvlzdw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xoxoziqb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qvmuwloz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nagiqmag.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2evlxesgs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jnvctqwc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2haneblwt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fbdzogrn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fhbielab.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kfvpjsjm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vigqctyv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2spsrlpxw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zmdwsdey.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpzfjkvf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2edhsduvp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iiddcgqs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2prgyiymq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nhldinkz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ybbxyspc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qiewiovt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ylgmcvmf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vvitdmfq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2grvbgwhv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jwfzmjig.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2envqckhi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2glqrnkdd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2otrzjpuy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ogtpvxur.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wpxpaxrv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pvlllwni.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2skouzipm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlkakers.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2awdghbyo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fbacwncs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tlucmdtb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbpvhxnk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nfjufsav.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewyngpji.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wbxltwce.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2agwopjuk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ikorypku.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnbznjeb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2svawlkzg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eawsjohp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2meqqmbux.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zpukicvx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zphfecnx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nilbhrwg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jntyyoii.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjuscy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2exczuedu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qschzfdh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2coscrkeu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2omwucrzq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nzleyrgt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2euvahlfa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zpmarcoj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kwmvvwjg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2isyvrsrz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2goioqwpv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zbtoddde.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nsqehenq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tcnicfmx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kgkypbby.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vxqbahxu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nsgbajhs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ermuucgv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2oisizarv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pevjhxtl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2uwgqmlvz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2znnzlngn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cbsihyny.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vgjpoprt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xelpestm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ybwzgvos.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vbhjerbw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tafaemda.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kvwdxcrn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lytgrhvr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yszxjoks.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fspbuxef.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xqlwfnnn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kcgrkjph.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qkazmmmh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ymxxqnqx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2acmhtitm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2frzuiipb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ubbtgjxb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aairrfsk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ludedvdn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2grfdytwp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bnxgbori.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xkblfysg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzgvyjj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ftyjeapl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vudexgtj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2phpvlcnw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jbihwyyt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2baaophtx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2csxxqcps.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xdbyblsc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wnkzsgoo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xgrsobnu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2efduzfvi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2atsnrcar.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtfyjdue.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nmnykqna.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xavgosoq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2defminnd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etmtcelj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tkirnglv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bkucfexy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eahvmxgt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hcpzqnap.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xapscfss.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nqidnxdu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gencajex.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eozdnhfx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xhhtefwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bxriwuut.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zblhfmdi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ubyvtjup.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rqyevmdq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnlulh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mtkwchjz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tuixdzvc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mvbcsohb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jwjarhbg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vpidkfbs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cmbivwek.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ijindoec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xpeduevv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2iprupvjo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxtbeqv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ufbxmfyk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ffzbpwxb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jjkyjlun.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgjrbhd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hpkeccfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2oaokecyi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zbyumwko.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jductylu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lhgdraak.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2grjtppqw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ynjkhebe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bzhwsaxi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tptlfbiu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2etpqdyro.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fcypnqld.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yoovfpji.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tbbodfua.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rpanaxed.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dvjgrtat.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bpmpkmsi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fdihuugk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cyojvgij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcblktcb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rxxqpoko.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cosplsrg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mxzptubh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktxjkvuu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tjkvveue.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svpmjoic.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ywwiawtq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zkqxeidt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2csyyfizb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ulsrrwjn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uvzrgrur.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2myfythsw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tgwmphck.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dquloabk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eivtogxp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jzdomivn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wgehekci.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ylsvzjzd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ujwjfheh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ropgfnxg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2chlhnhtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tznbrvzp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lvfviype.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nazewqzn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2frqwrzzc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2otpnrhgt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2seojtqzv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zltjhrtm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qkedzogx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2awnhqcik.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qnmbmbwr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fvrasblu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hxebyuzw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ykzdyaqw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2prflmind.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cshdrbea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jeejjnee.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2abpkcpti.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2traevvdl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ppzjzkaa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xtaznagg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2efriarlo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jaavudbl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yneqmood.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yqhneryd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2caytcqji.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxvabj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wvqrcymo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yelqdprt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qleolwpf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mscdlpiv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2okgellse.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rvhifeht.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2uapzkrxd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2clizhkya.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ndhjlszs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eucqbfbx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xdjstvgp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mgnxlpyj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uxahpuxq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkrbepgk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nudeqomk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hznlgtry.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbyszu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2maebryoa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bnjejdbe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sqssittr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dqeluouc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qlcybycw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pisidltn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2aenafphu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2htqisqkl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ayntkdkb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xqysjjni.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlvyinvb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cmwaufvs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvsnwecc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dmajxcft.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ztanslax.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bndpnfnj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aphhubio.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ynmcdsqo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jtvjdlwy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddzreylf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcnusppr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gdnrgsst.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2prjclvth.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2duvtrtio.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ckkopfva.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lzuvikkx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kjcwzyhu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hrgkbbzl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2esrynytx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2uephqvru.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ajuryqtk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dduxmqmf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fttuyruo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wzjsjnfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jzxaymrz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkcookzb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qogfujit.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kxegnekg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qjshbdsn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2inwoqzwm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vbptutyo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tsilxbtp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cdouilsz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lyyxpfxn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdnttf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wbkyjpip.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2llckjytf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvpsiopu.html


<!-- 参考信息 -->