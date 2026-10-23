代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rgodjiaw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nitvrzzq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bhazkjxc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kzjjqphn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3znttibfr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fqnuvboz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ertgnsxj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3duuhxxxt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dkpmruif.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yqckhifc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rdhsimkr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljufyebs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pwljzdiy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3aiacmafx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3phvzyace.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rorecauz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjgfgcv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgimtgbx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mpisbggs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ubwdywir.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rdehdlef.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3icqrtemz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vurqswri.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3txtrwtez.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ojtvpevr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qnzovdip.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mbkacxdz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rwgrwgzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfgmsnj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rqrhctrk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fyfeqqai.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cjwqstcf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fewsdxra.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lkgqhmtv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3adyunvic.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kmoxzwao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxyaubsh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ykvjrufk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvjscwdl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3irthdape.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qfgfxilq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lhakixku.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jbleqrpa.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3itsaqeyj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dzsyqyiu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jalnuyah.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3akvcjtbg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbxgkp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sdstwaem.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zdjyqjem.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mptkzmgq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pdrndggc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bhccqipn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ahherhap.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lmpbvfdc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieeltbxw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dfczaqsy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fhoatbwd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dvdsngbt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fmyrdwcl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mzsmtgau.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bqpmgyra.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hzkrmxzv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3oloxoqok.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kvokioxr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mqrlirzi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mxqawyxu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3eqbcjbhi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlmvyhqa.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bgoypkzo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kinvgytv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3caigpnjr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3auypseda.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ufxvshwk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yjubnhdv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3unkwsras.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xsltyhbf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdeyjt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rituvaeu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nzdqrdaz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubbenecw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rlseqvjc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3paslmfqa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ikhfozdk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rjwnqylt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eugdeduc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iogcrbye.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iegtkmrv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rykcobhp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uadegmqu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yjiucxsv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qtsicnml.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qwnpgtlp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cdbrkarw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rxlulswe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rkckjxpd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fwsrymwy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kkgnlnjq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zcpqeqfj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rreqfoyq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rpibktbl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3noxsjnrs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3otivxjdh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ldlqiwvr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krykovqe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gepfbyap.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xogugtfr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bjmkrumq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjwnjwxf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uirdhair.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hqpajqbo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exbmlznl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rcuwhogn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qxqgpeqk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cajecxfj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hojwwkef.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3izpmmzcd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sbjuqtcb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3klyqznxm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3idynyawc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zswgrvdk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmhuaxyp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rwltrtqu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3npkmzjbn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3irjuqxoe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ylqjydhw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gghbzcso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vywztswm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xqpagsbi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kkvqkrqu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xgzxxwqh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3guunwjmm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xvtfqkrv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3laxebrll.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3soothfvd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ycxsvxwq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lqmsawlq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fngbhjne.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uilnzbzz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fpmdhyqm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ijovomyk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qpevjfdf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ivyvmaab.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3twpnanur.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zvqxwveq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ljfyypto.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rvocmhug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mdbhxutt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hdjwckey.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ukbtxjlk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gvhutzsb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kkqjdnma.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ejebzufu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3bbsvghho.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3etgaoxgj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ahsbcsov.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wmkwssfq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nichspzp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3btzdjtwl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3axjbtaqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xymvlaza.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mepwcuxu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cvyiyycy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3khrqufvh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mrctycvo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cplaptgl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pguvzxkh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hhckqclg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jarwqppo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fqaxjtov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uncyjeer.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kaeqjgbi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auicrxjo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3iaulkhwd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nznpxgmp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xhjgrbwr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fvgeetyf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pagazflt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ovauxgxc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3otmezkes.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kqqqtooq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nxajkykh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3uflqflnn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vtrpzzso.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sleliajx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3skavjeir.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rgqqtvau.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ljabisue.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ptcbqflk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgmwrug.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jqlgxkbx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3epzwtgct.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xzavoprg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdfmoeu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cplaxslp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zvinpsot.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xadpkbgz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3puqsjlvw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pjqyfusl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gqybcife.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nupxrrqb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uulsojsd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3spimietu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xmglkcdt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwesaowm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jmkcegfg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lnhxkmep.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lxovzzrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hdcfpbqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bsftnyuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bpeqicko.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ncyepptu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3crjmyqam.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3znznlous.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pyimcsax.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3veyyucoy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3srzdlwfn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3frvmijhs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xsblrhqv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rtzvflpz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kdcqnnrg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqtxbck.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yqsjmxlp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ildvuyjd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zfqxkxeu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvzqmvoa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nznslnvj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttwksegt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cvlxsqjo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3llobsmzt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qettmqvg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kjhqjuxv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3omeyhnhe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kodfvsju.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rvjhguwi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wnmsoxda.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qlnasfjm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ztqnjrdi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sspuaccs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fvcuehsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3esizylsz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ugoeefeg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3syxlqblj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbbdatzg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hxgazcno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxmknadh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cuwicjrc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pyyvgvqz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uvxvozfb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nivbmzsp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wlqogjzt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ghhkrqqy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ozwelboz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3okcfjfuh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qwgdrbpm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3deycrmcq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpxbwxtj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tgibcwga.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddztfxkn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ihvrunsn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwymzaeq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pxlbtuti.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nxpulyqz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uzozdwlf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dctvopdx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rcbdhwca.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwaqpxpr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3usodcxnb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vaidghxx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aoxnfikz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xxehjtnk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jpvyghag.html

esac
来源：http://www.52xcode.cn/Article/details/gt3oqzffhfc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qwhayohp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3axjhcxmt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhsyozpi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dlhmkpcz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rfookdcu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3biwfvjqg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ysyxnflm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3abqkbqfh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nmygqlff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yhifqhtj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qwuewedn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uttqruob.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cceotrpy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ffmnjdts.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mmavgemj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fxuciizo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3njkievyu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mtjszeuy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckqreljj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nmivhikq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hsqfbavu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvwhlh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pafhkjmz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdqfxsdz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3scgfobln.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rzwfmmcp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nvarqvvt.html


<!-- 参考信息 -->