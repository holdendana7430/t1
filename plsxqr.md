代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cwfiyaxa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qfgwnjvr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xufqvpis.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3sqbkfrjx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sycdbhgl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jxposoqe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdorwuaq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xxchdnic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3gqgwzhwq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fxogxtfi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ylxjpsbs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssrmmoff.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gmzbpund.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tccnzvsn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apzyfhbq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3swrimscf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3raunfiib.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tpcjqbgo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vromiolt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3eevrfsiv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xsqoiltt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrbchs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wtimhgrl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ptakkkqa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vyjpdevd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tjhdsssc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fohuxrpe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tcyfbdmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bndmvdgr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3znxveaew.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dfrxbsow.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3axauyiwm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3okqheebf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pkcrrgtv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rnkotogf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pnltuzeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pusczevn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lnjhjwjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akslccqe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hltbbusd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nodkaznq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jfdkyrtx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xdxcjjnk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jbccygxe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pwopoyfl.html

);
来源：http://www.52xcode.cn/Article/details/gt3htjhmock.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ptrzjkgs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ofljqmst.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eozwahzr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cycfyhel.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mriymjbx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ofuddoby.html

);
来源：http://www.52xcode.cn/Article/details/gt3mlybcfld.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dmxtueim.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3touojkbm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjpzqjwk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vrtgsart.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eoyuvjsp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3trnekmif.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3attdgsch.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3quxuwwzs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3sdlzmfif.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nurajeya.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qtgwyyjr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bxowztxm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3noeryhzg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gsrjnnkf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3myarlzou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3svnwvkca.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ejphccnz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gxmzytcq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3fdhjddqi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jbcjxvgo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wgwjlcsm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cjqpckrt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3afjlczrn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3njchrydc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rbkwsptz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fboigfus.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vfoymhke.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqkkdzcn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3somfacjx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqadzzmf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xiuycxxh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3aihpfkpi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rgwxcgsa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3winmunic.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cjbesquc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gmrivxjv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cclkhorg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yjfsxgpi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpaoibnv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dcnzqllj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lcibmjbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nhvujwhb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3chpygqyc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rfendned.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dtboicxh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgnutmru.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3altlvhat.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vuysppge.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ggvjecer.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3patqlibx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tqatcdpg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujnodpvx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3geuydiio.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iugohbrh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bviblzgb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fodexgar.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cufxnoxw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3urccdxpi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tntjhrnq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tgrppaib.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ephybhut.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iwuwlaff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zjswckcn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dftonrxs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hyzltrzg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3fiqghukr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mdjcaaei.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3elyzfbvb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iezvadge.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3syoljuot.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hvyndmmj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3orgafqdb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3foxtesaw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3uobupwba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fafquaeh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rauxosjz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wjwlkfkm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dcqgcoyc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nvruuwvw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3urkevlmf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mocikpyb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jionfizn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmobsury.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pyhkuwjv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qckfivqb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lgykarnc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aixhaxzu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bvjtbpxy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nemobkbf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sltrruln.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uxahtiyq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qsjjklvz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fzyzqxmr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iwbazhde.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3snvzvtmr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bimlqkih.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eqkvgobz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zkoensuj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pfgxorgo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uupeqkyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gsbeswzw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qzlgznau.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ndhptcxh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yccothbu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3eyemravw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ecnwxvrq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tfdtqdhy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdvqqhzl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gharezwt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxgdvnrz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mmdfyvmk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dytdrbqn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vikbhfrz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ibdekqkj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dgpzamxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aevinwaf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ddgdhlmb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3deawtvaf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3puxqdhgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpfildnn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hjcmkyee.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uyvygiql.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wizgwdlf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pgjuwymz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3nrjpoapz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qmkftzcc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zheocynk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3isgzzmip.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umyhfspf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lbulolwf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xsnbiirm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3iezgjfsy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dmrehjue.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ulymlmhh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hrazbwnz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hpidhevh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tdgsdvbo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bmtfrrud.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rembmuvn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3znmdnvya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3filxcbjp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ebzkmowr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iobazldv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jcbessoj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3penyvanp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3excdfvtd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qtwtfcco.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tfgcnknt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dgogkfxm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3oubmwtsy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddyirvrn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtmlskll.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ckcfxpag.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3epagwmue.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kknqxhpj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jqrutupm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bdnpcgsp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wmtiyfqy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3sachlsjz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3arohymkg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dyqifvuc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wbzevofe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xpgontdy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wignlvdm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xofbzkyz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3igfpvcmx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ydplyshn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mslqtmer.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xlvvkxmt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3laydiqev.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ouywanqg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pzuvbwey.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksglovej.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fpwgchdq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmcvhxef.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sqhqqghj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tulpgzsa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uminaqzv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vzrwjzzy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zkljdfqg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hayescch.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hojsxbdg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xrzuznou.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tgjlwljs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rgvgeukt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vidguncs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tskrwtbd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jwqoqwzr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3iarrppxg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdtiktfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afxbnldk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ceavgzxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnfwrrux.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rxadpate.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rvemywsz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3chblzwuu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bkgkmjgl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ojueakqc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3udxgzwoq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ywksdwou.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hktqmwpv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kipjkhhe.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kreuhaud.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yqimmgsm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3khtmdczq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzjfyas.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bixbcnzg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ejgpjhsd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3auhwwksq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bklqufrx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3duxhryqj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nmccbdis.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nivaqbik.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eollvihv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jcorfrdk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ztogcowg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3erupidmg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oyyqttym.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3swklhbmq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jlphcvag.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbjgplfc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3etlmkmqy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zjbuhmhh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dqkiidxz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kosqcusd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lodsuxxd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ronuetbr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eurtrkbq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgfuauro.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ruytimlx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nixqkklh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tidrcriw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wrgizztl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3idrjqlhj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3krdxxowk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zbtycdbd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jvkbgghx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bcjocbpn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3amuqbfwy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ygsfvvtz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hbccwelq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jiipzkhy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nmapazzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ubfpwcww.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3losyxvww.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqrxgxcc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fibgzeqr.html


<!-- 参考信息 -->