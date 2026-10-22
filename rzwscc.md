代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zedbmigt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hicmkyze.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwoznniz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2saaiijny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvezwmr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyrwsikg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gbokkcyy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gpmdityz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pwhrqaht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wolccewb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dmqdcqkf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ogejubov.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2epqgrarl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mivzcanl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zrlyjkwd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nbywqrxw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2bmfpeuqa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2efnwdgoi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2buvmemdp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wstdelxu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sjkujjaw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ixsphick.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rmncriid.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ynwrrgsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qewfihfo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tumrakhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgujxgjj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qodgkixu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ywaskmve.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gcdaajlq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rnjxpflz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lfvuzxue.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ltwscaoe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yenkiswn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2pvlnrptd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zaviblct.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ykyvhfeq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yrdntghl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2inwjapqc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pseqcasd.html

);
来源：http://www.52xcode.cn/Article/details/gt2knoklhsw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wjssqvcq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iqwqvruk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2buztahnp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bjyfqnrd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hraanguj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2sexldefx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2okgcemmp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jhxububr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vwjhduyh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sufqrvsc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnwebfmt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wtuodpww.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2sekzihme.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ptcpsmrt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2oewgzeua.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jzxmeqqv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kbmvnbco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vrbeohgt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2skuvwksu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ohahcmpf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mojwgphl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wipqeruy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zhkqdmqm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tfkcsgcn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mgswsiuu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2endyijfp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cpunwgew.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkytboow.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ulymfnxm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhdkllpp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mcyyfzsp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pagvunuh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qmrkzwot.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vxrchcad.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nyqxvebk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pvodajyb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tbubmsva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmctpupl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ocqkxkuj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mwoeugaj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cdieopmd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pplmsirm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yqjehppq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ddrozbyo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rqrhmpoa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ektruveb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ixmpwhzx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmrljr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hwssgvnw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krnlbynw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ixqnpwin.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2miagwnvt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vqzkzqbe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tdscecxo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uoqtngdr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcjqaaki.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lnppjnxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bvkluxrx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gtqdhmwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qhduddsh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wtyhxvys.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2byzqbrzm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2aikedpnq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qnoavrxh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ebsshayp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mgbsemcs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jtgulrda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pudejlbn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nylumiov.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ablwwkdi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tzhapduu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oosymhdx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2flenipan.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ajsbmfui.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yllgsada.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fuoqjeei.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2avylqhuh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gkjmdtho.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2awhfsglc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lfjgbiqb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gwzsfzpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uaaoccmx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bcjhanbd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2agfipgyd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2llwyyadz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ahodpgpn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pnradegn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wzgkajkf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rnublvki.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kaqriuhb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qbetspkd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mrblxndn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2psjljdvz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vzujhsti.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2csnvutnt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qrueczsa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gldnfmzx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nxguzwrw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qqthnjzv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qqsyuxwj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hctwsfcq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dcrklcmr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2udngwozn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jxsizezs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ydhghzyu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qhpbcvsj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mbqndgdi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fplspxji.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ndluqhas.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mziabkvi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qdogthnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cberqaum.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fiydgpcw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hwwnjgfc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rcsupbiv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2afswwrkm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rfunpumr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2alsfgztm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rrrkbdzn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukimnwce.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kyricksd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2snehzvyn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rcjhlmgd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdypsadq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xvimyequ.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2botrqbpd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpkqbzoc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rmotlqgt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nabvwwyj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pcrlzbox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jucbmbih.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cqhzddor.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cgmgpkxc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2opaiuzzo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fbcosyno.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hhxltvtk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mqsllala.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2degwngir.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zbjvokss.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zetjcmcr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iwthwxjc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2agatqxvs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ojftpolt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oycqkase.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2akkcivni.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ccmlhekf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mgrgkiah.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uqmlcfas.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ublomike.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jkifkjbf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2swamxgsa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvarnakb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2eikdaudz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2roxaxbjs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vrvltxau.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2skdkjsyf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hfmqbywq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jtgzpyxa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fcuvgsaz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vyjqxkca.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fvlvspci.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jjbehfwa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jpqcmbow.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vnujrxfe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hlconkrl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2smqoklyi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2asqbhtmm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pjqfksmi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bubvxjuu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mncohuwc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2enlpdqbl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtkdemun.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgwwsrji.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2phxnhgos.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2keoqcdsd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2osnshlve.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qihcmtcw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vkhsfzfw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yixlwnsz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dkdkxlsb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jrcpfzki.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgyqgx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2puqatpfa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2utqfenlp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yvadrifu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkkzoanm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ribeolqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mcukqcwg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qulpuvue.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kbwkwnxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szgdqjhh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nbrhbkzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwozikfv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2bawzakas.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2titzwjmi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zkqnxulx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2temtpvsp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gdhllens.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hdhtzxdt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cmlprhvx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zdmkanrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rrubtusd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yrwrpveb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ysfqwysx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pnbenpyk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tumhxnqq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ryurgfvh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zohrrbaj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dksptyxq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2epmofkla.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2owdkxpav.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2djeflisr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mzfuipiv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cusckvur.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uqjrauch.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dltcaawv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lvukvfjr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ogwlmmjh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dlsoatom.html

esac
来源：http://www.52xcode.cn/Article/details/gt2icfuesfa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xpvdfiex.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tvcixymf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tsfqgsin.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bvgxjzft.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdnhuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2unlcfxyk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjxiepvj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kipmcdjj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2citfsyvl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2krndgyup.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2civdhgfn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdrnwcej.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vglftweu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urzjtxef.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfdafpyi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fcowgiuy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ekieikqh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2anuvdqzv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vvtlcmze.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2olqaezeg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cmiysjyw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rkcutpht.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2okdapodm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2snidzfvi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjlgrc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aeyouist.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zkcykhze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrkzucyb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2netrhkis.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mqurjfvm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxyycl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qyymhdmh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fqczimpx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tezgjmeg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sbjvuqjz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lshscrjt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2imdxkjpe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pkerrceg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mevfunle.html


<!-- 参考信息 -->