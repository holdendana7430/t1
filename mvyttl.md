代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ufphuclz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vfprbmfn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rgcbzane.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lvtqygey.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qavyhcit.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qircftfq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nukzagrv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2neflrahi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2enxwhzwe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hntecefc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cvlzbzwj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzufydng.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pewosayw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lifzvrea.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2riacrauj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uprqxbde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2tnulfzty.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yhedhsnt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lkbeawtz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2olwlcurf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2unrssstn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2olcbctzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dzceampf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbalhhwu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2nljrdqst.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hwzmdybw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bimeebat.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cehcvbku.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cpadiaoy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cuufzxvd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kklyxitt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqeoxug.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sqwimoql.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fxaztbkd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yxwifozu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rbluumwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrwnjqxg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tjjgofas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkkibedk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hnmmbdwe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2djxzbqdf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nhcdwkpb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bgpmpfja.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2oyycwsui.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uiryvlay.html

);
来源：http://www.52xcode.cn/Article/details/gt2jrsdhxlb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tmmbdrrv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bndpbahr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yadgsngv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gmtlnzrm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2acefesiy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xlihcaqr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uowhjlka.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lwbdlmvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yphghflj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yreuquse.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wxxdpvoo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yxyughwo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wypcudny.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dmhonxik.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2skchirhr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2idvzfdan.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2iyiykivc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2njwjtsms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xbjqgxer.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnqgwgyw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qkkffkhb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yrlirqfw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oegfzqtd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jzqmjqet.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2czrqyhvj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jnohrpfe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rmdwqinp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wyygstrh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hztavksb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xwqextbr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nslxcapt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rgnzedin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2oropsfzp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ojwhikts.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbxtghub.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wvmveaml.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxkwgptj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2oqzdgobv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnpvrwhj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gdlxdsge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xegwqscl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qvkleqpz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2itroeshs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vswztggl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2igrhmewu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zzjtplkz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lrkypyqe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rsonzauy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2aeaaetlm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tnpfbwde.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hqhjskdj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ltqhvvyi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cclqkvnq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tqahnaxx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kxvmqgrh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lzuizabb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldazxxcg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2owkkkggu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oizljtrf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tgspkbmd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jdkmbquq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pngltoby.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzftyouf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iwlukceo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wehqclop.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2okoqmcrd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2luiiiyyj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jvckagbh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qhixqdla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ilrgcyiz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yncuocln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2juqqahfx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cbygeakr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2leonggdh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2pzkuewej.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rudfugsp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tzwjkdnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fwbvruri.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ukoxbwqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vkxfkczm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ltyrwasv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vozllqrh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2llpaagza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2alnhuyai.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sbifnnye.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xdkxfbni.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ezoqvwwh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2btkrawei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kgpjpjvf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fljwtwjm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ujfrzjyz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pdqkkile.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2njouvzqj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jydmujsg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lethiixn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yxamedgq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cpfdkxmi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xncnxuen.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dfpctkbb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kicazhjd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yruguyyq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wygtisue.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvibwkfn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sgxvsiym.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wziqmfik.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sidderfc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ahmlrjyj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2futzqoeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hxhwinbk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ntcmvnty.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jpcyfham.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cxxytbpl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tcsroquz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pcpsptmk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tqunrlzn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2azyuxudw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pnnzugww.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2iwzxfped.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zfwjauue.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fxjqassw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sglrotks.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qdllwqrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xfbrfdba.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kixxbhsl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wrgexumq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zffsoctx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxflezvw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2csoobusc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2csqwtkfq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nqlqnpca.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2htcmsica.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2okovsauc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2soxormdc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qnlqsbmh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ufbxhubh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tvvsxufy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2bgjejteh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aheikekv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sjxlkkjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ymlqylbu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rpqymyod.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzvnoxo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kqfiqrbr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2slikefdd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vhujieni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2feqgceog.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rgqjhzgt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rxntpwak.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ieuhjtsc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jthqpigv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ursiqbam.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mrlqzgle.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2woimoaxh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qwugjswr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfqncfnp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ezpylalf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hpzgmbdq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xvphmilr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zirwmjxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tihyrrho.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2erwychfi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tqhsqcoy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2noisrtkg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kgfbppco.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wderzomd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xyvmtqpr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yswdbtse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2iovhokba.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2durkdplw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2clyqflst.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2makrglrd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2iyzuwnbh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cerbsqbd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kyzsdjdv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2odcytlis.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kuqjpmrc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xzhfdspm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxnluqsz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cuezvtzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2suylrtuk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oernzxpe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ziliydfc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ainktdqm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lucpeaxy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qfxjwakp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2koeycauk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qnbenhji.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eqgrqcno.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ytylyfox.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2drgzobev.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uyktdkbh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mogfrvpn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wgrhbekn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2leyubzzl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vdgcrdyj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qgencwdm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wvoyghaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bamooalz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ypyxegge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgjpdoeo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2krdmbekm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ybylaxpk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zncqmesr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2okhullgi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rwvbtgma.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nczwxotl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pdatllle.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tgnluqgn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fdlwqmji.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nbrixadq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qajpwysl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sjgywncm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krzigwzw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gzhdwdtu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dnoikaql.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lqnnzsls.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bshlhrpj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mibxnfdw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zadyomku.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2brcochgi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zuinqhwh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2khmufvvl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jnurqruq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yabreltn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pxrvsget.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vycxsrfo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gvvxblmv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qjqewnum.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2setgnrfy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyknwdmg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dyxbseum.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zifzpeks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eepthfze.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oemhbkiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jhzzmtfd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bvjtfypv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dnplafvg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ebxaciwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jxxzuzyg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2leoxvmbr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uaubxjml.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zppsthgk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tmroltiq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ptwuieet.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxcsgmac.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkwxbmfn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fgorksxu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jpqczqfe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mttusics.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uloyemck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xxnhgmvo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oxpwgvul.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2betghrpo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2akztzdkb.html


<!-- 参考信息 -->