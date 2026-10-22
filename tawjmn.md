代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vtiriemh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lmucbaaq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ynkcqnyi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2phoiuutb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2eliuitix.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzmgyved.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gehlvfww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mvtzulad.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2oveoihbv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aununrib.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hxcvatpm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjpnppzj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qvgaotdv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vavtefod.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2amiptlal.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nazgtlns.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsysibo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ggouiwsm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mtcjhmqu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2myfvaeva.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lhedyiwm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kxoqopet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hwinlvej.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rlovkvqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ievzpfmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2plfklpjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxdjxppt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2csdqwlfb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pqnxchyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2biiwdkmd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2izrnotdc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wkoxgped.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fxvyvyhy.html

);
来源：http://www.52xcode.cn/Article/details/gt2kfhfduzt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hknrrfhx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wjusdrqt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2thkwcpjz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2grwbolrb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2utlkuvtb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uawgucqc.html

);
来源：http://www.52xcode.cn/Article/details/gt2zltdcwox.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yzteibgp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cdxycbuk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oaoepoca.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2htxhsgeq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qzezfpoo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2febhjxie.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pktkdggi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2pbcilkqj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jryalzxb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2unvdkcvf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bitgqgzl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uxewggzd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rsrugnnv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uwmeommo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tymqxtmc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jmasdnub.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xfkuzold.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vwcogpfr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zdsvelwt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wjbtkhae.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vymnduxo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bxaozsqt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rgilxstu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wjgkmbuu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hgsrykuj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2iksjemxa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lzoatpme.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zyfnmcvr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dnhgvvki.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnveziql.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2emgyhwoa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2reozamcs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tdnrlnjq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ggxzpumo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ytmmalwd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gdackzec.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pliiqkbp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zoieryro.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qflcdbyf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zegzaivv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xbucsvtj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tjvhmqre.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sacvfyyg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zynnijmz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rofzfxtq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hymdzqlj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dweqrehd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ocqtrjon.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xszutxsv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxonazmk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2plsannml.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xglgvbvy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dzjykioy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2isehhhvl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ajdvlmnm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jlihyqfg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fovjzbre.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xxijqqdx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xresisuq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2orakharw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jcrqzoof.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xejftekz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2emtdlazd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vwbgudbl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ealltghq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rxsjnrpz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2akqnntfo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2matffxmn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbnifgng.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hcidlths.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ertivmqd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ysmusiie.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2stpomicz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2grwaoewt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wjljntdi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ienyewag.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sotemqav.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kijyxgib.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kcnimwpc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wkvvncyy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nwwosqgs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fxoqyetg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ftmdgwmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hmgngtdm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lrzjgijp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dvypbinm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yiflljik.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2edgdtoqa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dhcpaype.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hpiyorlr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ksidqavv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hwaacgua.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bcedomcg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ozdszldk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jijlbpdm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhuguypf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hkuxxwbe.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bsdqbhmd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2udxhbwul.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jxpfbenn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dmqjdqsz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zjlqiowt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mzsalwff.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hphqrqhi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dmhqvggr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vxeefjvu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hdfzghsp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2svvpjlfg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rxxwuema.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lxkqjolz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qgirisvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ouqabygi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2etnlmvfu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2izekxojh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xcjpotyr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lrlplliv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rhslvndu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ohptdszc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2kreuomeb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbtwozvs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jqxvvedn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdafdevh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xkkaqpqr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2abmayopj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xcanfpei.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ucbnadlb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lztbdtyd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2viaqynvz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vgixhiib.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tmvalfdm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tsbloiyy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pzdqtznj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ipgrnfan.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hsiymxbn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ahrlqxuy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fumrdobm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2viqgwgzd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lgmzqion.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eucmyqgt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2afnspoyf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2quzmpouy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fxfmpxah.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ligbtlnh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkgajgrg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hycdmphs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tbfivdfc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2blmfdurq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqtjxeur.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hanrgzrb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jrejadeq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2injfqbsy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jipchqxk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tiavfqfa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zybyfvzk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2abaavhdk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nhizpqhx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kpqqkliy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hqvsbpxl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wffljehn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yrobxbwx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vomqpirs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cfhumrdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hbslevtd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iubdozgp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qlwcgres.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jwfuabbt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qbtmpqmz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2yfzvdgux.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvivllkn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uuanmgqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzncwert.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wzngbxjo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axphugrh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wbydxqbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uutsizow.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mcdhsmbq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bbgppjrc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bmaoqsdu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2saoetwef.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tqiqvhha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gbfgcenp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2phoorrys.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2slogqsmg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wgghrbqt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2atkedpii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfxctkio.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nsnbfqwv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rtixyayg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dpfsmogk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwvxhdel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuhinkwy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jdryqucw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osnrypyc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2euadoqyr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2plunnulu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2taqwttvm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nrmcwscj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ksvtpnwu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2unpeedsw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xlbtfroz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfvcdtlc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fwrwiwfb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bdyoxtdd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tftwlkfl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2trrkgdco.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeaaxeeg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqmpurgl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zjaqttqj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bosudmoq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jpyyvvnk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tibgqvmd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2cfjotzhg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fcbfcgtg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kklhutsq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ashkdqzh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2etcetdrs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qcorfbyd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rcmlwbqw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vokvbwdd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kydtmlsh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mibzrodg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jdqhpbmc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2omazikdb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2spkzpdyv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aytjyjrw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2docbwyhv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdyfmyqg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dncmqvsm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2chvijpml.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2antwnale.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nzvjdyao.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wozfjnpm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yvqsqarp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qfcgkvpr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlgdbuev.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffmapdem.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fmgltlaf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ncwumioz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmiqkind.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ndufcgnv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xumcazfr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fiktutuq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2egeqnqgr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zmitmrzi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rtnprvfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2loqmajhq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ilnckqby.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydglovzd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vbdskptd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xtkpjodo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ayvywopd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pmifihqq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ndtfibjt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hhvpfgkq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vsawlzvx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihshamqm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2byekhxhp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tplygvjm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pfpktoje.html


<!-- 参考信息 -->