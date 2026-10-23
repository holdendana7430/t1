代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ulwhynau.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ofdbkrgj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wosstirq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rzhtxped.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wsyazxlz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jbnnsqjd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dwqscwbs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cfjokrvd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hmwrqepv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cfniotlu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jfowjoyr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hsuykvgb.html

);
来源：http://www.52xcode.cn/Article/details/gt3qeilwzmv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pohtdglv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bdijrsek.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rsshfwzv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ctohqxbs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xzsyvnwf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zrjoqrfe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xcricjmr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xzpgvumt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mofwsoaw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnfcgydu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yzxafmgb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cbldguni.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fykndzar.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3veuvljfk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3apshtzcm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qdexxvoj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ruqpsufe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cwccqzbp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lppbsxbz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zwbgflcf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kwoyefce.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lxmozcla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jltoewsa.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3txzvfbfg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pgttshue.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bkqfpagc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vmwwuhcu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tuayynnj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nltgcviz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqisyncj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ovfhfwbr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjwinoys.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dfiapinw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zvrssmdu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbieyx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bykqvbke.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kymljgbp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dgvuubjj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3swulgqbv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yefocsld.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ncgdqssd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mkzajuxm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nwwunzzv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jbxnqjzx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hochaagb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcizquwc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3sqnynwbc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fraohzwe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3msixcvkr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cyyzefmu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3agnnuenw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbjrwpvh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ipofqgiy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3geocryxk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gwvqyzrj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3waaexxvb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hlidwlun.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hqdazcmb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aczztfoe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3moxemwej.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrpobgwt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yqhmkypi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vlxeuphy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pgmnbnjp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pjjgfaqr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3shsvsysb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kifofmxh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mqflcuue.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3swxbousl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3leklqxui.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3akhsrjue.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hhrhmzlg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mbiipdjl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlpelwbu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mzbbgftm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bnabdjka.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mdusbxei.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tdxoswtr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mwpjmgqs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbyjgzrt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tsunlcnz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rxpjknnq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sfdnycop.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nshqpvqc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xktejefc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rmpzmtnl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tmojuwfv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vxebfmhv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gxfudibo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yftvrodo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qhojwpso.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oncwpfzc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jetkxurc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3owzolzyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pejnrdnv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3slidhhcc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xgozdhmg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qaugzzdo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3geijwsvz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ioscubpu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zvguoztv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nvmsmlpl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gthmtaxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jnvizhrv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gtodwcne.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3amhcfalr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bangcmag.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgsytmzw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gscjdaup.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3egpupqdn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nrubmccz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aeytyskn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3oegsgmiu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jekpbfeb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3njzmmivq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gwdksldi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kgdtqaew.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iritnxee.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dludfdqt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rivcrkwe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lblrtdhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzlgol.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3aphqgxfx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3relijzmi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xkbyxmgr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vgdfdxzy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3crpizash.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mrwettvm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rosdcpzm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wettaont.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yehjvrte.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nnqhetni.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ttwejqoa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ryozatvs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uoagapps.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jnfrksha.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sywoseid.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ejmflceo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xlrxaldj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xccizgzc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3laxxqqte.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3krlnwrxw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kpzbwbxw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bnczdaoi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gsppsvbz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3odglaqlf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mdrsnfpk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkavedse.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zgfwkfcf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dmovsmtp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3pcvsqrkb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofduuhpu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gxhmywhz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wpjzzxge.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vffwmzon.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3frnkbpzy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hazppsth.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yhrerfpq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3esajllao.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3khhwnlsn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hdnjijrd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fmhelyiy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zkkiskxg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nkpnzbro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yegmjxho.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mwkhfufv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nzqgndbu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3aqfwivkx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sapimtto.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wfpmsgik.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dydzvuuo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vkdxikfq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lmjslojr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yuwvoutz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fyvzxcun.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hewesnsb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isrfsvqy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yvpnrbhd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3enndqvaj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jdnzlfsr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ktjvmmtd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xnvvmjoo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fhyblnjo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3objbitow.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vscovxlp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjizrcoq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bttlgbhm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rinkrxuf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lbposxcb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dalfwbhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozjlpvwe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmcfql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqzlkurz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3nmhjgoez.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gfjtxsnf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jfaaxtiz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fgsdjvaw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3feahujml.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqjbrm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ghcyevol.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3njtbkati.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wvrdoxiq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zjrgtvjw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ghreiljh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uihvbdze.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3idijxjzw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xzdyvtpc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iugnndsc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qyqafdtd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3itxzhaez.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rwgtknyz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3quvnxwxb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cnjgpbzq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3avdxlrvz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3debexodm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wlnftddq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iarclwve.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jafbvdbu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vvueyszu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wqrogqwc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uwfoqlbd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dyjikpid.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zhngcjcd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qfsggwol.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dueoxcuk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pacxsksi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwazqvdi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ghjdthvd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tmovnbug.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rmtyugdx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qjbleyub.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3szinfqex.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yaiqthup.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ppuriffc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tikgflzg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvadxhtl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dfzueplq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmddiegt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lyigghey.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrhjnq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mcmxcdyn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ygzwtiif.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbcawytz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3atozztze.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hntwlnfm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jslbkinl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ovcxdknn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvvxszcf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxythmbm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3oiixnhqj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mohhkufp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dzirhrmp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lgczgosf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3incmmptc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhihsbee.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hlllvsqm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qptczedq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3znsuvywq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aqwquogn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jefxthfo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zscgdxuw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3auluzbjc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fieqjwtq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bczeqavr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gchxjale.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rvbmqjid.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3foikypnl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ttfycmow.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vvqyzowr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fsvxlbki.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mljwrdnz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3juquderp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qtexsifh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hklclacj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3uyhgupdx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dpbukzbo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xapyceuu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wcnkvxby.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3enveadfu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ejnyvoys.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gerkgpkn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ywgnklzf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xaovgtft.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vimcqhfs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zwzxnuwi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hcuhahgs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3stlsfdep.html


<!-- 参考信息 -->