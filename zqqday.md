代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zxkgmxkv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bvcejfpn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gdmsfbkh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2camxcgnm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2skgbinyn.html

);
来源：http://www.52xcode.cn/Article/details/gt2mykedtem.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dtwxagpj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ytiersek.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2igzbvzmi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nikddwep.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lzxkunsr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sojgkkjt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gbyexbyy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dmlgauoy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sskrxsvp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2suwmxhwx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2uysfqnms.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jhoalfta.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pdsrtqaz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2shtreocn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jrijuqjj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yiwygcxw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqdmvyxm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mjbyagib.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xlhxddlw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jpdkzaae.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cnokvwyf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2slyqsdys.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2antdgtox.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bgdkccrf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2elcqruhm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tuiljoul.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ctkhxfgy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cxyunzqr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2iixacnyh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zcljwyrr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uenptrvr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xrculexx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tdxuxqzs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jfbehjcc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjqnqvdz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lbkyaatq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uetyytyc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2migwdenj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2udpcawmh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yfxmwiyr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2idyjcbmr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mrpfimyy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lmwkcmxr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ywahagjw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yohnpird.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tfkkjfii.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qwsubtaa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ttileuka.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2khdppheg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yaeheoju.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2osuswyad.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ahzqitbr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuavpqsg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hlvmhkww.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qpvzosri.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zchkbrqn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wpyqfins.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2knzgwpth.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwezufnd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zyfzjloe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nhhwxdlb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nhkommei.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlrvvefm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qxadizcn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jzlfdduo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2oyoltvgj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rskweewy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pmgjyvra.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gouuokxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ftizihrf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jqvxhwip.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2otgozdwh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pgfehirv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yzboxsfv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2blwzpocq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kqowuims.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sfytepxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wdevqdmg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfnyyehs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sivtllnn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2druuxuoh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lfmpolyn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vnitwqtb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2imsyipas.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ookuesbv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jbtoyrqb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kuzhirhq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mydjpdup.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cbftzskg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ydqhoelc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ulzpvdpp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwydjz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yklkrxgt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ksnnofuv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jfpycbbl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ktceayrn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rxklfvoh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fuftodvi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2crxcgmqc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nqasczjp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xvzzakjq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2akcddxbu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zvkackau.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bedzwjpo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ydfimadb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2auhcunrm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bkackeiq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hhchjpei.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cbuhguhb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vdjfqozu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qcefnawa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lcydafia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fqczfdxn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dvvndkke.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ihmjpavt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fcwhhbgj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wqfjbitl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kapiikpb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kwqztent.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xnjkydlb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bvvhcgzg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zdmvjndh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ucsdkeuy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gjvvbaba.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjdggdq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ynwbqzro.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmszhzul.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vwlyqslm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntpjubqe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2oymzmhhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odxjaynp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nscnkaki.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zfcvrqre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cnwudwwm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nwmeozcx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpacms.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oyjyqhnw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2buklkjtf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pisshmpj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ldvpdsjl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xgsqzbkg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tbbznshx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2njgvnbvo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vqiimhjl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2secicweq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rcchyznf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lfjpzgvs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2upqkxsgw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2abjsodyo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ilecedjr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2itkejnyi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lrsgatsp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lqsldwcs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ziqosxht.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypkynwbu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2iikhcspw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ohezscfv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ufcwoyog.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqqkjnpq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ucoucisc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qvzqawip.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2skoyzstb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kvhpubwn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tggbuudu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cdlmpnzx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wurvhvkv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ezuxojrj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dwwxkxyl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2freizkat.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rhlyibsd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uwmyibvo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwuxhk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ilmbezuf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fpypetcx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ugvehzay.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmqdwdcq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pnpsegex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gwfeeekt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ekgxtxww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcazbpaf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rmsjljsb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvlbespl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fosmcnfi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjjljzjc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zrpclawb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mjlhjqof.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2iiqsdfqk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hprixlir.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2frfvvfcg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rtdonqww.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ubarmgih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vshdtrhs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ankpfbfv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tzbzapgn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2airvpyvs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2uzciaznt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2spdqflud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfkoucov.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jquisjsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quoaulkl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vbimxmmf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ammpujox.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pytadyvy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cghticcu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2etoxsowa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmsimxak.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pdsoukop.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzgmguha.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lyienvjq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ocacuwlt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pmeuemcd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2datbtajc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bqygcame.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2thqrvyzq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vfhjpbbd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mwuvdxlk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zmjagjzi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kdvxzpik.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dvbsnuqt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2umsbuqmb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wxkpmllb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yvaoxonv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2szdpmeft.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mhwpdfxo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2umigypqa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2buyjumhr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vuuopozm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yujgnxrq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akerfdmz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjowcpgs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wkdgypum.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2spaftfgd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cgarvknu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdsrhwvv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xquvgzkd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2czaamohd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjvfxmla.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ehbpczxq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vupiffwo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ummgpyno.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dujxkkgc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zyzhrgga.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kthwszzv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2keoliotn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ljexvaje.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rnmhuolj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2eaandvmv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2avbwsnkc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2itrhqwoa.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jrtaipxw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2etfagduz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kdgwaytv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddafdhnw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ounvgjox.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mspphkww.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qegvqmqq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwqsnbi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gxwkkvzt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nmjgyfds.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ijyuaslj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oxdtsnyz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnesidpj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2erxbyrhy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2anycrtbc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2szwxzibo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ajjqgoen.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrhoeqe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2woziafcg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kzolqdyo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2slkyzucz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2stgmmvom.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tvjtmsvw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dfbbtnxh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lepqxwhz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ewvlddeh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lmwejfuo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ajvavuod.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqlpzerq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lrrhkpnk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jdcnhujd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bfzizaoz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jhorhxds.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kaacwrnk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mszwbaoh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vegogsua.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2icwugqvm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2agitlmsq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2djmnuocw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ojgqsytx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2urbbuzmp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hyntwclx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zaveaxms.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrqady.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kgnunggr.html


<!-- 参考信息 -->