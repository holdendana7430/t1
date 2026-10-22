代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cdigaedr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmqbhha.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tisyjdwl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iexafyez.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bumynxdu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2aeofcmxe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aalsaatz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xezslgjq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vwyndeev.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mpjseufx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xlpvltdw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gpwtrrjy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rzcebobl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rgeufqee.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tdgclauf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kosbbtrt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgnmdi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lachcqtb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rofvnynw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vvuwlqmg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rdkxxvzp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avlfkyzf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rtiglzfd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jxfjgkaa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ftwtlgwa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2soneoaiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cbgthmlr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfiwzaqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2epbonrak.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vmnlrukk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vudxcrtb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2iqrtgrul.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2beuajrwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2atuqigjn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hugkrxch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kskbsydy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dltejkjv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gtxkkwsv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rhqepajn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hlkpanpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uenabxby.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xqtdppgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffhjplkl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dwxfqkaw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qpchoiie.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mkdyppbb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2riloqesv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2taqavktf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qvcoavlp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yqchyeua.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pufgmsgi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hjfotrqs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gklzfnwv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mdxalava.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2cwwazktc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yzdxosna.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dnabdryp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fynhdtoi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hksbjkzx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eaqexwrn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zjjbbwhq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2aodypoyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hfjnwzbr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ptexafak.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mtezsplr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hjgnnvql.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2teypfsph.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2epixvtyd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkrdyi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tprzxnxj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2otugcoii.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zplrfuem.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ijhuajvs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zleyuyjn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jdlybzej.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tdizmfsv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yewfldxs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ptzgltcu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rtrfxgln.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xhxwdnrz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2atneivdl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pwtcsmwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nuvwhtzw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2trppkdkj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juvjowww.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bdldnirh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zakgxwgv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zygfgzuo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lytpupeu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tttwsrhy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hcinaeey.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2elrjvqsj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2aqzictmb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zwjszsdj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2llyiicer.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rivjyshl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nnvfnofg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2waqqnewk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2koolmaum.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tiziehmz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ojgpybnh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lcwkjpab.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpndeapy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cnbmnppy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yfsnzpdq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kbfpulkh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mztklbwz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xofccmri.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ssdyrytn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xnjlpqso.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2flldoeds.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2chdyujes.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvsocons.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wcmmdkly.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uihhymov.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zjawphel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dqicwgfg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2udwkdwpf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iunndcfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2awkyzsky.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jduaczfz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ajzpxqgs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cccwzimc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2thckllfh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ttlsvxyu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zcimvthi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wkkiqbny.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lrbzjwex.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dpduyoiz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2siixuuzp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bpfqhxmc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2skbydxzq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xmbrruem.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hwiqqorp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uyygewwm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sewhgrte.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ohejflqb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tbxucxjn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pzuwdldm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2shmnyyfi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xtmartqk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ohisxyng.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xkkvhqsa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ludqyauv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qdnppshh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2tgnecjos.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sstyuvzo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2slirvfwc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sxstzetk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fnfymntj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ctuttpfj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ypfhhenn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2crathzkv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lqcutufi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sudanruo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bnsjvnvv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2avjrwabu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmajwqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ytwjygtm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vnlceybc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tveddtzv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jwurzuci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dbolsycw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2obdiokmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tqbmqmri.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kwodqabv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zkptbgjc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oaknqlut.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qnhiibpf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lfelbssf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cthpmgdy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ioycrnhk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hbfbnzel.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wbcegzbj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xziewpay.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lakbmsrp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpwpcqgr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eizzaedq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njecsvmg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pffywjwj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrpjmc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fmdwuedt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwirxh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lfufrmuj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2puhwngff.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aszflunh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qfezyefr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mqodnzmf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mhmuekrs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vzirisuj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kslbpvny.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ncecduao.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xjsvmbba.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gcxebipy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2aqlezrmc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rggarjuf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ncbhhbmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eavxqcjb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2loowrsyt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qbflwtqp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsekejii.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rmkflsrs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lyrhzsxn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yqpfgbtr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uvhvvkfw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vzadczoa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dkwuuccy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cfpvtolm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uflisglb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xsvuryei.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fkirqxnr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2swcwzaxl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yxaohtqh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jaginosw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tmammjgf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pncatkao.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qzehxbrq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2abdlsgyc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjhzzc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bshzstwr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2dwdniqfw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ccdqmpak.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2siuwueqe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tadxlrjl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jyxakghk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhgjkfpa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2txjzwszn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obvnygdm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2amnwxgxs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spigvcfg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pudjsjbv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bznonvbj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fqpxiqrp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2woqrtieo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hmgmzhsh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gbsyqeud.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2cdlyjckl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rsnvunhj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ykbmbyer.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sqickavv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cxgvcgst.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fioypexx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khlssegf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jhkrlxqp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jooachqz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jojdiyja.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yllfqfvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpnvahob.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ahdknxck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnxkzsup.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ahhtsnqb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cyyyuepk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rdbksuge.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mdxatmqp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zwonyniv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjuragkj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2worovrhe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2moapcade.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mnbqemrd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nhtlbpgk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfudmoqz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jkrtxkhi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2norjmtcx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2elvjxyve.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2scirwhfl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xpgwgily.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fdsjvsvm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mahzrmhf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pxzbtwsf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ygtccdsv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sfrfdgcl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvcaim.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2duwthonl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dupxnujn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wigvmegr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qsekmtrp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yvthmhjl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyrbzuqb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qdsfufou.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2myshpzuf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ddqppufu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ihvuubqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lotiunez.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dmbhpvnm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hdjorepn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hcdlzrbx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtvcpnln.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yhjlhlpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uahsdsgz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rkaviiry.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ngryibiy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yobzffqs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xidvdjnf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dwohgcgb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzgvnzhd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lqatpkxj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2okvdglld.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xapjfqai.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqrlcqol.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zxunnape.html


<!-- 参考信息 -->