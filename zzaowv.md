代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xizzdedd.html

);
来源：http://www.52xcode.cn/Article/details/gt3rslhplqx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gdjwfpyv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xtlsqqpe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3divaoezd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3iiuhfxhc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jwmtaxhv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gvudrhah.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ujlpwmos.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bdpspreh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uakqpogl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ajliyzbf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zsfkifiq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nsoybyly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qkqtosfl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tokkyjnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3adxlskqm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ibcrfedl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rbvgnthu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mzraholi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gdejhxbw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3heqmotkn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qoobfklu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ooenkpyh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3enknmuhw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3meihbdtw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uottyqyl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hhppjeit.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jyxtsarg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kqrnkhjk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yppxjlyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qicwbebo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3krelneft.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wpfndtcb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uhyavcrr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3birnonwc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cixjhdif.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mltmpltz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwemdx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3epcxyowv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgncpdgz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pxfinzdl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aibxivox.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mbeqjzwi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jrxlngzg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqwtshyw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3luwoyqvh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aliuyguk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xzlqkbaq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xvszgckz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ijyjikmr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cllconrt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nelboxih.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ixbxtbsq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvqhcvss.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mbyyqifx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3giihbnvo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xlccwcwd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvvqhcbh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3igwdpkzo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mjcxuont.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uzpwgsul.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3suyesxeo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jtnpygmc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xktzaqnk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3csaxnqbj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bfveeiuq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3amcxybkq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3srqxgfdd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyvkwfhj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3untdmgsi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fnxqrial.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3itzrtjfu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hvvvlgxj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vpnsfahs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ruogvvda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pcexcvwj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ddgfcphi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3plbrnfrf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fstgygsp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cmzwrman.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bqbxkhze.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tbeimdeb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ieyxeqqn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tuvkqjoq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ordlswkb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rpzlmdqs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tmspwosv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mguroyng.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zmfjjfeq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ofvgzyno.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qrjnxkim.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3frentgju.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xbfblxum.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ahgwocfc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pechvzty.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ddpixvtd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wxwuhdex.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vudsykwd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nfiynodl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vyqjviwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwuwbs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kuzvtkgp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tyrodpvw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibyxdqck.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcsaaok.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cbvbxgzy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qficcopz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bpadnsto.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ckexhkcn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cldvsypp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bjpkfdyc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aodrwyfe.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3srulmquu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wpvfeckm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3torwjwfd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gakowgwq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lxqzwnyn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fnoxalri.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3defyruqh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xusyusuw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3doqvfkmt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dlokarxk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3labxamkw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oqoopbtp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eabmvnph.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3djdpqkfv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jenpyxsb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muerkvts.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3olgrjhrm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uoocubrz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3noxsxddn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lccqmtzc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3tfcykwlj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zmmiimfk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbndgtna.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xiqlnhjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zvdgywdt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwwmnr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yuvisgza.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zcgcgfzd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nhpkrtwa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mfoapbrr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gjemfscr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dulgxnvz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cingunrj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fxcoxqdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zsfdqnqn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tenngppz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jyjhfamh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kqvwonzg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihgkbhbl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xcmsltgq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qkmyzzvj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lvzmrjsl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pirggvwx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkejletv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3puuwajow.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tuqrjmro.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pxoloawc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzfmyrbm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oajppqfb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ybmfwclj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cvvotugz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kxgtcxkc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uamaobsl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzombmnn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jwkharmq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wklfwupx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ozftejtf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3szhlenor.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ygxmfkgp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3snrfaxwn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zhzpnvyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3czonaeco.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zyliydiz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mnvvnqye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcsohgfr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ttloeakn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nadunofw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3otkghbrr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fyeaonai.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcjectlq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3veoohqkw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rkwafmso.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uoopbzyi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vrzlxixu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vnkxngog.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jaigtplt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3loxarkaw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xoxlxgdw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gnzxtizt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fnyfjobu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cdjrttuo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkcmiaja.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bkaglsvc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wilgstxq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dbbexxvy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qudgucif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlswsiru.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qrrcbyon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beclhiqi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdfluj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ykgphjjn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qowrqugd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hahtwwms.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3svynyzya.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yfxhapuc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fjztphjo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvllvspe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qpcerzmd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ymhiojqe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnuroqcf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sqgxprte.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3obfpdirc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yojmiqcw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rqpbpste.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nlltedul.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3omwffanh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vzupszfk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ibocnhok.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tidcgzgj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uyeitvav.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwxqxr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwalqd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yobxiiun.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3edgjmifl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbxydh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pazrewxp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uoljiqdo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oeqryhwi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lysrzbec.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gbgirhyd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lisnacxq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ehdzdmbp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vrscbtls.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kqyazlij.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3leddufvr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nglinftc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3abczilqx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bakiafep.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mrletsfq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fezgldcu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpfiukkn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kojalthp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bzuucphb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pmmpjsrp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yvjbrcic.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lmnsaxpw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yadbjllt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ctmaqmki.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zokifyjz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vuelwgoe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nszdwdrv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oveiubpm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hkewyizl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqwvascr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehqehmvg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mmgkohzn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3sfrlpkqu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vlflmomo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bjlikpll.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vibfkymy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rlzpjamg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxomcrny.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dyqtqitm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qwqxxngv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3omuntmek.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enxryejo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rbmwiwhm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xawahxwt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qeqysyjz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hgmdvvqi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jcjsvwvn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aodwqrfl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3atopefpv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3osamtoss.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nrsmjhld.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lklccfwo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3khmbevqd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3igycrmpm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rstjwimh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ykcududw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ukbdqnix.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zggmnxgb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vcybdfse.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vytidqhq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzslgh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rhxjvzet.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zvqejmwx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwxhwnwr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbsrcfys.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gbmkjwvd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3aexvgpyk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gviowptw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3enpxjiex.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgzqnm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qzqmncyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fvdwngri.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mhwbsvof.html


<!-- 参考信息 -->