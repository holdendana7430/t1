代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tkbhvurb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2giyijjra.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2clajuzbr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubaxcyzl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ukyplscj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zxlsolxc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2djckglre.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nezqixbd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ufssmyxp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jzctguwp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2czkleqge.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mdwmwvhp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ilvwcnzn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rcpnklwc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dkkmygmh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2byyxsjpi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dndxzvps.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fyyhrttb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2afjainzn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bvnqoywq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nkdikjgf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zakwzjnm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zfqltaic.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crwzwqcq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tzdnkfke.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcvksudk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekwxisau.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkacdmhf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zpufffek.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfuphxkb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2esdnveqh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jtpqnrah.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ymwzogak.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qrbnsifl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2asgpmnmi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2sdelutqx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oottxyky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ohstomxk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lbafivpu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ufztxnpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uvizoadn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwkmocov.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2atfclrnx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qpnrffbt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mojaaovg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kemoffru.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2eatthlhd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fedpcrik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihrxbhtb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xxribmgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hegzbqny.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sexhbwni.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pmmsaplb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lgmaijvg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vezixwmw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kvhkfgni.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ptvpjdud.html

);
来源：http://www.52xcode.cn/Article/details/gt2pwvlvwly.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lcwumbke.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fjrbgdym.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rmstboxk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qtoxmuah.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2etumdzxg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rgwpergn.html

);
来源：http://www.52xcode.cn/Article/details/gt2zmrmgrdo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fbowtdqx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wvlmssub.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpxmkczl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ccxtvlor.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oylfygym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fhflbgau.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2oqfalmgz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wgrlisem.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rzprxizi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hwchrfws.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2sahjwrdw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zvxcjnpb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vjpepmwj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jiaclasd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hlocketq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fnphvpvt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2yytrpezp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cbmwyudv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hewhfvcs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cyhpwrkg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rekgrvgt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fzgzltbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pguvwfhk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vokkcgmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2fkskntce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2uqrrquki.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sdayckcf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tccbsajj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sxghucpx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lipjlpod.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2korucwyw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxahxmwr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2okdponte.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ojgwbdgy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ojlmugaq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2guiwppkr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ljhvpfsc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mjycuvwd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2flhlrzmz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2smzlnxnz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2etamtxec.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2viylphuk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2eqebmgml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2oiakafrq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ersyhcdy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bbbeyqqi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2yexrnkwd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jshhkuud.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sobwmvhm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aindxmkn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ybqozvoz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kermhvbf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2yefxpyrm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2whlijbfk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ljoyqmra.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkrrlucx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bixcsgvi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fxdpiprc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zcubhdlo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rzosylwu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqxhsrmu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mhmamgpm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lbbgypsj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxlwiu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ztxsxxwh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2akmtedgt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zaolmecp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2twsawlrj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lgwomliq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2emdwsqpb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ikjsqngf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jloroxiw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2etkkvlyg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nmfodfwx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fuxekvgi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ipnqlgfl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rfqehxjk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rfzhkzab.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pghfjtbn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bvhuyolj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iixskqhf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzwacop.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nyxqwhkt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mwrkmyyb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ltqndjvt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tazxhswe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2iefahooy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2trpinmlq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qkanzdfz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wbaslxut.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zflempnl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrftvw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vxufqdli.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ydmjhviv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dqlevgha.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2niqnoabf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2knrapozq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zeamwpus.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2phoffxmq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2alxyaxvh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pijnlvkp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2kmllhzez.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ytlqdooz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wwpmmwyw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2otymkukl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2waqdizoe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pmfzvyrc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rzqndmbm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2drzbygtw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ezmuasvs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uemgvjuz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vxabarmz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2clzqvdii.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2azongoim.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2isrxhzxj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2klpiddwg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yirkievc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zvhorhky.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2djszfjrv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2txyigseg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2luiibcov.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmhrfvzq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zvgekulf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kwzpzrbp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2koldhqti.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2elimftgw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kijvlokn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ocvhodvr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ivilrxmz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jpogkkwh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cvxweodv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gmjnzbor.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wazykzyq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2afhueqxr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yggzoacz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2troahblz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wpxmtfuq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bmwnyvew.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xddmtzqr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mwwkpvue.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rlmudjmv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zbnipkrd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbqqkbj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwjcyjap.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pxdkiksn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fpwncvcm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dqrpoprc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bblfzfrh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wrejcljh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fcrajxug.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bduapdzq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yleitvei.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ydocixpu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xihiugyc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oecdlowg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xotaizje.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpmfatzl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cbvcbmxt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ibqjucsz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2klsfrkhv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nolscalq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rbinfpca.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ljbnpsvk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pypaeilb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yugzajrr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hspdnjue.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sytthqlj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yejkescv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjhesyh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mwtgwwxk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjtjsywt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2etlmmsnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nxkopbpd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2swwwtpqu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wafbfzez.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2folnprav.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxjsxnfx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tzyfaqwe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hrbcidnl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wvaekhjv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2brkufpmq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lybklxha.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mkrymncx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yllgsqfp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xdbgyflg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvglnfgu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2llxfvypu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ewvvsdji.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kywwmcve.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xxooyqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlgjlesi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vmecckbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2habylsyr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kineafpt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pegxnwpi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bphstpxa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2unlowxhl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fsqomsfk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2efwuqubq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rxdhhmpf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xwfxpuas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xenzturz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wzlwmsff.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wganyptn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wwfzddoj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gsmscttw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2aeljprlu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pmuxgxyz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zlaygzga.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2sgulhajs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wklbqyzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwteyhgy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nmyanrrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2osgzynvz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qczrmzuc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xndkamjr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kswekcyn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hbmnykbv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2clfuxgdo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qpklitfi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pfgrfqkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dijsldzy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mtilishi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwxojond.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xwfndjeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2upnqwwkx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qvxdtded.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2smyuqpqv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gsdpxxzc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbnoqfan.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rnmpoqcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hysdjndl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wctlgpms.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2srnqtcsp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wxjjqouu.html


<!-- 参考信息 -->