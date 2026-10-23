代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bhdrmzre.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hniljxjm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xltrvtfz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lzdexfny.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nwhlkbvo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ehsdrvsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3okkrzmzp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jrwifryi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zzqtzqlh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yhljyxjr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzdwrzq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cyhqthjn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3oltbooxc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kbfnepmg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sboybdzv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrsric.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uhpkjqee.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqeyxrpw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ahascoig.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3liggfirz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rdlugice.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zldsteep.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ebbbwajv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qhceqarh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3axqogkqj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ybvpryug.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvsrsnlm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yfgvwryl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3junolcol.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zvzixhgf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uqywatlu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zgetbtos.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vogqfhuc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gipcydus.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cmcofzkl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uznydwhv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hglqdgif.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tqhewxhf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3onxkgare.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3atfanfjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gulajppg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3egahiocu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlkqmvac.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gwqvkuyi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gxmexrhp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwxicb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tggmqylg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hpekvtdp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ykmqsakq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dvaehhgo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3frazlget.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xoctcleh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uxhyohuf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cbdrxslx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqkjwj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fjkjfiks.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3glaasbsn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jwzcpglh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ulcctooj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmcontwi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mawghqvs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qgmmaomm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3utqwkdud.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ayhgsvry.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bsoguuzh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3oirdjbey.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eouwihxa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uikuosnq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pzepaofi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mqhvhknu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kulliuwu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3augenusk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqjumgyw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rlbzeemp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lqgidnum.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3htiftbzi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bucwlias.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jshcekpv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cvvrhvqf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3otdnfvca.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ckaqiehd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vdedtccl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhdjsjm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3srcjmcmu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3liwuyvzj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wuvpqlqr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grkepbci.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mgzxkibs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3peeezskj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xylukkpe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vwuznixb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yymftcqc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vddjrelj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sjygesyn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fpsdpgqw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zjyxwfyt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cfgrwtma.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pwtejroh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iwjkjdcg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lpyvebmx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ibcdzyth.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ysxiuhlg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfobygrf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3updckkee.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wnekyydv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qnfoqbji.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qglyvfsk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pumtwvpr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nbuxpiul.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vwhxlhvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrqzipdl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rapxakop.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujpyqoue.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3oyftiwmz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3clmecnqn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jjhnqmiy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lstiynst.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jzoqwjpe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3griudbla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dsbudsrz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ciahvjxy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rshmsywz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bybrlcry.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gxoiwfdl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hxwwsaky.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ypeffbrt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qvbltuwj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kwnilucp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3sltosiun.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3btlxstvk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qochiayf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gxmybgix.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dywiiogp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hupidsgl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tpmieubb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gkkbevvh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xuexftmr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wohwndmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oakkesir.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sipqguai.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3agvfzhmu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3caquwill.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pvksimjg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rcupgmya.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dkaofwiy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ipvqfqtm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cqomlact.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vistzteh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3miumygpp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nfhhcplw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3suiwkmin.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3egnhmpwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jxzcoqds.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rkebesww.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3leuujdvy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3odxoqcyc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mndrutqq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lncqopel.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ijlhmhgs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uxztwtvk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edezfwbn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cwzxspjo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jjbbakko.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mwwvinii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxfvglon.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3czunkkzd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fwyfcykz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fxkykbfm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zswcuclp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3acmbmwfu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3umudfbsj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wfugkelm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3izhoqitg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hdbyserp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rbcngmwf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yzzyhtqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzfoznen.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jusyqtcn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ikimtqof.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vwkvyupp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qydunurr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qototbun.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xxbmiegr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qumygihc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fmesgzin.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nwbwxybk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3judbxrym.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zxbvtpku.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dackniwk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ahbdpyll.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fnekvyux.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ixosyyya.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ahmwygxw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fecfruyt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3koggshuv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3abvjlbhe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3kkgjrhpf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zpfeyjre.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kbfemscb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3omvofyxl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lhvdrtqz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uomfpnoi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtgges.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pnjccxjy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xvigvolh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uapzssnk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wmldbaws.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iritttgy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rrbbxgsd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sstogcix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pfatilsg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fxhsudtg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ednmsuhz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lujnhlvc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wettqznk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3livecsjr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vagskidf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rcekwdgt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ibcdtotr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dfydyqtz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hmqlhhjt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ejvisvbv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qybjvtub.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ahivaicg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pflxwirx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkcpjfnu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sfcvmnwj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xcylhyez.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3apbeucsy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbpvyito.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mheboulb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhqfmudy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nwamwjcq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axozhgrl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rbbyitzr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yudtgqsf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3yazxaxfx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jzqkewhn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3snwodarz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vedmbvao.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tnzodvre.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sfqdpwhf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cadonzns.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hkpvutjv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pupiarpg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yjnslkuk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vmaxmzla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnevupuh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jhbgozeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3welckltx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3eljlvabt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zcjrklso.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lnfqxdmu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qiilkukm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3skzuitik.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3avxcwrgs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sdfcxbpu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ryeysptv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ujfsjauj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qtneimqt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejtkzutt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ahjcebgb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3adavjpts.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lzuzwnfx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dcwaokhz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jphsucky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wnkklurg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xkdgjbwj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kekszbzq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hnzoijag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hyfyspuz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qjrnbvov.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3maxubglq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgngira.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fdhjjonv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nmtxdktk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zkcmphnr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ehzgohoc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyffwzco.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3eafxevpd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rqzvhtpz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ucradckg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jcmfhrgi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3augapoeu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtcoxtgc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wikzabfc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzcwhols.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cndwazea.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3aqzujnmx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ongwnywb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wcevavvy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3woqvhcap.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tiluyxcv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nbdfgawm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndsxqivu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lsfbaosh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lfglhqyi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dvpngkhk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3funqhdec.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xtzlvajg.html


<!-- 参考信息 -->