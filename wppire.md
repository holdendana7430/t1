代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vstrghkq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ufdjlylq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rtwtvyql.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3becctjlq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rcarjeai.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xmgnmvki.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uwoacsrb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3avekrdng.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mjamgmat.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ikvqtdix.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kclggyco.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zwzbgzdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbwdruhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uyoyegqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozwuibhx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ftcjnebp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kuapzrsu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ylebcyeq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oplecnmd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gynlpblt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xmyssftu.html

);
来源：http://www.52xcode.cn/Article/details/gt3pdslvglk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3leqohjqj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fqernydg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zvnpzahl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pllzbrza.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hfaqkkom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bfemyhrz.html

);
来源：http://www.52xcode.cn/Article/details/gt3gzwjsaqd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dzrmlbfn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gaswtylg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3iogobjve.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uxzgwskp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qnbanfay.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rxcrhady.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3svgctdsg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3eqygvnbf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3znqmrnwt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sjljahqr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3axkbztfp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mfzslscc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tuaxfqtn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rtnovunj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqebly.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oxpssrop.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3afafgsee.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tfbnjwhp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mhrsuxnq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xwemyxea.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rgmtlpwp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cjqiwovx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cixxbnjt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pthysmkg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3btgcdjqu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3nllxhfwo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gbnpzmnk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jkelghva.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wnfmefti.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvfoyozr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tdqlrrhq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zjsjrwgo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vvbxhapd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3buujicwt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ocusgdej.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3obiehlre.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3oevhepbe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qwoxomqb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rsmrfsyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ptdydrqn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bsnylgpb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fkxrcvam.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3izspbjaa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fhysnoom.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jxobdcxm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lumpccli.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3afrvwslm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vyngfqbc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3njcjcsfu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdkfoiwb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uouwdmjo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jzqmzbge.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wzshvxhw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ihdawupp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qurywluf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezdxsiom.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hpdvezvy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxvupk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ecvklkrs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yohwmmfv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umsumfva.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nefdhnmw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3obyolqnc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tsybxgti.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ufjmmckx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mtyszqzu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dylmbtvo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3kftayacj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uvlircog.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wnovdzgj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3svhathlg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nzwccyrk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hfeiqfrb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qejgheid.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ledbkvbk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pomaakvx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zflvoobn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3pkhgdgon.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fvokleyj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3svhtddwn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ooxhrrbc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pvuxaujq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3obyssahm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3drlwvsbe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qkjaynft.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vouuream.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tpayoakd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qyqoimyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gfdfdrhb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mdldokod.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dpcnyhuq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bduhmmff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3biaqagfe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lndsfiif.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mvwhzatd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3lwxhwcfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hcbeokuw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3owyzdhmk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rtsfpody.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nccvvhgs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhrrhpc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wkpgejhe.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lrfzcxfo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrcrhft.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nfdwylhy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3poixrqgt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jxviqaxw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zzgyablj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3oaashnqu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3izosajih.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rwzcywtv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bkgqbgrg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3voycgemr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wvmvvwfe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cnjlmvpw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ksagtzja.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mibzikyi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kjomxyzs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3opoawkwc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsvrpxye.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pnexarnp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srhajrzl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ebgxsilo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mrxiryty.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mgtkxbnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3isjdcvqj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eosdsgew.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wrmxsurk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oiedtbhq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jggtdsur.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cqvncloy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zfrazsst.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kzggvnys.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zqygetrl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3aueixpgw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kbbozcsk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bavoszbm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uverfuqj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mzsrzaih.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fygxjsav.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ukmbfcpe.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xwxeosjf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wbkvikjd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3afkthnaa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3duqesqcr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vqzgiyzr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3oekdtcox.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xfxqylvq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3cztlzqnc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3abehhtku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3suxcbpni.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3plnhszjh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3osszoidc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vfwhkwbt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovejrgya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gusfcovx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jvgwywfh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lxquuyal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pufbdhot.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vnuncugd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hksbxkzi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3smxnjjfc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fkblwsts.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pmrwaqrm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vawgmbjv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vttfbcoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fuoxttrc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nuhatxmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ryojybsm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yidnlgwm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbgxcpwl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xavywhgx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqaaxhxw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3thcctlcc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djzcradq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pazleybk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjwetqzc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rvquwumv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3peztebov.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3nhpcmapo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fkglixoo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxsyhcrn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gofmcjyb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kkwyxjxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dnrhuker.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bgnikyew.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3efdnbbyq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xbqxevmk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ksxkmflg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kpbtjhsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktwgzdbl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3exnkfbvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taltavyg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ybhhilat.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jzzbhgty.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mritntlu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ddwoyuhy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lrhpzqzf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lwnedhqs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mdezuxzp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxbkkusc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wzzkflew.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xxjnoqjg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrqhwngw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fopczoxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rbgulcfo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmgztysz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xnltvcjj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ysbdxwbc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ijlbkncv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyfpobog.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fvtwmisn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzkipejr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rpqkqrjq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pmtpqpwg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ssaojeto.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3btastsqd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pyxjanak.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sttnbfaw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rrkhxccp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxrbmody.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3thribvna.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3itqomovf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uxyyawmt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dwejqbbr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdsunsld.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcrzgtyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkbbdylx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3alzsjllg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ueeacdpp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3miciyfsw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nznlmjys.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ofbcbozl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ocadlxef.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3okjawmgy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnqkeuhl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jrlsnmec.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xnewkhts.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdchrese.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3joexbavr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tzijreut.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sckprwyu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kexmyjaw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ovlpwspi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rdrkijbl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vleavtdb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3evrdcurg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wirwduuv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yldnfnfm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ciywimlx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hqnbxvdh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pnlbnpsn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hfsocmcr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ahjceqjb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qkoqmqbf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ikdpvbrd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kedyaups.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xdkqsmxm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzvizznk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoipitrm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3seseiuuv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkjgpf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qrnvfhgh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nvrwhvzc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3etttrbtb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uzhwmplz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bysxmwol.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eclpgodc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xngpvpte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3alhdghev.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3friqobjq.html


<!-- 参考信息 -->