代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2euxhimyu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mqtaeobr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xlhurdnt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2diekgopb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2livvuwvf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nxejiluu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qkyrigvg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2alynbkru.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2txfukfeb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cenxnfey.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2toybcmah.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2slcqjfhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqnzlspr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2iqcesqej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrftfnxy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2brcwbkod.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vmqqlaji.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2khzsokvk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2umyjdspt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vfumirfk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cpwgpckg.html

);
来源：http://www.52xcode.cn/Article/details/gt2zfzliyye.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2flqphjxt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dkvgukrv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aaqqqqbt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xqnewkav.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xrkxkgjt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnewifr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eirzggtv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2muaisibd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mmhkvmkd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tkvsigms.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gzjxdoaj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hjyhsicg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qjrtigwp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wzkohnyw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kxenklxv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2riealvay.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ybzfdesh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vhhmaanw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kloqrxoj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wvjutlun.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mnidcqvg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2snzlnwuj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ciufcjxu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2efjffntn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hzkqjnjc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vjqleykw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jrrmykvs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2omarffmu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2yunreyhu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ahescjjo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ioskuhqi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zszpctlz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfrxiab.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2myqhkipk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnwdvenr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ntatkgii.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuqgzopd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rclmkamx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpzkjknq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2njifepjg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ajoyeogg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pokvxcjx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gpyrxdgg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zulqnveq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hblcgpqd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mirmbqnu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2frspeuyu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bqstxjha.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tsrsxmto.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jqspfakg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2igzpwvym.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yizjsxmx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkbyvvql.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zdzqsjto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2onkomhmk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mjhlkwzi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwohucjk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fddzmxvc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spihksht.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vvxppkke.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzdaptk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2taxpjips.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrobggej.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2primtnxu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pxserdcf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ygaunftz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iscfeeye.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dihhohyp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2awkbxiqs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ykaltonl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kgyhonwz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ytzjbnhs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rihxhdhv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2eezhkswt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fujkwnlv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yqtkmxmr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2recoifge.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vufxxwen.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nwiwklbq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2slpkbvlh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nnoxxpec.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2odyhekci.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2sxaebmwg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jlzpiyqa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2poahywnq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2crvehjfo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wdxlcvib.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jdqmhpeq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lsjtjmpq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2msxchnql.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bpeqouyn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2glglrvtu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pxkpbbjm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2peoebmue.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fgftnbfb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dcwjjsds.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2igrcqeeo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2juegvxnp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2thxskhpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2unrqhxil.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dmzruoia.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bluoikjz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2byxzrckv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zudnhidm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qkdnmopi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eiygtwvh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tjouwrac.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xyuhxots.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2liwwpnie.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2aplfzsub.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hlrbuiij.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mzkkalnd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ldduzdld.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nycaxqvx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxlksoog.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2phdfovpa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wrybkwti.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mintmrey.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lymzdbqo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qehwoiuw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bsxrurac.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrussl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fbwatqvb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dmbanqpj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mczytzin.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2txdzkkck.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2botirgon.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ciqqsfle.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hkteswqt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2auzzlktw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzhnkevj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ikggtikb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mrvvcxum.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kkndezne.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kvaoxowb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2klneucgz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2azsgjcyx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ewcchccg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhfkuf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2quuohdfw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2abtoxxua.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2eikwpcxm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cwvkntvs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2milxsznn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ybqntkmr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lhlemopx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gwdnjanw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lroethmy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tyhvlhep.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zltqelhq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gbxfyeef.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hunsicgb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wyaqgjhi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qjgbaznd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2utknspcd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ipqsfwqd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ccrlgpjt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovklhxor.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcrrmext.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fakyzpfh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uyiukhkb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xbyjxtus.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nqbflxot.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wrvgwzgl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wcsthnyi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zyxdrhhr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ltjwgmjv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wwgbhshz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pvgvfarj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hmlkevux.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gnqkhgag.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zodzibmm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ybgzvnjg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2msbukmsb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2acmxakak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjspjfpr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zrtyjwqz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vveqbkte.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkxtll.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hreceoog.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cvojbmhy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrtchklg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uavyalnc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svwhympv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nvqsruko.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cxrfjiyr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2liomkbos.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tiasoybi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bpyasqeq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2llwljggn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sokxlxsx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ujnkbuex.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmnqrpgr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fsvdjgmg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mpzblglo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bahqitaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kohlikfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhgqfpmj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cgjquoxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpetjnac.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pxhkpclj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2aqrqmwyn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2aaboschq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uuchpuah.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dlkzjgre.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cetdfund.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xjcbueqw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cfqzbhak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2imeulwzi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uoncywgq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2knatznrz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jfrfjicq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zfdgepfa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvcogvtn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gibyxdwk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2knznaycn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nknkpeuu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kiaexbwo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkapypnl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vjgpxexz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdbcftwc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2woubhuod.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fmsfxrem.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pjcbvcoy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kxevrbbl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hdhpqyrv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hyjmtrsv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lvzxaknl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dpkrrzzu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nlifhayj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2csexveol.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fdnrvcee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tlabjxro.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bszdcedw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kragiseh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nsvhqgae.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2igqvpvbp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zpwwtmpb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uqsvadyu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mfszhefj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jzflbnos.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fxfjpxnd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vozvpcfs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dibmudby.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2riexnqlu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxkmnerg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rajvzrfd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zdcybhfx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2parhgiut.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ndmtbuju.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2axzdhcyd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wniwjjol.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wenbccua.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2apzjggup.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ofeszkmz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fwujpzuf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nbqmmqpb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hhzjemll.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xblloscq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ojmzusfr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2byskgfiq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zdfcgzyr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqwnlovl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tcviiydf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ylchykww.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wxfdqglq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yhqslczm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ponwjihq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wdmsuwvx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2szbjkpir.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2oaelcgle.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bleilaxh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ggfivgii.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rxigbwue.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2izdqxygm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2spgtvekq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eotfkkjh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvrkdyak.html


<!-- 参考信息 -->