代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ftiozxgd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bdfbvzlq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gzdwrdae.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3oapuijgs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hxyirtux.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gkgkiiuz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3offxxbyn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfcfvwel.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pqmvjqrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3grhptwqk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iwrkfmbk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qzxaraqg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmbeovq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hgqoaerx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3euuohsro.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzljrtfi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ctoaquuh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dmcyzujw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yanclcwh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fwxaqbem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsvgjler.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ndlimhxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuvgckbz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dkftbquf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3toejzjkp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3muglwpum.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xwrncmwq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pyitodpr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bawtpqst.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3owclszpj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fsdbzebk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xfkcdcwt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wjurnwui.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kwcmxyhm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pqfikufl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pphyktns.html

);
来源：http://www.52xcode.cn/Article/details/gt3gerhbjmw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pwmqnohq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ewkxxjlc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ioqfiwnw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yydlopdz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ymdnkjvm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vyuxhjwn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wrejiwcp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xzsjefrd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ppbirdjc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3asvytyga.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xtwejzgx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fuajkhpl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wdlwsste.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bdktymdc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zhepjoxl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dsvlcgkg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xykextsu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tzifjicp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wnugeupn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mjsulibt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ijnheuuc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ffwuqwin.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3csfygpir.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3divnfjgg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nlwednfk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qvdlyqav.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3flfcicli.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xacxukgr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sehctusi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llwishoe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qzbiiahm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ttivzvbl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pmlxhait.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3izvaxscr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bzymcvmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oqtnchuh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oaetiblv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yihexzns.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wmdjfmoy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fzsxoilm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3itrufrvd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jlsomuok.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gooaedou.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tvapupid.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3aopzykdb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewkdwzlr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ovsszrll.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dhyicxnb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kpeqgimk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqocnlaa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tvojonba.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3foyqdvlt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3faxpkppw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubyhlzlo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qgsamrdg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emlmyyau.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ejewethv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hbqqcdgr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ewirtpbp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tlhrspmy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apcnyzig.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ouayatza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3omedyecq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3puucouns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fzcapwhs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nbighyjs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bdbsodjd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tyvrwrpl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ocoymyrg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sdwknxiu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3txenqgeb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3amxjkpkl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jeeauqog.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nenkhxfy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rbcynwgc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nxdiaaud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zyrqximk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tiyltdkd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3moztbjcw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mzdihiuv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cfglcqzn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vsygusxd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxqvpkvy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ifgeehsk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3mzvvyogi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ttrnyvey.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xnlctdma.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ibxwgjcc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3fbppbbci.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ilgkjhhl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3czfcmsmt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ofiwivxe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vcocfslt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ctwbsdar.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dqvmqzva.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3savuscjh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hbchbfol.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ertafqda.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3foicyred.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pfzbnrkx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vdkibhbx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hwiylkpx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xqikxksh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lbqglmwe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3imbowsyu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3abcsiqgq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kofiaayi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qqukxhyc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3uvrshfml.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xcpnxbvx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmvrmy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nebvzwuc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ymgaxnoe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjuwcwj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hjgjncql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vpmelfdp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3moavpdmp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3maobpozu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rqwhngcn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntoblrxc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3slffsmsz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gpuyomfp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3amkapsrt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dpejqmnt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ljibfyff.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3izcsgwvk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kldmurwy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lgatahvh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qrrmieur.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jehldjsv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3emtxzlph.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3boukwtyi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zeexwblc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mczlbqiz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3muirsqmg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3etowluhv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jtfebahr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jwsqqrfy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqvqjhb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3egaehbxy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mozydnom.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tixqtdjo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gjuliczu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jnubpthh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wabwnqjg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3phyrkwen.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3szmwcxku.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mzkqcwsj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3iaikxwsv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ctzqmbep.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ofpduhax.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ajqwnxfk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3buvddnzq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3epksikju.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbayttvz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qdggfucz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ckdroydz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3odizqlbh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vnwjsqwz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3wobpcval.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3vsrjplob.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tenipiev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gwrxclxb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uafcqqhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ypadrvuh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gdrepptt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uxglggeb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sebwqfmj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nkydntnt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qecoqejp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfwqvqis.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhnazukv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvxbmkmb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fbhdblqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqdepgbv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gvsfxtnm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqgoyvpp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jvynhqwi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kydzhkwb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3crulwaai.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nzpbpcsz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qzwhfkcn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tjuoweju.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wbexauxf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xmghenpf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nacqgacn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lvaggrua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tldvbtqu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3djvhitiq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjwdrbuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suseqwgx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3thkekfbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbgmnjag.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pblsglsq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xrtohgjy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hvmmvrvs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qidpljjh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yxvhggta.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lopfeggm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xyowozok.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jaichqbu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mejlltni.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3weswrwpd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jnsavvyw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3plqdlcck.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvoakvhr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxzybxni.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3codbggcv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xfwurzma.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jviipmpz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kdoakkha.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wseybsqw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uuwzymsl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pdaqtlhu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nckqgrzr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fhedcclo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yqevcbqd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pfvphivp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iaupcdyf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ajvhtlcf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulbyggpa.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3utjvndra.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3koyhsnri.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fapiqivv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tlmfnjqv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pnjkuycx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3shwvdaew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bretkads.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3digvglba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nupewrvi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3oambebua.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3onexknvi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ifguisux.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3givwrims.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdfdyerl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwkcdrvf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qhmphewc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yzzjajvh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qtuiiyof.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3agpuyvqk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cgyxmfse.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fueontjz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzurxkkw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3drsuegmf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lineolke.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eypccwdj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qvwebkfr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3onmfempk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dfvlowpa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gpnhwzgk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jnpjdtta.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jegscbxm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oqzvgmvr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gqparvev.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfrihntx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ibetpxhf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xdsjkdyc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sjiawrfl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xxohppwf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wivszyef.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fhmkaebd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bhjgydsc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bikclptr.html


<!-- 参考信息 -->