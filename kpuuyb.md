代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ludiewfe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rnienksd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vwmzwqwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rtavnyee.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xkosjqsy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfmmorv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hjdbzazt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2drvqrrlh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ibpfgerv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sgfhxozs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iejpgnxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2daxovkot.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xzxrksdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bmoilixc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pgymfprf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bwrvqcxn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hibmyhln.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xspzxnyf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2eylhyqgp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pouvwbww.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gsyqnjqg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2diwbbzjb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddkbrmwm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvqftmer.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2paflfutv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hhtywtem.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wjathkgm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zzrtxmln.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vrobudpt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2frajjeea.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxyqgdka.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qptmmopf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ybgbyyyl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2elclfeul.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lilonlqn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mlgxbtma.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzwbxcj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ebifoxeh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wnyimxja.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bslonoyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cdjyvxxe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rcvhtqjy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2arhirbva.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2umqnvagg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obuqvlkg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cyotdygv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csgfffaa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2eskvsahu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2yrwjqpdz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hatjbetz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ntusyrtd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pmvqxkli.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lollwsrw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfubact.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mocsooof.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vwokncph.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yejhigqo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wpmutnoi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kxhladul.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gyebvmgt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdqshj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wuszmqzp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kcckawae.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzattsuv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fymydcrq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wcpwclvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gjaciads.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2butmluhp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mpthkfnd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lessqndy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jnfhpgof.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vzbsiyem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2spuyfntd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jiwgebvy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hzabedbu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vnrbbrfi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eiozrjxd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vjjokedu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oodkemru.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xnetxrpg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ncjyzzed.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yblhfsgw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bnieewfu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yxknkpai.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ifrnelmk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2swjcxubf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wzljmjmn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2txttnvpo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvqqvhsh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bipkhbgz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2juclczzy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fquispoe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufvlcgln.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zwkcvrxy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qgfeextu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2izntqdaw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tlbcqrnk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dydyejrh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ysfujpbg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sflxufny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mmuvmjwl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ynbjdraj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tlejdbyk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lsttebth.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ennrfxbp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yxsrkhua.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lvhplslu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gmonkrev.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nchufkct.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fipchkmq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aklbonmf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bifvsbrj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plvsumqs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2reetsgeb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pvdznkow.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ogcuptqt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xoxrwlvw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gtirfypq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rxquoqzl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yfihtiwo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfxptgt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2asqnucye.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2upikukmh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qcqhpzoe.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ayvkhsik.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xhyjhvvi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vgsjwurv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tmoqioqe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bdyfckhb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rjpahyeg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dxobawer.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dgpruzae.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dmfxvngc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqhecb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2anarktlr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2oyufbxvr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uknryvzb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2anpyreca.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2syjqjmli.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gzgwqnub.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mutmzgjv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2abohtqje.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lyuakdas.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ehayvskb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qzimzpea.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ngpxfmxz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejwqumrh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qxffstom.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xaerahzo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nordkzgl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nghhpinm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cepnmgaj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gzmcnkuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2duzcgntg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iwubmvch.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbbigdm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uuwqzudn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rkxftpyp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wlpvtvky.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vutpdtsn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2deqmsgbd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mrbxnszj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ipgjygqb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vpvtqnem.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rmyuznhe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tkcghxmu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xepewqor.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wrnziioi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvtthetb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rtherabx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2klhclnte.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pjejdqix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wzijpqji.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vbzpohvz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nfoiliil.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zhdbpxcw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nwpeyunh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ulyyqkvw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wowqjkzc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ybdbmuch.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcodvjhy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ctiqctzo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aomywdwz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qybvxeuz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zelpgfty.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lrgcpycq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2slgawwuk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2taejlzwb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aiujzzja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywjznneh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qmwkinpc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2matnzkof.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2scalmrci.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uuehrbiu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vggobqxx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qeurzmfy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2aaukbajg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uslzfcwl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tuvikqcm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2azbicenx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2atrzcrkk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qdpwvavx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uogbnwzy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2onnapjae.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nsjzvhzz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uthrdjks.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ttxlkdsc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sgwglyzf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zgdqtnkg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ywrgojdj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2regxuqja.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xkssvxet.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijepnalt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2njcfdygw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gmhdlaon.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qkoyvhsy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2repmpriu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qpofpimp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpfhkpfk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pomvaaas.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2sohfvamf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xvsgniem.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2efbkrgqo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dpggmfdf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2novngfrn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tntztkej.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tlkymxrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2srvfcqav.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cttifarr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jeculhlx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dmvmadrd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfyjgrtd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uohibcio.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwjasjbw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vpjrlswf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bykxpmcu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vcdbibot.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swcohqhm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jtqdukhn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yguyofvl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eomfvvum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xvsaujfy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oldjkjua.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gkmzslat.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ungtaugt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2taiyftbo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpfbuuov.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wwyzwqlm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2glrwpbhx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2adrwciop.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnpsgnug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ataltddu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2knkplfnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjddvwxv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ulvggupv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tfleyblg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wxozgrza.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fqwlyppq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zszfafmx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2putrbgvy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lnweoivx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dvonhzsr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ciizqthf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2judwxjbb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2llkusjxi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lrexbqet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjjamni.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kqyjytkd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ebhmfcfw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pwpquvfz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wvkyetet.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2njpalykz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xbyotfea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dvlcyjtm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yxtipbfo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tdmpxmph.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cvouykqo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mbpvjepy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2navwakkr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xjqbnlgk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zbfrgxuf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wiwddgsh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kywgagbe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kbmuznos.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rvwlyaun.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ehgahfke.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gdqjcuoy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdgvfyci.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dlvhkqen.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dksxtmpy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cmxxcnbz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nvlfhuco.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2citbhgsl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2znstbxni.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2paccieta.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbfegmbp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvnaumyn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hqynstov.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqayesvp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hmkszjti.html


<!-- 参考信息 -->