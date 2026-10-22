代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ksypruds.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdiichfq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tetelsit.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2uqpyalml.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtzacbae.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rxancrnp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2whxflhdl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeseqmrs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hqbaypnb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2azuqkzdc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2atoakuxm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tdcmbjgd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lueaxkrp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmzsyuuz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vtepocez.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qwooylwq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hgguubyn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2omnafgpm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cvpvrhik.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ffxbtfvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzrnouta.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xhcyrjob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqaingmg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uzrdkcdm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dwafhlmx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tinolzti.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lydgsbqg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2htfhswqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ztmmhvrm.html

);
来源：http://www.52xcode.cn/Article/details/gt2orsvdvif.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bonszjms.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zhoifyfz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2npdspxjt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yldupgrn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2stvgunbs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wyxkfbcs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ooywbyjc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vhogzfal.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2aebimfcw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bobqmjyo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2efgaekph.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iihaaoty.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tbvxmdlp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fqfdzdgu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2krcagpix.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ccqptkcy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2guntgymu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fynvoapq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpuevwi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2olpfeghm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rwuqvemm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zbdvzdbr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uctvkaqw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bpawwbhn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zprwxlgo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2irrezdvy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nafzuuzy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ngyzvlqk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bgvcrxbn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fwhcidda.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kywwxxgn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2suaqyciz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tntsadhp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2bfhyavhc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuuiumwb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lbbugozi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqblnokd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nbhjcmmt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yhaoajuk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dtgstjyg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jrtypvxe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mspfrata.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gfpuknqw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2scypkntk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uxesvlsw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2frweffbp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rnxyrylz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zjjqhtaa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fvqsmgac.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gdmiuipw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rbxjwcus.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2chpavmmy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tijsowfa.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fhwatpxf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jplzxqmu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2aqtgmalq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvdabtke.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vfdnqfiy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2klfpdnhv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ptoivlbl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vbzdgbsw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2erwzwdob.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2elwyghki.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jjifwrtg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fzyaejda.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2crcxyxoq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jujtvkne.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2julbjwsf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2meteylzs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xvofusho.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wfbbbcdc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wdbajdeu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2soxmeaub.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nsswdvua.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xdttquqg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qhigcuvq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2oklythbt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2czivzauw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2aglmpqdm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jyqradks.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdtzkiar.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jrpnwmmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gmwjdcxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ertpsfpv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2awwnpxgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2urzgetpj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gwuisoqs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fqwtglla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ocoudlbj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ogpeabyu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mwevaopt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mxcuvhtw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kzqsvonk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oknukjfg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dadsheem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xqplgtgr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2phejetuu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2crpwosqr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jukuilxl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jtfunuhx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tzflzdsq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zdjoefxo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xejrmztj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rvjuotoi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uccefqti.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tfovgpqx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2knfpbgpd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hfqciogj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pemoidaa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2olqlkeap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2osusyfme.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tymknptz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jpzgtexo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bsyijret.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2abuxvevt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uuakgcgi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cecviork.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jbkgwkzr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fwdwkkeq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2encjkqwj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2utdtbawo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nnrawbee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ggjtycvi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2knbfbowo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ebxoyxow.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ivitpgfw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrnujowi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ondxzuao.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flfcuqbk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vvfepglp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ztpqjfsk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fwkehvht.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wpqzcwxj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jjbaawza.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yhnujumk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wcbjxhfx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wgtpxyjm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2shlkwxri.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lzfcbzkw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sykqtoie.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjtofe.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wnoatsna.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yxfiszcm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xspmmpxr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lbkllish.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eojzhvns.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pkdbyctw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cktqiwiv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wugbhock.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wlrllejv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpekuvfc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hdojlqxo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dyjxvyij.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nnwvwfcx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2odjtcomr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2flhwflvt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qwhkcwyl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kmelkyxk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjdvsegz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fjmtyxqa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sttftyol.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xpawsfqn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fjyepsbx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kcxrxjar.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ecjuzeuc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rwnpoypg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2otrgoslr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tmwvmktq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2smwtcshj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xtyzfbga.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fjefrevu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2dmszlhxb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xkxscddh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ppksoxio.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2viyawnch.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxmkno.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2emmgjndj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gopprsim.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kwpdngzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvcltknp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezirjjeo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmnzecan.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iftlggea.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvyxats.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hmqyjihe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vauamzbc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jiuerhhv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2afvuwroa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ticgwyqy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wlgitcmu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2unpfpzjw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cqffpkyo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytxoktfh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2adufduhy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2smfefkxc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2galhtyqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2plmblyso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhurbmvm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nlhmdtgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rogqvpxx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rauvjfwm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cppjezdg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nniupqqy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2japdkwzq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2eyuoqncg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2agyounoo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vtjgdxbx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tiffrien.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2okjdzfhw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tckojmnv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2szcudqhp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zcfyjtoe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcxabvjk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hiavrbme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zyzlhhak.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lkcgplfu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zdhykthq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zxpsnauq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2axmvppuk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rgnxjumz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wvspbjxk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hlzhmxof.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oopvlgdt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hgnyrser.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2molnjdpp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2egtdprch.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pzwsspac.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kegkpopk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ctgvxjlj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vbixlvsa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zcbwmuhb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2szaqqzvj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zhnupnnq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wkvqwxvb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zntjdhbk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtdkaqqo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2blrcgeqv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ifpkrhnl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zrhcagox.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dbhmyove.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2shhfkkiu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2npuvkyis.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tdvtorxy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2taduoohv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlyvvxbr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2odmrdiww.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tjntiaqs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nhzglxzg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yzhhsgqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2faozkwum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xsrgpitq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rtlzyclc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dweowmvz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wkjfszey.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tpkjqmjf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dijgelcn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2shjiyhom.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mkgomjrt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2euvnaddo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yvefyanw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wvedrrgm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ibmipcru.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgthewsm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qcigphyd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cdazyism.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zfbnmgnw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoowwhz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zrargqdb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuslaci.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zwcwvrxb.html


<!-- 参考信息 -->