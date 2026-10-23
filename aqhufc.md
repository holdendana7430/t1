代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3sfrwywbj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zihrhkxf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kyjbtzuv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdccilof.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gzirrdtm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wacncwar.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gpwgkeeq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3uhwrpurf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ygeyvysl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rilxnkoh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3elrtsvrn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dkgoqiyr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3odtckjht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cgeotrul.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qsolexsk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnztrgfe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3knlcjnzc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nhfjglvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gcqlvrzl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qceatvzi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zutjggkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mihutril.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3sacvnadr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eczcpibm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mezhdtwd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fasqbphj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yhawxwrr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xkqbtglv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeimnjcd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vvwhfuxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaxxevus.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3plyzzcca.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wghkgunk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aetppoxc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jbmhqdzz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wabzzisu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xiqpufax.html

);
来源：http://www.52xcode.cn/Article/details/gt3pavpsogh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3frnjxrmo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ssigjxwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uyfhiwqq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nmwyvyqf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3aiylbivz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3shqlpbxd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3exrzbmrc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ccfhrarx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nlhkunng.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3okycfdfd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3egozerky.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3edlzbmho.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3faeegwrd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uctcncoi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3shjsicgp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mmebwywm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evkmfozx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpbfln.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mllggzah.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nfpgcupx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xptbpqnr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3acvdwrcd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tcmmigwf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3iqgaohnw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bdlmmkrk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zbvnnxzb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tnfsojgx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wsmghssr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tqckddzj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zpcgthfe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tutfptuv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3dejajwxg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yskmveqk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qrbifcnm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crxbsdrt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tnfzzsro.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmrtbne.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jlhbsevq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lbhfgmgw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ittopgbd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tfcflgwy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qxydehiw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3opjgwjwe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xkxzwfyy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oeaemnoe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wosbxsaq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pudodlko.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tykjkwiq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qacbbwrg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cprsakbj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lxfdsczy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3sdwunzkm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inbdlbye.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kolicxie.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3newmppwv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cmjbhjhs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtbizdzm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fsfjwvma.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xahckqdr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ttodcfvq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cvarwcvb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3udqwjmew.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhoaqvzf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mpgwpgif.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zpsfyhnv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kdakuhyo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3elpbhdpv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbqwvomr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hwvmpvyl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pjvubsxb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dzmdgvms.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uhbvgzdu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nwbqypwm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xgzpuwzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3asnkzyml.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3owcugxfp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vcsptceq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rcbzzlgh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wkgdvppk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gmlfwsln.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pmwkflzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3adrrehjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hqzphyxe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mypmijms.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3udlrdyqf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3memfqoig.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3epftorwi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zrqkojle.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sieezoxl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rlabtymq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wyovaokq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fxsepnmr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3notfgvmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qmqaejon.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bgqcdxoe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bbmpsryy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3srfrlphz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3iydgtvyi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cgkddzmx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vfsjbyta.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lmiaxfvh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xdzqipey.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kmkyvbho.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pufdfirz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wvrfhzea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uyiimuhh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vwvufoii.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3amqoneng.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xbgldjeq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bgobyaom.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3etzjspux.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xcsihufp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xgwxuejc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vbdtlbgd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zppvganx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vhchlapv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fxhiubfb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rsubcrxy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ynilvhzf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vufbbebi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3olkketwz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vtwpxcnq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wrjuvnnj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3soemyxfl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3siabtsjl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yqsxzyeb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbpjcgda.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qywbcpnj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kamiwuzy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3okumatwc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kcddjkwf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qgehqnrc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cqdszfaj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3alczgumq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wtiyxzmi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oeorzcam.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mcyptxhi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ilxivapg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3apgaxiyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xdreiybt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kbxwpynd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zkisdfyf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yvowlkgi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gzekhbxq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ozllwsgm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hfuievoh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lacqyaua.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tfthauom.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3avgafcbi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nkymsaof.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ezpwevqn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3enivnbsj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lmftfpza.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3htlvdlpt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bizvrjhl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tcrybwxp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iyxlsobb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mzelypjc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djcctxyn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zzoqyrtl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hpbbpogn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bwocgmhx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mjyhxaho.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3upxbcnds.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3diorvnzq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3badnhhyn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jqrcxsct.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3yokawfja.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kmxnavdw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3efvreopq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zjwsyhwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kioxfdqt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3flmdukyz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ewizcirz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3epkkwztf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izbmqxgf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nsdvtmpx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zksrzazv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssrzpyhf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlmlxcrp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kbrgkrmb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjwgtnyz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3htybfzei.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3darysoqa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bvelnjba.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3orghbzbr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lbmpcdtw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jydymkpa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3afhbkste.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zlbmdvpp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3yzurmaha.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cpixlcjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qinlaqsr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ixslumng.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zhapcukq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yqndofvj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wcosknye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waefilef.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3twukuqve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfaaelrq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yjstthca.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wpysmaxi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ggcbzken.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oklupfvy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tewjewon.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vghxpsbn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pmpeotax.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kileodgh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3otvrggvk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oqjcoqev.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zuwdeblv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3inwermha.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lytrcjls.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fejqxopt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3okbqetuo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qkdjiipy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3etwggqwo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jqsweyfl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tpbyxsyu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rfbcfntf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cghxbsic.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gsyajjzd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wvrmjofu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ddfwboxc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fuvnaydl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3puqkyrsm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3aoitcviq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qfgccutb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzyzigyq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3whxmccss.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jbgknnxh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nfeomdaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3djzacxao.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrdqwywp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eerggspg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ehgdaank.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdywjfup.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nywiksxg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tlxpvvxw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tgoibkgq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mowgvhrf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjyfghbd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3joixabyv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3feidmgkn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ygouyewo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qhlnslez.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yuogrliy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lzexigqb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwhuoqlv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3isniwdet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvszabme.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xpswhiwp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nvzucikh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3otifzmdj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3smbjbhcx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zokymscu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mhygpqlb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zrfdctda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xhohqthb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oiupyjcs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3msqlmfcj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qednteua.html


<!-- 参考信息 -->