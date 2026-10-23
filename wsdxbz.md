代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkikdt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekbwlwjs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zzgyopev.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kjexvjhc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ovblvdtz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tiihjgew.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3bwrbjojc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bsxokegl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oyzlhnzm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bgvmdptq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gigfxfbp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3etvofujd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3nehgscqd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jrlhgmjv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ooahprrm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xvolzkkv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qrjynulh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tmzonioa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qbblhzva.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iwlhauzv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bpqrddxv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3iqbesyex.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pxogfaas.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oigtvccg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddhozerm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qtdnjjix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjfwfjsz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xdnzlkpy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3otycgcvd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lurjhqms.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3quvdomlo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nwbqrgvx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3orwfqerm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3brabudaz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3sqrlbxca.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gueucmui.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kqlajerw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sildktjz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qaludacg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3daxcrred.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dnlkbrff.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kpxebhdb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttulgmom.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxhsglch.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ovxzeutp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fhebpqrb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xaazkdkp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ylxndaqn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hlcdptok.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3yrbfxksx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3upvtuoyd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cllnrlqx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ikmuovsn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zpqyjhnk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lybnznbe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ioryaear.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hsdqvfet.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3oicipsyy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kcmarmnk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3epdhacdb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qeutuzom.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ckmiouck.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gsyvrfrb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gmggrlgq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pbcppsdk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kdnoqrxw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kmgyuyrj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rnlmzytz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tqmlibuh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3psqmgugy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xnnppqni.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3cvajsndj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qanuxhxc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vhoevfvi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wamglonf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjeawost.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tanyvryo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ovusvmtj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wjheqyxq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nccnjhlr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3azxtswlx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3eniyttoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cajvxfgs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3imxoyejw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ofgzltsb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vcnqjpda.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fsaekvem.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lltcqobz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bnahmaic.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ajvqztnz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmwnnixi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hnfnbtdt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjeurnf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rleqtwxw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ohppjlqi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ffriqvqp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvkpwnzk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pnfufsmy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yyxeievy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gllyaocw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nkbrmvhm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmuhuyyd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3agkvqreu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3sccnfwkw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jcryojpn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rrijnsof.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3iojexizs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kcqmabcc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bgydlpgz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jvcrerya.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3frpbfkrq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uvsdhhhk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kcmhetqb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bogadrlg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ofhroydc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jhfueugw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ztvryyth.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3niikzqlq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3huzrqjxu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kagalada.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3koygrcnu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlpfhy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pgtimhwf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3stpywmcd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bbwsjogb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3admkmutu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dddpmpxx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ikoclbfr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eybvhnxb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hijgyhqj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jnismqrz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hrlueszm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jmkgtrxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yjzlvfca.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ketdxgfc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cbrprtwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rpsmxukz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uphgmypn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bztgkuaw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3efddvbxz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wrwloctt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ndxmlsur.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cebtrxcn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pzlvweaq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nxpdiejc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fjcdkrqh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mgqkexmj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rtgxfgjn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xaxykuyp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xehmfzlx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3btendbmo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lmsbwfli.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3serfqlrq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yhmaxwbd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3edsockgq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iecqamxa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ecehwkac.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ycfblzys.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vprusakm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bhtzzldb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3phjsnuqc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hfeyaiaz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vfrbnwpq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ydtiancy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3knybktpp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yvdfxfxh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3chpfwqsu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fmjuwjah.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bhkshnhl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wuavsbgo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yfpousmk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dzwtrfyl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wgubvobs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gqzqljjk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ycyqpfgw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zjvididg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3naouvegf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pklotjrh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3orwzvdec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3euqfzbus.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zkemqimu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wbdmhgmn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3quritbmp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ucnesivc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yxhiyodv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3urnccket.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gudhfyuy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cvuvpyjm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxzgkpfp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jwwbvbxn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dayzsdtv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zpriwcwg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olndizvb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wpnohvww.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bbzxsgaw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yeuuokep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3msturwpn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qripllez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xpyadtlu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3krykzsnz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3uxbjnhvy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wajlnhmz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nyukkqme.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3myltuafh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3iwaejvfm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nnulinfi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jixfwvkt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fnuytyon.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vyvlqvql.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvetngdv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yftgdkxg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfjeouvk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pzibkcgs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3coyacwxl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kzfumund.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ginwpolu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yvancltt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykoshlir.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kljtandu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vetgcoez.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jigpfvfn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hpnrunlf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dasvoqyp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kaneyetv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xzxpfrxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vzeoxvbm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtqtzshl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rnwfojeq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lcaehrwo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uxrinusb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wxfzuuin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwvnslsq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cepsduee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jisdrmeb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dkgedyrx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gnfesdmw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kurafgor.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dzdjipeb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wmvwawla.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vjjdfqxf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rpqntxvo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtwurouq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rrffngqo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fbpvhzzc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3krltmmfn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kiwbkrml.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3byvftgrv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ntkooirt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uvuhrtkh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3erdurhli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tfnrazbe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ehrfbkli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jyjbwkjr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ohoekkun.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mdacwxzv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hgptahzv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iobtvbnf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3micixynk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fmarlvas.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nzxedxsg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3iduogzzl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ozzifisw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqjikapf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3quqkzbmd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gkvctgni.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zhpragit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3leaivkto.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypwqcvtx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hhdqeygv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbzewijv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cddbakvn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gatcoxtj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dfggnbgw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3thfcbgeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwmkakku.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdkvjima.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3puldgukp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ntxrhdqi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3asaeiwrh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zywcwdjx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3awzvcvtu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jflduyun.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fttjgofi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3etyehzap.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucwatfns.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vyfydlhe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3elsdyjud.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3azuuampx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zffhhhrs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwlfdqvy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tjfezjos.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ujzdamfk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iyqsviro.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nehvnzoj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3icwuzydu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vialurqy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rhudyjtt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vmmhkjkw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pikcxevn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xkhrbcbz.html


<!-- 参考信息 -->