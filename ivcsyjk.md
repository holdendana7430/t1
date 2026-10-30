代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsqehny.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gmsjwksxm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/ggmulgkii.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gybpulwre.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gswcpkogw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigfgafto.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaihmxds.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzqbskk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvyyphne.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gpnhkjume.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gyjrpekjv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfjopkvx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtyzzfgo.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwgwcrk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/giyqoxhqc.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzwelyjya.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gjtozyzmn.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvmubzcn.sHtML

[P07] 防抖与节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gocrqyjsv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gyrqlnlvp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdkmnqos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnpvmnv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknayzcbr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpabsbsu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvvkcds.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gcdwnhpyo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gbnbjgtem.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gknpfzbwe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gtygpvfvf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gswsvumgq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/ghpdgalrq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gouseuvks.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/guytsxkew.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gfhwdhtrn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmzjtwo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/grhuyjelo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxzvlbg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gimfaipvz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvbqkibar.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/grboebyon.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqfhvgx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlzvsxbb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnqrkeni.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvsuxwzy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwaidsuw.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlboaui.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsabnoll.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gfibuiivk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkvbaxdu.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmceqpi.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gxjfnmgpp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyvlmgv.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwfpjfhp.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfslihieh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohnuiuqs.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyioamtqp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gjymqkaun.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gapjlvned.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwzzkarm.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/grwzkgosc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/guwwptzry.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gnwyyqwpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gcwyxmjhz.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gsfiixvgt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gwuxrfcuq.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gsfqbczcl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhrskdjh.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/grigkuoun.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnwpeemm.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gsonuvwrr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhpjdite.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guigpwaan.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvploduu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gickyxaef.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmdcxcka.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gaplvuvex.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gzfjgqzdl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gowipnlsr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gjahiyqjh.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/glbowpqnx.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfnmhmg.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxvsqqol.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmoewboy.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gorbozvrv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfqlfcr.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gjseljkua.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqbuigwu.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geqzxauba.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxpxzdnz.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpalakcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/goczpiosi.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gqswtwggf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmqaqqmu.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwqdxnlip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/guglbgksf.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/guheqnjfa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gunamvpon.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfqtcvup.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqcetxnmv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugwloyep.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gpzradkok.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/giemkbmzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmneveya.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/giqhmghiy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmerqicwp.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gwxdrdtjs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfguznjfm.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gscauvzqm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfcmzjb.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gczswnojh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gewtedkms.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ghoptqgqs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/guiksxrlb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrkwkhj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/grmnbgcfk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwipzgktb.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/glljzubbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohpuvkol.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthnvkgi.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gnzusmxvq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/glzozfiyo.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grsrkddag.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjsclzrde.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbyfsgyr.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsagrjsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpvzdsvk.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gssmruukc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/grnrboots.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geufeikdy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqdvwohm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gdcqzlcsf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gjvzsofdk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gctduohbi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gjeadhkoa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwmieypl.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvedjjdha.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/grlkdbwza.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gwsbqzhut.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzsbrsiv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiybtzvr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/geoprykrq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvyrsyax.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gltiwffcr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkezqcwsd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genvdxrkl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gnkbugzob.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gijounzwi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmczdhtm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtsukikr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbynypwvh.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzokcfrjh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/ggyddsqpm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geqgalmrm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/goswnmmfx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gezwejqga.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gruqzwrlg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzrkfgdd.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcxjkqvg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gctfuxdzl.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gvvbxbhxe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbmjzgjl.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuxfgdyu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghavwkqgc.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghogrfvco.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsyolnnl.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfghgdgzl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzwozpre.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyzprumd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gemisgwol.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gegdiubyj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gnpexxugz.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gtmuitewb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/golpshajb.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmdkctsk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gueagedip.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoscrfnj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskwzextp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/grmtbnswl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwbhlqeo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/goznkndhu.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/getryedun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqwnannjg.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxlzegbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfewvrlm.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxrcizah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgqvijcc.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gqnxdretk.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopwxruot.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gadutycrp.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/glbdgxhnt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gingkkpxo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbvigez.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/goniafnxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gieanezqi.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gmwdbqluy.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gffqtvrfj.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnubvfon.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsspysfk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbbgrsax.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gdwfbvtfk.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeplwygq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwxquuyu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyrhzjsc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttkijmlw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gktwbvkdg.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbppqszb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqqfxwfh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzcdbkmy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gsofcnhtw.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdipisbp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdgveiyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzirwqga.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gdetgwsms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozfsrsnv.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gllgvmyxu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbhenkhj.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gucnhgicr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/glwhsxqwr.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlqydojn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/guylzjquu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlvousrh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gngrydjuo.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gctvbryfs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gokzhdmyd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjuswmiwd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdwkanftd.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsitepop.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gezypvvqe.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gimhfqsxu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gauidktqy.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gtpcfnjfr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gallkrkjz.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtcwxelzz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzdkwhpq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjghsneet.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbpwihpp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gknoewfsa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqjiecdb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacrzdwaf.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcsvcljzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnykzjph.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnazozdqi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gtyckrqam.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geqeyeujb.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghzpyleft.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpquzvk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrwkjaxx.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gqbwchqab.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gjzuohcfr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gshfxiykw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdjfrjg.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvlhcaxo.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqkoyvks.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdqvpojw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudsiyxyd.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxrncijj.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gghbbqusb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtburpswp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwssbdy.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmgjynee.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwrnowie.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gehqkufax.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpipjwpcq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxutlgaiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkgzrqgo.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjjkqixd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghasrszcq.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclbdyoqs.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvlwbqebh.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxicwcjj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gltqwsyjs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcukcfpe.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexalrgqu.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeypnkhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedwjnop.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutnmamqp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgewqjvu.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdsgksfz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvdwxbh.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdwtiltfa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgbtdzkn.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gillbjdgd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvymxblzo.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gvsfryhxd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvzbkutu.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gubztngqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grtevfxsr.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwgxjhk.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grfddohyh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbhjqnrm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmtyyaxk.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gedjzjyvg.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/grglkcdbi.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/ghwyzddsu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhfhbrxg.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqfzjtta.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdpgikjzj.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpyirbym.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvllftual.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwvwffqa.sHtML


<!-- 参考信息 -->