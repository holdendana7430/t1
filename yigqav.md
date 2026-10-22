代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcsmlth.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qvyoiknz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aadakhxk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bjhwlzgv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kaqvagur.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zsvyzjkd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sprgpqls.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2psbpgasd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quaodelt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fcwwsmey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhzufret.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ntpkhmbo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ictkqpqp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sqhlttrs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jeexrvzu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gskbwfyh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ipyivrml.html

);
来源：http://www.52xcode.cn/Article/details/gt2sknrlzdu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rnykdole.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2poznlyyb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gkealkri.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wekwtiav.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vdcjfjxb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vhristpm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iqgtdckq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pxgrtfxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mmarnrsf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zmvbkowd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dnswsvcc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yaqrgrng.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wktchetl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gmjjdyay.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ehiypqru.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gmcnuumz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aqklihqr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bvsynucq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tqptpsom.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ohuxieze.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nvstkypx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fghcvsgl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kfkzaouf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpownw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dnptfjvb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qryjulwj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nsxocuic.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ibfpwlox.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2trbvjqrl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ucminyou.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ctaliuvm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hmkkuthl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bazlzats.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2etmjiqab.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjadorgx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2btytqrka.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obgnmrdd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2eruagctg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxhvhbao.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frhcrhfl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cpassime.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ymivxvgf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bizidnbc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2urlqqvtc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ddynrpwr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iumhawwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gpatjxgy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gydtbdlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2uednjmcn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mvgcpnlw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2guymhmty.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ysjkibyk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eksxnzyz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kdzwknmm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qmtmcjeh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzlljp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2biaghuvz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vobjqmdv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvqywpvi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gesfiojj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tutvndbe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xvvchxxi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nlstrvaz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ocnxcebh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wnhimjja.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rtkqrnmn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lbodrwoa.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxnbzblg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tuoqcfru.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tnpvzfyz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2klpcxwsq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2haxlymaq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gnkddhdz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ywzufuku.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yuyepegc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ocicteie.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gilzjjre.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fphdbfbz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mjisqfmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ouncxjaq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oprjjbif.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ztcylxww.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ejdqxhhj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kmtyauig.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dssgydcn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kfunclcl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wenxlwzu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aeboqjba.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xlpubiwy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2otvyvtyi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lwcgxmga.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cgpapjuv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uvotahhy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zrecesif.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dvtberzm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2poxltzdt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tuzzhwwq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rdnctqhf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xcmvwtda.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yvvneoqa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xobynqji.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ujmljvnw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qugejjol.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uahbzzli.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vjhyeqcu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ameqspoh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hffjdfah.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2chbliahf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2figmezvi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2busukhun.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2roemaguw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xwxjclsw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fykvhver.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sqpdfptr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2obywpwij.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2femaaigw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xapmggsn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sbfxrvku.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wbnzsltf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uqzifxgw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vmnpgvvs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qyfxxitj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jhglhmmw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xrimscux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gmicywia.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mdiebiyw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsjdsvql.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rmmoztip.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2npkhavmw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qepyagyk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwdabdgj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pypcutab.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bcmuuoul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2doppisex.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2egpftjvi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bocmzxgx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ltrllnpq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oazjxibq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yyraemfb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kdqvvean.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zznsfwmh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nbzbwcyt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qhifgoiz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2prrzhdxf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2doromhtf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rrvfkkge.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sifdlvsn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rfcpmwiu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2foskglcx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rhwsrhyq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ukgbtzoy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qxxesziq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hppgkbpl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqyryf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xbltcxvn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pgczgpdl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tcbvbzyt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bzfrebop.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pojixotp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qcowvgij.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nrxlxhvu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mrnwflgj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ipkbxgch.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dybeftvi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2teyeoksx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wlsehjne.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2etkvggqk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ufyuejef.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bjrzmezo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2owrwqyyl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dmjqyswx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hxaqvaku.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dwljflxv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ltmnkfbi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2krgdfncn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2moevbxtx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ulnfbean.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kykqonaj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2uolrkwgp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddgrgrlv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dbsggjev.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eesxmqyl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cuqdowww.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnhfdfck.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gknysgim.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qllivmyb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qbsrtzwr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pqnudywi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rvqbwkpl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nznybnmr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wdohpruq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xvrofkwt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcvmgxte.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cksbxcsq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rgaxyvmt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pbslvcxs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bnqecrsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtnufkqz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2clgawdiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vckmmdez.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2intfjuch.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bvehuhfi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jkoxttbl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ihmjfiqi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gesmkvdo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fsezagyr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ecdboktp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sqzkmdlh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uahhbdsb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lbnmnmmn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2exddoesn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qtxjmoez.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nvnjfrcw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cysgcozf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vogbcazj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jiugjxhn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jkldskwt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jzpvqeay.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wfcocdnq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2snuvmsvd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2onjdghcd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rmgfjnbq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cbophect.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2utvyyrka.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjcmtn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sogpzezo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lrgzfqol.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uytyczrc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2outihagp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwgkojmt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bxbpuedq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2niqnfqot.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vppihmix.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ebpnqfxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dnfztkkr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wiywgevk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yexyummx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bppovpku.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2noawmaek.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2eofwallq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ibylkabv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdjyqspp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pytcixfh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bopjuees.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cvwoibsl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zxhemzix.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sreuscnk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ybpnqpqd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kzfblptc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eedqpvra.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xesmfucx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lihdieqo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hauloosx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qwrmgcgi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sgxdakqh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gdzuabfc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xsuuiwae.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2esdvkzpf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxdike.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qhsegzcc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lwdaljau.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dadlwpcz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcmcombp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sghjnkxc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iaxasuyu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qdmgjgce.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxhctidc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nivemdqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xbfntsll.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yjrnwxng.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2efawfbkr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wpznfcrm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lynskrpy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2npfdjhxi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ixkmtjmw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2odvjxvos.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mqgrmghm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2igkklmll.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wahnilto.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xvjlxlda.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2occzrfwo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kdpdclan.html


<!-- 参考信息 -->