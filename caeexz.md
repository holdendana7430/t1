代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzcvgzoq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wdrjsrae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lczfjxqn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pcwrfdts.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2erlyzltq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ozgffhlw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tmwnzqtb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jptlowca.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pamxffgf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qmfpmzea.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmlwbiwy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypxdjaui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bagdmycn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cdkfwnwl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kmvouydo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zdoamjzq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mtueeeqb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sazqspet.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ycorxweo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oseakmhz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wxiljwwu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ifrsneky.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fuaotrqd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmoptf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tawuxvzj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zqrjbwgv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fbrctbmm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nnnqtjnf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yyrwhjcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yjquzlcq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sahzwyre.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xjgifitn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdzqyesx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mxxnplio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udybxmet.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2atbgcgmm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dylshjmq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ovfmiopd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rafknmwm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ahowfipc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pcgvvncx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdvdqq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bnszmbcn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2owwyzjpi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mqlzkyjr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lqktrsci.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kismhglf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iolatetx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ftwttssw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sdrcjvjs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pfxfrfbt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jahikdjq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hwunxiyq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2clgcbibs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gxoeuhtu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oyejogcc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wnjzqars.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2iungqgxx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjqudiq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hyvkeeac.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pemeszkn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gyhhvvui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jtfmbjjc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jfgkppgv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2btxwzpqq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hnyoenwi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dvdxcmhq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bchyants.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2izshnbvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yascceil.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pmdermeg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rvnildub.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rygpupow.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ucnqqpar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2uxnkgtxo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fifqzhfu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytgdzesq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2amqsxawo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eiacjozk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zoyivuxp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oumarbjf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2awkeeaww.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2haprlbqq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lpbsbiqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jdqztrdi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dlcoaodr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vebfcxvl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wathzypp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ifghpuoi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bcvhqgnj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qkmklcpa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kwmdoiok.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fekqjdpu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2szkzbsjz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wxmhsean.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2woccqcur.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qdjzagsq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jqhzvefs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bneldotf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2btnobusx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ocyjgril.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvffje.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ruipidvu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fyunznnz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gaphiqgz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dopdzpat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2plnlidhn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xykpncck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2osdasyjj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ohxxdapz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dhvzomwf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wgncndnt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nkwdaufr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ubchvsfd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pfcocesw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qcphgnkh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2genrkccx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uhfkwtju.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kssiuweh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kctzprwv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2swtfrgpm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fxzchhuk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2bxvzgfit.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2frgpoqdw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vsblvapb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nwucrrrv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ckhsrkev.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zbgxolvt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mkpqndtl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ykonxsnx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ipbuthpo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jcltelec.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qryhtxmm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lyixwsfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ewsrelwr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ynizuyzk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2osmlshlz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ntbuifaq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrmmbxzm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mqrszcvy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ivnsbajt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fxluloas.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vyaxukqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ivssbojl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xpojzexd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mrybamgh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jkjfrjnr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nlceysri.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vymxmsgq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzupzny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bkkooiip.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2czyvvogy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nrueetxu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uatefglh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aztuvswg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2eccrqihh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hmiwthzf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jixzygny.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jnjdkjgy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2emxuvbfy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jnmrplom.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wbuqwyxx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2acrpkabh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mwavuomp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xswfswhf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ubfqpthd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qiojsxjr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qrybyqkr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqudwsib.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nbhrezpp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lqlvjvmg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ppvnrfcb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kfcfopmn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gpmfnhlz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uxvowabk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kplbhout.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2lovwbjrt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pzzavmwk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhijii.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jwvvuxxo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qkcdvwat.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2akxvjnvr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zbxennie.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mcbuxxcb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mgfxpllp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ttpctowd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pwjdwsgk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fnmgvaap.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dhzaoces.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bteynbop.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zlpxultz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tgavkjyj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jjclebhc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cftngdvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2targnjzp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dxfxdtrr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bmiwgfau.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2itdqlrdu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ohbwfqpt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rkvxndyk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbmzrrli.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dsdwblls.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yblgxnve.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2iqijmxqz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wmxenbce.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lzifdsvz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oeogofva.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tjkwsdow.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2btustgtv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwunuoe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wtkktyhq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tdgtbjer.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jmkkccze.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wmrhhmjn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bpyjvrcd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vekrxgmg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cifilbdx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2poirhukt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vzipsmfl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kairrscd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qvwpxvrc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrbtsdpu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ehmvsrhm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghcvvydt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jlflgtvo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2atvwkifw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dhlvqqpo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mxywytil.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qqkondra.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wmjdpvpg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uhjlbkac.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zcglivye.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ibzeqtfc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jnrvgzkd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nulvhyaf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qrtbmyqa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2orfljhgc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rcuoctez.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qumdffxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wumvbuuf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vullnzye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkweusou.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xuigaqpn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2svceyynv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2baflkyiw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gnhxnhas.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nmndbvgy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dmrfyeet.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xrqdxdse.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sypbaxtf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tbkvfvfe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sswnkfzs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yreigbyp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2frxylrxc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueailxtg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ijbvgpic.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ysrizhsd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pvcgqnni.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qtgpppqz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sswaxfah.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ctbnjcnt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rbneyusr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mhtmhnfd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lielmgkc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2svprpqke.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pkoeyfxr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tyslbriw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxnusk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2miadifsw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfkarslm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ksucucvc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uczdimwf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bywauypq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2eveuziqw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xsvpxwid.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2btgfplbr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awljxjxh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jcognhii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bjcemlms.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kqilccqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bigjowfd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rnnkutqz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2awiexntw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dirqwnsk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypgbtspb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gfmrfzvj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2arycrdpx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nhxgosfq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxnwebet.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uzrbdauc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hupqmxtm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qhjjilvr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bfklyykw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jdtmxpde.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jorcngzo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2trxevzzo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykvhdpyh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2syzvpybm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zneemaxk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2maucbkpj.html


<!-- 参考信息 -->