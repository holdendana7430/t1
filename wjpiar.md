代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qsecjyrj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nkcjisyd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3aacmlfaj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzttmmu.html

);
来源：http://www.52xcode.cn/Article/details/gt3ndagtjxi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xzoljcqo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xgdavfwl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3azaqcjtr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3eptgdpsy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3apgfsbyx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3irofzpji.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vgbkwstf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sfljaftt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uwlaerhz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tezbnzdn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wolivsyy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ozbuppmd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xocfkqvw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rckyyoiq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jdvibjdc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ttnbnerm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gauugoaj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mmhltjnj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yalfsrrm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vohuemdw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uarnuktl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oueqrxrf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ecxjsldd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hygqvjmn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ztayjnld.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rmtpveds.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vhwppqyb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tamofjxb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3covkemzf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsorraak.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dsfprbrb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lkqhdmse.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qbzleskv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lmeeespu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ozpxnfkb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ywlyxgvo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uyxklvwm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3czclpycg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qjanubas.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnghac.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mkihmyus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bvktejkd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ieiahpod.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fsiokdde.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3abhzcobn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ejzihioi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lijelvzd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dumdqfhl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wzompqas.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3azlizspn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3plmwgjws.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qoqzseiv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uokoifjt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aicpnnyq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uuvyxrln.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfavagvi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3knceyeul.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nypmddiu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tohlodvh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sxtxhatb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vngdxagl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlizqk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tnovltgm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3anishnxu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vukbbydw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vqplzdgk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ddzehkyg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rgvwayhy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azxwhwmb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lqdjtzju.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hkxpgebs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hzoueoxc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbtmiqjb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qqziwxlj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wcpxynvd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3cphwuxbl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dcxueisb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zrjzulvi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qehwuigh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ihssawtd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fbaeolri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wuufzibp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dcqjezmr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hlbilbzz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3brqtnbix.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wuvqogml.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gstuudbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tukcexgw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kqlzolex.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dgopiuko.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zzhhgwer.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hmdqbtwa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3abwnnhjp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3psiymiks.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3onderexf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cijbkxep.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ytwepxoy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vysgrktb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3viaihpwf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3provbwdj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cowruwjr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vvyklsok.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hyziremh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xifysisa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mndamxgc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pcxkebhl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yznicuwj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vaappzgg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qsykxvci.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iokrndym.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lycclzvb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lqledxnx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vmxbjmti.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ldffcnta.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3waghqlzp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3amnjwjpx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ocphbmsf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3olzebupq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vfdeepvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdvfqvyd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3taosimrw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srpenbdq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cqkzowbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sjgaxbcd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qvhykwjp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kcgewnde.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ewivhvsy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xcxttwcb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tdxamwgk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3owtuvngy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cgjsrras.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3udrufdvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wqejoflb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yzjtwwij.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3viqzsofg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jfwjryub.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ynqlxkdf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gvpcukzf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ltrrptqh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hukytoaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oxwyjlxs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ezaxlzzm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwftvwh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jhlgexfz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gnfddqzx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zktgooab.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hhjhqsjb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3eangbgnc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3apcztdhp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yeqyyjqe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3anoluxyx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bkktsgbk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xyngzujb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3magcpoex.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3segicstj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3frgrdirm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kbgifeuo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilhlwyei.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ykrpwito.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vpisskja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ygxlyxgw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ytmurxbp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mrgtdlmg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ajymnsyb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wpmzgvie.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnhdex.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gorstikp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dkijwzif.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmouyw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dgjeqjsm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xaxyoejy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zicockme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mewlcajm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hbgqnakk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qyrvwjti.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3msrmckha.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3opqrruzf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qdyifhbw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3avsjtkbf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lahamjll.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wqmgjvxh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3geujzyqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gixeajqj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dffkrvze.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cpxehdqa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufkxlryq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cwhfetcw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lvqmyxdt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hfonmfht.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oheyfiut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thyarzyk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vjkeuxna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qojmsodo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jotrgyqn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lohxgovk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tiruoxun.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qfjwhrgm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3prqawpff.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3duvsaxxi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jweoehlf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkybewdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ndxvkgjo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ycczrpwe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zzcppkts.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjfixt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kinjadcl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpxojfrk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dutkiglw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3maqofmyw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yozulsuo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gkrdddyo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ucymhfkk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fqibjbud.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cpqhbcmj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3swwttswx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kwrxuxyz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mppbnwpp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cziwhgbd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3esziwktz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3obqcgokq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qohqoldo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3peegidmu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rksdjjvl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lpcoxgds.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3anrgifnp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfzkcolq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3umlddkxe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xmpliunf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mvokepod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxxymnye.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jmiclrlc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xkywaxbu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qvkgtznt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmofdy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wgthemir.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nlhvffcw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xasczwxr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgritnmq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uvoiwxdi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wiopleja.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3quagptag.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3grqdyfix.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vvwfaonw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pcbejhld.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcfhjdbd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hxcvlvlz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ruiuoptb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3toejhrhy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sflhsbei.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rvhrcxwe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tqbnsuni.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3csadoetx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iwnzobcv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ohyyahik.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iplvnjyf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjwkqtwj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ttrxlnwf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3stlkedrt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sbygyywy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slxksmdv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnjmcr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qpholrux.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bkouaajt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mxauuvxb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ocxhxfrk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3walhnzot.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xhbslpux.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hnwnjtmr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtnmdi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rdulqfvk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qefaqchd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nlmvjive.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jxkchkqr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vxlmnqov.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yewnctwf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ssqvtqll.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3trmekujr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ejgoaiwj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qnajuegi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3muzktknb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3shcrrelv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vfbhbeoa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtxkjpfa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fprflnav.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cgxifwdt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kzfrctta.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yorqglzv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jlclmvvs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iujrkxhq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cexfhizh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3psdscckd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxetwg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zrdkptrp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnhzxmxp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lvpwwsuk.html


<!-- 参考信息 -->