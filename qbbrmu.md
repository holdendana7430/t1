代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xzprahaq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2malvwtpx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pasfqexb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2qajphnab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bavastet.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kpkciphe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kvytonjj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sqevdmvp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2unxblpto.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hyelyhcs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icnxxvzs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezzrumyy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ryaxbjnu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trudmpqg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bnfwgnep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2uaxeqfzk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kxzlzrnz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lmaydmfv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2njyjzuar.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2carkxmue.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wnqfksid.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lsfemvir.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sgwycdyc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hpfbdjod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2baerrvdb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dglsnekz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ebcnkvil.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bjjdmmfe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hidodjyr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jrnqujqm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sycbzjxw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hwkkwsxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keidnlif.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mpjusmbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqjkwvsx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2shwzinel.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2oxelofca.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mlfyatni.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xxbhiryh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gnakarpf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hjnunurz.html

);
来源：http://www.52xcode.cn/Article/details/gt2mjfrsdpw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eyiamxro.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ejxewzjy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ygmewtyd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fxygqjhs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2prgixhps.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvldshz.html

);
来源：http://www.52xcode.cn/Article/details/gt2pnnymmox.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cllgoaqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wmjqixjh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynlensvn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mzkblycl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jsktodsd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kcizybbg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2yaimaeou.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2exxrimrt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2eminipgx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wbcmrvcc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2umfswnnh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hvbjzpds.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ubypdjlj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2keqlmofu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ufpvjmcj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sshrkdbe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2shizbeae.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jpiztufy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2taitlfgw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qztriheu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iqrggsrq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fuvannih.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uiybptsb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iqqoppux.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rrlxfqry.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lmgbynxp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mfcvfzbj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjzvzemj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2albxxezw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsjbysmv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2aqjdiegy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pogjkebc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nrahbqqe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fakfylmy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gxhshczc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fphzjldg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kswtnaes.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2btdjyukh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cpixusmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2liwsrzsl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vvohiwzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kffjejwq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yoqzmrmt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wxdophbc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kquwmrcy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjgkjzyn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tjgjtxni.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kddbdzas.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dcrbaooq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzzfdrks.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2lgmcijhw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaqajtel.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dkypsteg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrzzejmg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gzjfyexk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drdlkayj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2svzcmmhl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dxrqguiy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rkywutfz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nyhrozxu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kmdrjfpn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nfejslky.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tcajgojp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xwriisjv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tiulynlv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vmgceeem.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2znbubaxo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mzbxqavy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2olzuonem.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rwdmjguq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2leocxrgs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wttyskjy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hfeezzkr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xwowgcjk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgnzhzda.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oukdkmih.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqqogdyw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kplpnpew.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wqgupovc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fshrmnzg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qhaklfqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wadwvenl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ulbguwll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iyifcpoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2auiqsydn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xfnmvhfa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ahniqctc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ytkdqvhz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2arkarfkp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vnphyvsq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2iptcnmwq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ldoyztvv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ctcspobe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vwtwtwxg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bqowywwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lajiawru.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ifmamdfe.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vqqebjbd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ossnknea.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2moutdcmy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rznorley.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pnwjpifl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fghpfymi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cehcootb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2womursnn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eishfrvi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2twmkqhig.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcmhhkxt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ygpsxpku.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cqyutudj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ncybwnvk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ltzapnvu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vhfvodwh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sdndxffs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ttbkuoao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wnascpkj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tpkazrpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uzkyqkwa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2svsenvcf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mqwmghpn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2grbqbkub.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dcgoylpj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uzfztchd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyvajx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2itebcscl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nazfzjrh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qtmowbte.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2eswtvubp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zmygedco.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2frvlrxps.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mkfsksnh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kodhwaai.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mjztjkrj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ucqlemws.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2inatgzig.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ztcyppzy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2amlnjtmj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kswvbepf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mrbcvbgu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tenixifj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfzaddq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2savlpqrb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uslskhpb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2iwbpocva.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pbkmmrlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lnipyabs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zbqovocr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjkmejzv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qkrqjvuv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zhporcav.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2guvpkqdc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzrweesi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wkejbimx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2citolzny.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zucpditz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pfazptsy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gggrfpgz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vcqacslf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qiinftww.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gjrycgrv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2sniuoszd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pddaeibl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wsxwtmki.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kmbzuafa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2unticjkc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gbkjvzxa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pbtkittv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fvazbzoh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjrdmnnq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2opznpifl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbgjjuhz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dxppvlls.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxdgiyxk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gobfnrbf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hntmcany.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dzsrshaz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2foearchu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dpblhnqt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2outcfytz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fdvlmepr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2itbvagsp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sqcyagnz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gtcdxywg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ttgdohud.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bsvaktnl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mammcokx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ebmzmtor.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oroyunrr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dmwvzahj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2btkjmcrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckqinlcg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hcfnligy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxmctcow.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2biftmwyp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mdraajqx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2trulutpq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pecpxszb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kelzqnta.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xlnsahur.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ltlzvole.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rqssjoia.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fytxovev.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mrgvcnbj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bpfeqvob.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ckxdmsqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2unhzqxan.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2katmydca.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gfvmoznk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pxlrzspq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zppusamc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aqcizhkl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gmjzzyjz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mfkxwdqe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jhnqnvva.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ffuqwqbp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fgpbcdnr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rdjwsqeq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2besqttri.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zlwbcdjv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xiquftht.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dtltnsxx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2floiskey.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lxxoszaj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kayiybjh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ohgaofho.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cnwuowzo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xowkvdry.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chemhcbe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2izwhuuer.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqebxd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mowpzdiz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jxvgrrje.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2otedoluq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfxaehvl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2shtdwgzg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wfxtgoew.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wivzfmdv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rutiwxxc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vyujhlsw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxcjmbfk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vcbiuerf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2indlphie.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lharssdh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gdxhnmzt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyuutjfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bsyijocd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ygcbimja.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ebfacbla.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sivzzemw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ykttdyzl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2npoqlbcv.html


<!-- 参考信息 -->