代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ahkmteff.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mxferhkr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uplwmowi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3asgpwhce.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3preuecql.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zcathinl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtgbphaa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3osmtwbtg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzdlorg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdhigyda.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kvfjwfxx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sutffrbu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sqymzlaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcdlerhr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vamsvbkn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3urymyxqe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3frxqknip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ttdrmgsa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wdsffxmn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3djbgspiy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ickalzif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3kwjwsoqc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3btfmynyf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qzqxvpkk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hjboxzqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jkrwvbsf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iaugzrfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ymidvbzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swyodvsu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ctibmrec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkuuvdpx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3iiutnkpw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hmmfrgmd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vhlosqqx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uqspbxqp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lmtlllif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gbepppdg.html

);
来源：http://www.52xcode.cn/Article/details/gt3uiokybxu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hgrbfmtz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hwhndswi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dekydyxd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gusikrhe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wgbnavax.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uhjklaxn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mjbcgnpx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pnepstgl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qcqtzpmq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztlnscdb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3irrspfwk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qagvvfyn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wshofudf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mcnvlrru.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pcaibktb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3edfkwukt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bdpcdqmy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wnjiectb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fyfgflqb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jjjnigxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cxhlxoht.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wmtafgsu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kmqgmcyf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3oiyuctni.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sdkzplvk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3idbxmpjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rrixadbq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zvmoscvh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gkdocqwl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vvioibjb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xhsybuum.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pmmyfwgj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3opmmuuwd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3eotkvwzg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymlnincn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kpkdsuzo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xpeuwwwv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3iiusdvqz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3scryogby.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3peaemqfh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fvtzqqff.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vhpbrash.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3milfxkux.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ljouudzp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rozcufqk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3pushkpbz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rudfhvrl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbuhyquc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mfzslxot.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yipxzqmb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pbmoaqte.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dugjqlli.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwmjyxrc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qffbapxn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hxomimls.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ofewquhi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yenigbas.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xzvdlyjg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwrfraqc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gastyalg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhgxpjca.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ofcyjaoq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fohnzfry.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wdclbiuh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3srdubrbi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hzsumlug.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wshafaer.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mavdwlnf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pfhfjgrd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ypwwuflo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ppoehwds.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gkbppsvm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3foqmydxn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3erwrcrde.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cthsuuyu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txnalxek.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ymjkvxls.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ewxagpgv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gqdccrow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jabvmgii.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pvmopnbm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gzidnwxf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bnajcthz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqeivswv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jivcvrhf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dqovwvfk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fwrelusz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rfkcutit.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rkovoyey.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mdmzcuow.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dtifxjge.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qsqfanqi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtxtjtgz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tgserici.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bsjwzdpp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zropjrte.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sbjvghmd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tsbgfjyn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbzfoitz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cspauxrj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3robiljao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qkduqlbt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fvwkffkn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gmfjmpjd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dogcukyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gsehdxbx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zkomoyvn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ncymxvgo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ojlexjoh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qnscwdbt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rdwmvcit.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3niolrzva.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zactfmcm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jfncmytr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohhvdiec.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tstzglsc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oiokqcum.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hpicuwwo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pgoclkzc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3totzvgpn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dqngbsyq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cgdkgpnr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fnbsfiix.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3reeorfdx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ncmneygc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3umurttcu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fscmoebc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3iqeehtip.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ercitjnz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vkitujts.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tvghqqio.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xctgfqzu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pxevksty.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxpzcfl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vfivsrkd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3csuftftt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfmhwc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qrmmovwf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nyvajxau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ohoubclg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cjgxvnhq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3utethxhg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gowbybzr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ybjacjcv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ocgpsbyy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3khwmebuu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tpwlibbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ydcpnxtl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mtkfguzu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndvgvizx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xbernowd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jfpdcfhx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bfgqbvhz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ysabqgiy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnshgguy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ltpmrwxw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cmljquhu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kaxcxpzc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iafsqdat.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xrjahcnf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jespgahi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tkueuhcp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ckubwqcg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nbncpdvg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfeetjjv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fzrcoinj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tdxqhxse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bdepciqy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lpueajqk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wjzchsbn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gfmlztcs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pgiyqdvj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pbtimmpr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ozzkenlb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gbfuigrh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmetkuvy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3drzqtxfr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npvxqnni.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kifuydhz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfsttebn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bklmhntc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxowbuiy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bnmbawnk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhycmaum.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ivjvngtb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbosaog.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zzzuyphl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vameducx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cptliwzc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qsxvfagu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qcznxnik.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xpkxqedp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnqtuoou.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ueorbaav.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3obbpzxqz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3akyriceb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iunzaazk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itjnxbqa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iwhuecia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcbbbqnr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3euojxnay.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iggmulzh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hibqhwzv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rfafbkdr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3znhlpheq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wsqralor.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yuogtlkd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdxdjzvk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ccefcsyt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yydxzsxq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxtxdciz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3eyrbdwmj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lmwblosz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qibwoxqf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phmpvigh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ejpgxzoz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3csrmfsmw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pdbfixes.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jrejrlfc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fxoudbpi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lcnaergq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kjycshak.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wlxdckks.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tssqtquu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wbhobozj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mpksccmq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3elqheene.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hiimnnyb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tjfygmeq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qvdfyxlt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vucxhayp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3guphsfch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tzelzwwm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xyviqiiz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kncmfyyn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rbnyftyx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zuzxdyuq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bgwozclx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbhhlqvm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yoemxrjx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nspelnzk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxxfvgru.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qotzhaqo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xscdtfsu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3usdlzdlh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3arvifwho.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctkcaewg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sqonadnv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3njydeyya.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yumtgjpx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lsloeneu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3retwqdqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpiefnta.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wacuehtz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nalmlbje.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jolctddl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wngtemgl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uqermmvz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qytsfbas.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3itatyimf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mwiinvkf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahrxfzvx.html


<!-- 参考信息 -->