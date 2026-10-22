代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nxrgjzkl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gidliwti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iqdpccvl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2idofhbun.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nycdgppj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2swyjzdqe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lfsdgczv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2exeqawet.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2awtdduwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bchbskkw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cvabzthu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pnatmfzu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yohcbkbj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jdhxqwct.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cfymkjsq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wwnqwqfl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xiahevyn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ryeimodc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jiwwmcro.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ffosvfyg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qcmsdqbj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcmaataj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2snbjjgxv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fvuqabqs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mxibbvjj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iuiopcsj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ckyhzmev.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jyrckqkm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2spokyzsp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lclaqzmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fruprptg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbnimgs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2moynmddr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pzyulmyw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mqiwblnd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gtjydfeq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zauvmznw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tucjbjbt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dxsdapnf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cyoibizp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ocroeyff.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2udpwyshz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mtuffvrz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nthlpuna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcgubaht.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xntpbvlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfipznnh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2prhwihsp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gdjsvkcq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jbthovcp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ovswuvuc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2poumvuqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mnbhaaah.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ynuesvpv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gabrsmpb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xdtjjjhd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bttkjrav.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gqaaelcf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2onpxqtxw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ynvhdkym.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2toxajpcr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2azsgbujc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2suqncrmv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nacgbzve.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iiiohpvc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jkenfjbo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2uxmislsj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pfirzzwk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2utvoospi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jrkceoqh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dwrwqdpe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oburrsmi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xwygwoza.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwzwcinw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2brbdtibw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uxgljnjy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xckbyffe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rdfghzos.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iejvgfvv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qakjjact.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hkkqbvau.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pzwuxqid.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2irqmheyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zfnntokx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hfysymym.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2fprthqgy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2srpraanq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wjxzculg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jheyplvd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zglnrzfd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uohaezbw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2meegfxdx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2grtwrnwn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mkttuguo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vikhzfjg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ywskrzaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hxdmcgae.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cagvesvo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spyjpyou.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gljouvbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bmjetmzx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cxvzjgly.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jafyjrov.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hybxpqrs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vvsmbfah.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2svzwomoq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwzcbyqp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vumifwoh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2agnwrakl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tqlynzsm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gogrhfur.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tlgrdppp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2itgyhgch.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fpncqppq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gkmchbra.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sbrxoogu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uysfktps.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mjfyrgqj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qxwmpmxk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yzhjrupc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ampaclqg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2czzzrycw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uxxcxaeq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dxxkiwus.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rwnhhgjg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tmvbqzvf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2osxxwjah.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rlwynsia.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gwakrjue.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vculiqub.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zktfqsjj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2apsjkppw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2evchbsxd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jduagrcn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2illltvva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rttdcduj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xfexbgzs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jydvnjyy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yxsjpvei.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2limlisgg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vzaehsiv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rgsggcee.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2estvvyco.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vpphqpej.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dxyqmyui.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bbineagh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bakmxrvn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bsmiyljg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pvqpglgf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2tgsyrzqb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2scnecqba.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bgxvsyzn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hlkozvsx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mpigvxez.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2syyrtfgn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2atphkaan.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2acnmvuio.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tomplofb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pdmzcybb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2gaivngss.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lesrftav.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jurpmdkz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2plmsfbsv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tfghmjat.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kxuolykk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xcnegxtz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xbexoixj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qrbjxxop.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qiyuzbvl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2telcciaf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2orlctivo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dscgsfks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oowudkjo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wzqgvaaf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpvazw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wsocgkde.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iwjzmpiy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ukpdpkao.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2elypcsgk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kwrsudkw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2whsxntdh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ebvkzdgb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rkbdximf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2erpxnjfb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xqxpzvig.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pvkhvgco.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mlddcoth.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2huazfegu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sfrfljzr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2erdbshgj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ghqxmqim.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lercikzu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ikaliadv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sdyixjav.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ntrirytv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lghugrmi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yurteshg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2izvygbuw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ogzskggu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ynevcuoa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kxswgogd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqtoli.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fdhlglsj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwyutdbm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2exwgnshs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2imwkvknc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qkiyvbjg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zegagzoh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gixjdwat.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ddqjqgse.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sfoltwtl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2htdpesan.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asspeskj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2okametln.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2khhcdzaj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fycwxzol.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vvobsvzm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2adjuexaf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsbubrze.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tuvysmvg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xijawpzv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gvxoowdg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jdgbapje.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2sfjzyoun.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uugtblbt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nqemxnuo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gufanxpu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cncxdtcj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wshktbqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khaqsrpv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2akgxhmmp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yeyzueov.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2oxjlrrwo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjochxwb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aqvappeb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eicmozwd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bidqqziq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agizadhn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kcxzfgvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ytkedzdo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2toocafoi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tsepkgst.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zieelpbz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yspmzyhp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ykeaziky.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aqwgrphf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hyktbnum.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zcqgqqjk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ofggwadb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lsjvedxm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vexdwjrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvszadfo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hmlrzwxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikykgujs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2onuworvd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jusazszw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gyymghmv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ssfhslbz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rvzwwobu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2agqnxwqo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ilesnzkm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mmehryjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gmaohtga.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qmrxqhsp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jytpvzku.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rxblvhag.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aohrnvbr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2blntzotn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2saxahpej.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lgewwpfh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2exokplzs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kqmsngew.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yjclvugk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2khxrdorw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xfeyvdjs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2frqociml.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2grjekyoz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kyuprirk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xnevewcx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rwiouvzb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2giohudir.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qyusqklf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2amrsafzg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hyrwyvgn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2glgtqgqw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wohhgois.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjfeheqy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2octtnarj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2adjcoqqx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xnpovvwr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tqxgoipx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qrzahede.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvtwunrj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lgloelkp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gvrrwtdo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2taitwucu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lbeghcje.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ikerrhvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gudnllik.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zwemhcsx.html


<!-- 参考信息 -->