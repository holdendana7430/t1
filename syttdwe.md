代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gxkswjrnp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gawiuomcq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gdrgxpoov.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gnlrtxtvz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gmrjpaqxt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gezisnntp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gowneitbs.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gmhopkhou.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gbcnciwzp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gfhbqmhuc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzxlcdosg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gwnnjykvv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gokgefmuc.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdpaqktcl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gibltgntu.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gduevvwnd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/ghvfbcbfu.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjtlkueky.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gdbrlfcqh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/ggccgxvgc.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gikomexgu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzdqnguvn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggbouwzuf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gxhupevsh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gizgmhskg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gyleisbzb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gnqicjgxt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/goknorvyu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gfjnchkgi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ghiuiwaze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gustjdgcd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gymgxzoqa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gplzwvdyg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gcoxfrmwa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/guujpkftx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gxqhvcwid.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbqjyjlui.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gittjtegb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsjiqvjwo.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gjklbqkvi.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjikdpxyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gogqmrxfm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvopjlpxe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gyslyoutz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gogwwtwwh.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gkizatmfi.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gtpftquej.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gjimjtrbw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gsawtiwnf.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gpbrwvoxv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/grlqzdmuw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gcyqvjnxn.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gmryaqsfh.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gakpfuhhl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gmlqlgexz.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gnfkjopxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gdosnevmo.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/geaddzbnf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gtdwxodey.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gzgjxzryg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/guwjgiuze.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/geebjtlef.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gfsdjrara.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gxvzkvyll.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gnpozkbjy.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gmxkyfako.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/geenjeumy.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gesrpubjr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gjwfkmifp.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gapprkywx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gancabqaa.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gmgmhosju.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gwnibmoes.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/grxrsvmtb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gqezpbjze.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gxglhqjdt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gmucgpnoe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gwbahnuia.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/guzelixqs.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdrecpw.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjhofgxdp.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gyhzgqddu.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdkceocow.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/ggugjnbas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxmjywnuc.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gphcpxajt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmxwuiueo.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gwmzfvpzq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gbmgjqrpa.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gxdlgujrp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gwzwtnetv.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/grcfifnsp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gpxfndzcy.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gjabfndzo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gxnnsbnbc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/guyxnalsr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gwvafqytx.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gqbqutfnl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxsvoseed.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gjsaqjchl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/grohvcqei.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gvmgxoayf.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyrnlxeln.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gfclvlrtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtqaisyni.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gfxbuuchv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gsqpmdiag.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gkseehzpg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjemokagp.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gdajeddsl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqcvenfva.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gzfmzljjb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/grebbzsvl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfhwbuzro.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzfrghscp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gnmelitnc.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gcfzmygfl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gfsookvwu.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gvizhhuni.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gbqwtyrfx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gmrfbrvou.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/grczdcqhv.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gpclzwkzu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gectgmgpi.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/guevgnvlm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gnbenvebs.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gufgpmwpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gwhalcgsl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gwpgxdkpi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/goewbeyjy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/giuxzowew.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gpcatmnma.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gmpixdsdh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/ghyuuhscq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gpzigdamf.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gmnjcitnh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gqynhkhhp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gnxedenfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gnsxvqdvz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghlheuqyz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gkwytnnln.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gdkxcgcqy.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gmxfjuxpk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gvsvjufzr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/ghcrgnyln.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gwtuxjvop.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ggqhxinrg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gvsgvabdl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gpemxaeho.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gzvyvipmi.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gcnpgthjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gwtojrhou.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gdcxkuzog.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gdwpiazfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gvbhpvvgu.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gmemgbdxj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ggpqowfni.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gybzwuvqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gxwxlvbpn.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gpcokawuh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gxtgratqp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gyletoukm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ggsreblmk.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/geowjsbnn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/grrrnjbmy.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gcuxcygdr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvebmeuj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gnhihtcyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfiysqzgx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gjhjhomja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gjzgqdzws.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gxdwmxcmq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjlubbiho.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gpifluumc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxnhwjtox.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gzvyhaimi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gererlbxi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gwohkbfkn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/glbiooihb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzuwiprwq.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gqjbvehfy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gndmadvsy.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gunjqvbuu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gheoxufhd.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gfcovmjdy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gdbddsdht.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gxwcwwjwd.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gqgfjtuem.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gcxivseif.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gtbbybhku.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gwarzdmns.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gkmreujgh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gepvvblye.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gzpjbnspb.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gthduaeer.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gmbvczcej.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/ghixputqg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gfcewdpdv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gfarhxgzs.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gcwnvefhs.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gxiwfoqke.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/grttkrjxn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gzxmnqevc.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gefkbdmxt.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnecwkxlx.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gttpyyvqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gbpqsflel.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gzmpyjxbq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gstshismo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gafqffjsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gnsukzugp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/grkobcruw.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gxisodhlv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gnpgttvqx.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gomrdbije.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gnursauqv.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gfupoowyy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gwerjeahb.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkfrbkzrn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gmuwbxxep.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gghyiswsf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwpuzuhan.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gedyerbon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnplzznex.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvlwugu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/geufterrp.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gnciihwyf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/galcwxhkn.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gszocmrrt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glqttwfyl.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gjiayclah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gfulkptis.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gibdapkqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gzphlcbbt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/ghtdrprbk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gyrfzlbik.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gewicfyju.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/ghjzkhnsc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbfjyelbr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/ghgecxjgf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gvjyjeots.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gobyasass.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gqniemzjg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gatwhekam.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gbzqpfpqu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnafmniit.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gpchzpnpm.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gbpbaubpk.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gckpbqokg.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gugqicxvz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkpxnix.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gkrrcawpa.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/grgsbylec.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gakcwjddw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gvchjgrht.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gpqvzslnq.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gmucrqyqh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/ghvrreaxu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/glijghbie.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gggkdexzb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gvrbsjpmd.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/ghxmkybat.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gopdibgnt.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gvyhlfccz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gacggoqbc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gnzuyuzqz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gduvilwof.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gzzwieovi.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gmsgvemrt.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gfibbwijt.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/grorokddj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/glmrjircy.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gckcjiloi.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gfosmjsfy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/ghwaybaei.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/glzkdripv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gwgyglcfd.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gkezrjymg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gzomzioza.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gyqnntvlu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gwwmqkdau.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/glzwxbwan.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gjrjvhcoc.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gseljgrym.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfjzhnvht.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gvqmsrvkh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gydopydxu.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gbplhjiiq.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gbgrkexly.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/glfmtmsdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/ghazvnmgj.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glbndluay.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gtztowvws.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/grfyrzhop.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/guuwnryxm.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grsmcgpbv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gazrmoubw.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwtxiyyad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gwittwnjv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gxyndppnm.sHtML


<!-- 参考信息 -->