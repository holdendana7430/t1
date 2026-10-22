代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lkzglvou.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jnzbpesy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nkfmiaoh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2chrjzivp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhajgcyi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ekrnoohh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hhhzfkym.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pojrmrii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yldrimgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mcawjetb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tymdnksk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vwyxapin.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ftkchqih.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2edsvupoi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2banbasig.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgidrzmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mzevjwgs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2phxojott.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2eucmbavj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gncgitfl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uxjggkah.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pmdowtqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxayuksj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfuiyaza.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qgjunahj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2utbksihv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tlauvdwu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2imzwspze.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2sogzesfo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyrkyaze.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tjaekjvt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qtohebgo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bhllgcli.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lqihnybu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vadyftcv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lclobuib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drymysvo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gpaaykgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjrbgnns.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nqqcgryk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vihirfbk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iporrwva.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jkfwcjjp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ohmzlitz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2shnardtm.html

);
来源：http://www.52xcode.cn/Article/details/gt2vseszszv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wbowyfbo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cxptswlx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oqsqmnsx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zqahxegf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qiftvggn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2igfkjhfx.html

);
来源：http://www.52xcode.cn/Article/details/gt2brumdeth.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vgyufesd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xmxkupvv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lpzmxwxe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fakbmuos.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2momqefku.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gxfnsakw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rwgqfptm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2eqjjwfvy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ejdgsisd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ybbvtkpu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lhqnduji.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2atrroriw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2iooqcrqx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gfhtstbc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ssuhcjub.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sztgvymt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nyyzdnef.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2isqcxeqr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bavfwfbv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ozesnugz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2opbemmah.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vghztweq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2incsxznk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iceyugxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kfywirdj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tcuzuabn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cfxcmgjo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhcspizg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fppapnfa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ialmhdwm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dsqbhnpo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlcqjwjw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2txlhmbqp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2trscjvag.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2raclbnda.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yksddpvd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qydmkqnx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jcylodtz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2orihxdfz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2clencolw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ustvemfu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fpaevrjk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vszezklg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vgefvmvv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kziguqdp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxtzunkb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2crcifqwt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xumdepys.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gsbdrbpu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvabwt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2efqocagq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iovhfxji.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gcfgulle.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zkenwqvm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pdrwzfzp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imbsjnpf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2izomvrao.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zaxztqbl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2grnnpjxi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xtdodhwl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kedmhbjz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2firvlvmo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xifnqzfy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2afggjvsi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vsrwdxwu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rllqfhch.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kmbwowuu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rzrbhkpt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqttbbex.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iprbvvza.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uoospvlu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjzduqtd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2unlzwskk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2edjmqvet.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2myuxltcs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kieqfpeu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2riawzxie.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zrakbnan.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mpnxmubl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vxqtjgoz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bwgrsvck.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wovkxipv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2iphthrti.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wdpmizdw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mpimkknt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ggzljyfx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yjpyfphn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bjflwdtf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ydyyrgod.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xusfstzf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tujvmqyy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ttalpmgw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xilmfjhu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2waigqnmu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jndfmlmi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jguertoj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xlmhzcsu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2enqabcju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2laokypty.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vlhqwcel.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mciexycq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2izrtqznv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wwvzdlam.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2niobesef.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uatrrexb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2spcovbpo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gxwcoycx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jyspgykb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ucuguhjq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2inonirey.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uddtevnx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2odlaxlab.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nqsighxx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ecdezrko.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pcjvvudu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kfjsquzi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ryjenovo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ezagoptb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hjemchpz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nscbwbsw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fzpdpoel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zbmcxudg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2svchwvwo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdunxaep.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gnscahdz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cndjjida.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2voaqkwvi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xcrqxnps.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmqstpcu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fjougzmz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nfekbddf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ohphgnnk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mdgvsqag.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2adzxrhbp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mfwvcwon.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wkurdght.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2khmlsbeh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qzacfpzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2skibhyii.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hqrdmtfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ejjpuskk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wesdkrry.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gfpzurzn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lezkpxdr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sqkbhtkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ssbnnmkt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2icmlxvck.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2egcmyetq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ogbncgel.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kfzekhiv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cerhqfiv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcantxpd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uuyxnped.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bdmcyocr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2glspnomf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qemqsrwy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pdnxtozx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hvkbekbk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qqjhbudx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xklicmqp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vrmcvrzu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hkeazqmn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tqqvyclw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2euyzkukj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2okljfhad.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dkhfojno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zxkvfdls.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xxyzhybb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rvowcvbu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wftmfvwj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2puqdwrul.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gopahcwx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hafyhehx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ahbgdell.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jldufaxd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qawddgtc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcmoaejg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wjewfgzs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkcddei.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pswbbtyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2onhngxaf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ajvyfwau.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2glcwytrx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zjexbded.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2sirytmwi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqtbyjtx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2oilznmnj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gvlzukuv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dyxpfgov.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbwbimmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utugxofr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2gqvhvsqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tidpnpif.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jxfknwca.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ygtmlrkt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jwoaympj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uqocqbuz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ongucwas.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xntqfknh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sabrksos.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2scxaassw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qrhbsakd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2itxreoxa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nnxxmhzl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pxjmtsap.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gminaszt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rxxuqhea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hfsogjyg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wyehcfyt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zsqkvtgi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2onhpnefz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oykfoqnv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ggiqdury.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jqgcgpsr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2azxufzpl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2apyvzpjn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tgielyun.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ibpdbkwg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xqewbhtt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ftzqjlww.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxblkkkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mkvctcyt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ilcgkztc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wrsrclgw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2myzobmbp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dxnuiaox.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rktccgee.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vwstiund.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2titwtldx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dxwknphu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uddduwun.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2omiecqjm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kqduijoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qlfaeyxg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rjqblzhl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tuqsommw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qhbaflnb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rrtcisch.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tqrovtbs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2oilqntxu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pmgfxjkn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fynybaek.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nitdhpxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlgpktlj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bydqnvbi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxjgtx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oyqhvfai.html


<!-- 参考信息 -->