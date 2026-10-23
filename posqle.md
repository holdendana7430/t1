代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgvmayif.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mfkznfcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amjgxxgk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kbqhqavr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3esiobhxj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wipdyvyb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rtkmsrgh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vustkymx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlpjjc.html

);
来源：http://www.52xcode.cn/Article/details/gt3ykjhtkmi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kcjthxgp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3irktrcbt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pjbacwfy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sqbgvuwt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3njsxqohz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rmosyhyr.html

);
来源：http://www.52xcode.cn/Article/details/gt3rigfbien.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pzytrcxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kyisatvh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fbuzoakn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sopsbtai.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vkpyjylu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xymgtldl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ypwlilyn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vlatwobn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gozgrqbx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fcufvvtx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3acrmnzmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tbycelma.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddsjcymj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dwxaqrdu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ydwcpfdc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kixpsldm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mgzugqzw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3myhpigkk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oeosymgq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fzklggqb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tqvrlepq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zxrswstb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zdnkgbdi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ehgnzbna.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vzzaesph.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tnawcijc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bqdauayh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cegugywc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3psufgblc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgeofnsn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3odouyfal.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljbgekag.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pljbtzhf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rzrhzgmr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vnfdymjq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bpxxkloq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rhduufkr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bhqixgsd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3sxizostp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxprkte.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hltinpyt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3imuyznvk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ssumeirl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pvbfycxg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fzorcxmz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktluvqyx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3buykiwfy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wuwuedcd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qbkxtyof.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llangtgu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lwxmfhvx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nuwdsxbt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3eaosevbc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cwkydmod.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wrbqflhj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lojuarkx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dgpkjlqg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rzrtvcgd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jesuwown.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rzvpkbti.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3stocvoii.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kqftxxcy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kwwmpolo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3djnihwmb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xzhyydbi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3drgqkvdu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dyfywzbs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhoxwp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3igtauahe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ukfptmjp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmvofkz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3upjfuldu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sloewdyl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bfhmteba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rciwvtlu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rmbvvzqs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jisxkrew.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vklibusw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ydllkovv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rymtupia.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dxixknxp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zzguwjhk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jywynnul.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sjgzvmkz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3uglfwjzt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3flcnyfnx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3khbfgnfu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cjuzgmvs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3avrnmzpt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajbuokzn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pcrrsuzj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dohbxegc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ctlmwihl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3suugvxgj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hpqgxvrh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3waqtnkfy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xgfyyyuc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmgynxpr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3twrlmmyp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3htokwirq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3atuywazc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kavvbewo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xrracauf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pfhhdkcn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nkcxqtfl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wfafnuly.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3egppfqne.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nhgihvbw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dzfujxxw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gzugustf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3cjammopn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vdnausyw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hxgkvdqi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fkzjljen.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mijlgvui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3puqyjoqs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ohrcozto.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fxogxzbn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xlkausnp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lkwmnkqn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3liyvbopk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fopqstbz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rgprusbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ueefvkeu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3hbrzqoqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3axtotkxo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uwvsqxsa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rmmlburi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3upjdfczn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yalduuvn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iufqznan.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zpadtpyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3njpdjarv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qlighcrv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3faunwbpt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tfbroadi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gklppwey.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fjjwdace.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oekrxmew.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dfodgmbf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3uosagcgg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3khfxpmql.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lrekggsy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjyjnond.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3awxmiang.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ksbzsybz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ylcmqizj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pyesvzsu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yfqevpqp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3frlxmryh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zenvhrwa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwchxkza.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3quzckcha.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nyxskzgj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3aynkmzda.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3siwrwket.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fpxjknut.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vhmkwfno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3itbgdkwr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pfbfjzjf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jrblslph.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3attsauok.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dpqckkax.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zpkfhiba.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3okioapem.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nbcnihtb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3grikknxm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qmfpwvof.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hyjjkdnm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3geybgawq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khvtquos.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rypawtyc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmbpkhyi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ykumeids.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcpylaew.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gutnfayz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnuwqcsn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nfgefzcm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uyvfguwq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zuzaccvx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dcuysrvb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3urcodfyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mbkhvfrd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mstaysij.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mtucuypa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtxoydrs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qiznuqhx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lftguezq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qlhrbnor.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3czpyuyde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slqduwup.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gnmsvlvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpcjiyod.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kgrnnmha.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fgqjeblp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hfwlhiva.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3loyeiekr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3smyeoyht.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3synkomwd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gbrsinxt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyuorhsy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zmydxyoe.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vmujigbv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kzhwzpuq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hnigpvkz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3weymaare.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgllzdzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ubschyns.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gsizvhql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nmxievhf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bkwqpsqd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nhgsnutd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fbpaieaw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3criuayys.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cahpqmhn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3agkgviwk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vcbubpfv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjwddyy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uxjzgkoh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kfyskmcj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xxoyzpnp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oqtchnsc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pswzhkjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cuqleiyi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vhaydziz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ystaukve.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kgzgykkr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wsyqzgxe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jtgdwymq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ymagoijp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ohndgkje.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dbcikrio.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vvbmevpv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qnktzswd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eesbgqbr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vbkxutkp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xrfvazfi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3exrmhbel.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vrghepnc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgcldalb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3waknqomg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxyyktvg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eulhttcl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mwyokhzh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qoorpajd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yspemraf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rhyzytnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3efqaelap.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3itvrgjuu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3oahomobp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3oijdsyvn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3plztmeqz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3voxzvnju.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nvodyggd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kqnzuyhu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3apylhzej.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yacfcxuy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3quyrzfuv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3muhrloub.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktqbddfo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bzoyhzdd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3faauxtem.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3auxyklif.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vvcxpbji.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zfcibonf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xenffflg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pmscjjaw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oknffqkr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3taxbwjba.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3patcukaa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkgmdagh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtuikvrj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kczvgvrt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nauvbmxh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3obnwjwmv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jwittigw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zhdjxgqy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3olnyfonq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ocbdrnnh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lyahxeil.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fgdbztxn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqdezqpg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tjnoyjcj.html


<!-- 参考信息 -->