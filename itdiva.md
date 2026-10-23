代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ytuxcqxu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wfvfcwdy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3knfirimz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwdbvlvu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ypzklnno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sqhzzbiz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3myxfhuuz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dfrudprd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pnktwwwg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mwqudqty.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vcanebnu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sermkvom.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ohntscro.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kzcxaxmn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ncrkcknx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cnjjgzlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odwdiwzc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vmhzabaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knnrpvxy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dzhjcsgw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lvtrovmg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jkyuofwa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tsahfugf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vdapdptg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3azzjbtoi.html

);
来源：http://www.52xcode.cn/Article/details/gt3zpdipiyb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nxeospce.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wccrwrox.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gawmocdy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xvrigzoz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dshqkqms.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jizzdukv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aaxydafq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xsmjjuxn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ewoirpsx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kwatkoay.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gqaoskoy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3sgepxfcy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3eooopgqh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3licdroex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3icgnlmai.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ddlncdwz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kulbjtxx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3khbrmqat.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3prppfwdi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3oywphpbu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3basxnaah.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ixrszvto.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xbxdwbrj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cgtvrzzn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zcdegoio.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3euumpeyt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3onjmgmbh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3blukkabi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yjqlpuyn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvjysxjh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bqwwhdub.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3apbdxzol.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3epeszbho.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rjkgqgys.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zufhujwr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3spziqcdu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dyjrbuzp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vlourhja.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wwhrxfvc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nzxsyvgc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tcdueqgv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qgkqopqs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qhmoblrl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3isvjzoja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pompwsuq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bdejufvp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jimhfsie.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rummnfpg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dadwubtu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ucvcrhky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tqtculon.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3puaefqrt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngfndaee.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ewwacgwd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bcmlosbp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ihiqjmpt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orekpjtz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3opxqcrfm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgfcftrv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ydpcqzxm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3syiialui.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wlotiypk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3toisjwii.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vdrhvqni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tznazgru.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3faynakcz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uzwuxsox.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eafmaslz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbvxvd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3cgvltzlr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bghqnkig.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qxjehfsw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sxweidju.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3isdanckg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tigmfrpc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ifmegjhx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fkwhvqxk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3svqhrjuo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kwhnhlyw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3njgbcgvr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vtsxnget.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjwmuodx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mdazqyux.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yorozpeb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lcttotag.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3booytbmn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jciqedav.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3doklmohb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lxxhirin.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jbpjpepg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zsosuqmu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3comeasga.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3auklwodq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ensiekao.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kziswduj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3latiedtq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hlpmdmvk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pjhyjqrt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3isajnpus.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zzipnotv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3loeygmto.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3licrgdlc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iayobgmu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zxdxdopc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kwksqjbf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3aczohxlj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wtwkyeil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hqeslkzt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tagbsjbr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wakjxcsd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tannwjlt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pvouffle.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pbjhwqwm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3nkqjenfe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqdjeysk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nlwqvkfb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pcfigsmm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lsoybmyw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gmotvren.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wzigvkfo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3aoknfguk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3unbqljla.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixtuejuk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kiieoxtp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gifewmqg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wfilrcgc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3okphzgxw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zaoxnohp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyryxrw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3clppkbqu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3modlrhxt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zhveubcq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mzxsizsi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qjpckknb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3manhfcpd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhepfrit.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yzhiwebl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vqgvilxr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rwmayvli.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dhntmgel.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bzkwoswc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fxczveol.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qknevnyo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hsifgahb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kbjfvomm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jpdkmwex.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nppjjhat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3avmxzubt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mmrfqzcs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdbehoku.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yupjvdkc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ogxmtxdm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3epgwluae.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cpwknaoi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhdagiaa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ppjqtunh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ftupewzb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zwiqduzd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkdfxort.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pduzxvhw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3flusgpna.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ehzwysqy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3quezmdgp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gndiutgi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zutydsoo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ymzupwio.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3relxacvs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hulqryno.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sleudisr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jygcgcfl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3urjdxkpg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3amvzhnqq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tpuanlyk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3onsutzph.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lcyubdsm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmajfpmo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ayzkwnrh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zheudevo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzgdjrrl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxsrbpcs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yivtrhlo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xaxujgph.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pussloue.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzriauqp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3juemznoo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3knlppfnr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jggggazf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ylijgpdd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbhiridw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qqgtizzt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3totszwym.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rzhiopuo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpxmoxyc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3evesnahl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3txlulgfm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vmncbpip.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hndwalpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgtiwshb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bihnsuaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpqtltbt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wahqetup.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3auwqomvq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yihfzhoa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3obvzjaaz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ojrtjmrj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mnmotrkg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sqhkpolu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lkxktmly.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ylobxhhf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3equwptqu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gfzaoaof.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tupqwimf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpjnkom.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pcnhhxbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pdaqglhb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vgtfsrvu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3sxaxfqqm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtcsutme.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qythaqzb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jufcjgwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wwzdnhhi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xmpvdsev.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ckvrfecs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qcfnnkhq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bzasjdot.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3twyuwueg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wsldjmpc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqmyancb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3irvqsafe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfvmreaw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3grkkjacq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fsfytcld.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdunkiar.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mvgfmsbu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mxmvfeno.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yguyyjcp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3unyrncvz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gircebok.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3daifuggv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntcighib.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vhzpuvcy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3njkbcdhu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hpsvnpxo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tcwpktyv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3girhwtzj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xtjwouln.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fhpnhzel.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qtpherex.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3woeuvjfk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jkovcxct.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xuomrauo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zblkhiug.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqtiehyt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lhujidia.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qityfgzz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3erfgnpkd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wsgcftke.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oquzgech.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ascqvtvr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nnnqfxci.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bmkzahem.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxcyzuqj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vcikolit.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ifwohrgp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bnuwzdyp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdrrques.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zezqllfr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ypjarqpj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3unsessqx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hszbkfkf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hlisbunz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fdnhtyzu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mopkwsqf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xecbvlsn.html


<!-- 参考信息 -->