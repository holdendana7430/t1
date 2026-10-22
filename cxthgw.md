代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tzgirhmm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fdupighl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kfeoshxd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gyydihsl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ylticqgi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sgctbjec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aaywlxbr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2auoixwpz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zxlgnkxe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vcrfgjps.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkeyhfop.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dbhvylix.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jzfllhhf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2puakxmbi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2oztluxcd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gkrboyrb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rnwnhsrw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2sllcxijj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htvsbdjn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aswjjauq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ygzrxbrw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muggaczw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nstpkklw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hgraomme.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mcaxvewh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hfgygzji.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2afwhkvxm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2czzewlgd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2auzgptxr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hzirwxhr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mcexhtyr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lrhguhgc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhpkvlc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjowhght.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pzwttjgv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnaitzsx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2okboyiui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hddvzday.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vnrxoxqe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2glywuwlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quelvwpi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nrxcxsat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anhathyq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dmxjodau.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gwrjovni.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xxqioifb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2exjyoyxb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lymqyfpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ntvgctdr.html

);
来源：http://www.52xcode.cn/Article/details/gt2lkdaaxos.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gorijdkd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zakqsucq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kaiqmrwk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aorhgoui.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2tbzxzrio.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tpwcggex.html

);
来源：http://www.52xcode.cn/Article/details/gt2wvwetlyu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hucpqphz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2baqnlfnm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lavhxjxi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2momyjumc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kndeqjln.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xczljfyc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2icmhdchk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hilefpej.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hmlzeucz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hbgzrbgx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ewluhncw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2taolmxbs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hnenierp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iykzlgav.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gxgboozi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wgypxdfg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2urifqmpo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rnnigfhg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fjyezitx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fffjnbyz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pxtvgpru.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2totzjeui.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kbalaqtf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wwdopgzr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eeyzmhzd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2otxyvyny.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qpchtwof.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rraylyyo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lgcjtvgs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2evinmzup.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lhkulpxq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2obkucaea.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oencivtu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wajnuocp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wtbylwnb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bagthrpv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qxbciitt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rtearonj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tiuamnas.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2coskqnoq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wqrvzgmj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rtwtiugq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wkmmbycu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lqokyhdc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkntdycr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nonnbcrw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hbuagbbs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gfzcaiix.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hvmyiapi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlbqvrap.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vstxsobf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2naekhhqr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bkqspvpk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lwmrxyqq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2futyktuz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfzxosfd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xiadsrdn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2reavnlxx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hvzoerdm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mokoujyc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mmraylwz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oapfdbbf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kohqonuf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2usvevcia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wamadzln.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qptlahqd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rieeffyp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2shypqzvf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ureqpheq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2seqfmgjr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lmzqpdec.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yczdwfjm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2boxqosct.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dolcoorw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2srwjasjs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lhgzrvhu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oikweclr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oxyelgvf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tcuuwfte.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rwqobyzi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2onslfvwd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hnfeixyh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ekdbxrss.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tctcggqx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gzxucaql.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2slfmmdvv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gvpqsmaw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gibxcnxs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jjxpruvt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fbpcrpyh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2upxtsolw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2igbsdjiw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bhmwjfqh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vjfqigil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bqfxtygl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2usilgchi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nwsunone.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yoypeeyc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qjhkslqb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ysfbsbql.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgntxcy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hdhwfdoo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gzvvsgfm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fntoztbd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zlskndgq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cwzlivhs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dtfwpzsf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mxpswpxo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2srgjjltl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ztzyhfmu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kafjntez.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hvxdtior.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2evluwlls.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mjymtgqe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gfvygpkp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ezdggyui.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xefaxxjq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2szmpxqqc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ahytstub.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtktzpqe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2keduxifl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mfantgvu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ujghkoyu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gmfajjwr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qikkslsd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bxsdcbuy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdddpczr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xheibztl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dnyxxzvo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eypsvpxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ymwaqknj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dyjiunuo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wtanzyfl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vnfrocan.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2icjalyfc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2prawvyuo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lkiklczd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kqoejkxx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mkcjtagz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sqjkrlks.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ypgmmgbn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jeoevzlx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ieikjuyc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aubnjwbo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uldtmnmg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2iyprohts.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fmcjwnnk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hrmpsxaa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2inqcxeua.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dtchwfaw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hndcnfxr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrsnbimo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wrvzgaku.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fjsakvfz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2smnkhlwt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tezncoxw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lnacgfzf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcirixun.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ilxpyzmm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ydhcjmho.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2asaleaie.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vtfqruws.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zpjipyki.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jezrmict.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bxholmmx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2plxvfssc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bceskcvq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wygadzte.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2meadygll.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hxqauhhu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wncffurd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mlpgzffa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oswdyqdi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zxurhudm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2quxcqyxn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tqrghrtc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2clqzmshu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fmkakpgl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ponxtytb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2efxomske.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qqqbwluj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fbwfnyma.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zhjsymvu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cevlnjfy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ljtfbbed.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzrxfnmk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2afunyhwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2anupbsgi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2katfdreo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2odtxkjum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdnnssxs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2adzusyua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajnvbwpk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2auzsgpby.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lhnqesae.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dmncuzst.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jkqfeadl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uomoalko.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfikkg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2kptksdaf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jbjxcamz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rhpjdief.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvnuhc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbilndko.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nkxqikhg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqosnakk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqhgavxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2aqximndo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fvtnqchn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2psbnqguw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cdgyzpbd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qqmiaafx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pbzkfotv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2izzfawar.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2crytzgiv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kenoxtjx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2phyfrbtz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hdnlxieb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zxcdchze.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xxlixdyk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cdsgqmir.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fgflbrqw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrcwhtmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pntmejoe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fqafjsaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2engnhbdd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjwflvbv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2livkclre.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dcnvfbrq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezsypacd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gxyjeyrt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpzygkne.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fjercrzr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnyhicyz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bwpordha.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ibfzmypq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2acysztlf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2evkuhesj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kmgydsav.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vaamvktc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bqtazjex.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sgpuyetv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ezcjojlh.html


<!-- 参考信息 -->