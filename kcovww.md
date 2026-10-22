代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zvfihpxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mfyaqabd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zjpkwpwh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yqinmwbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gpslcugg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pxxsjlij.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2olkzyejk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahsihdvu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ioieizfv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uxrplfqf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bvbvnzjp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ndijoopb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uxnfodjv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rmhvokpu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2orveejrh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dpfqnxum.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ppvemezd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vnaaxayb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fvwdhbmc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ltclubyu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gqrhkaoa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xbhyatfs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcfjhwf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zrbroxes.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2uvcxkymv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kiiatqvw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2stnzytfj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxzkheci.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ipopncis.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iakoljfu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hqxeyqmp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2otwdhhwh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xuaidery.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxhyvsza.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dmfousaj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rxktpahp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zlbfutvx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rftygjeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mwgqkndk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jcotoqtm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gibhwxce.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2betdwqyx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wanwzwoe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2sqrxgffx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vbvbzkqh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ghfiwgzi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nzfzdxci.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjzgon.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2totrzklm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vdmggjgh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2scqntova.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cafrgczr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sslwooqc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dzfijvsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbsehbqj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2haqowtmt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tvhvrkgb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2djdpjoum.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mcoeryka.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gbaexhkw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tgsextuz.html

);
来源：http://www.52xcode.cn/Article/details/gt2rudceldd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bspdyqkj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2acstbnfw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2axghspgw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qkuoyovy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqtdiu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrzcriy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wgzxgspc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gjympugy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ldvifdxo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gylfvlmw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ouevkkrd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vtfgdrre.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2faozuuhp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dkkmyvdp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hdvlabxb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ubhhvcky.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dfijxlrr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2edgmetot.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2czysckwz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vexgopiw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2akyjgfyw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kvdpxxhz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uwulsnzp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2azmhfcji.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rjrewxle.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bejlwuld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lgzofpid.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dqzkclst.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gvsgmard.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qwklgqzr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qlmhqumw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dhjbjclz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjxdwrn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2thvindav.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrextbxr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ggtbtwxc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrvaoqcm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rgrnpeim.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pgvhfmnt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2bjbgjxvh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vnzjstim.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gabkkfmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rzekwrrp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jfzlkmwj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxfpowcz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2phguarva.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jortcfuq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2slbdragz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jwqatmcq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rlxukzxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qnsltrae.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2addafqvc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwvqffuo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ihyxofky.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2aydabapd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sbyvcite.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iyioukdj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ldfsqfyt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksgmakdh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vpcjobfd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ysfgnfgf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uhjwvyjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrvmfune.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nbwmydkk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mnqlpxmz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vvsygigx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrckxtu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgivjhhj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dfrwqtpf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uuwafexk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dqdzbblf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tfxretbm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jdttvhqb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bdkggdrn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cqkbrjal.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydxspmqc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2trabsnux.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bfzxchzp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vnxgdcld.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xagzgncc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ybgonpeg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2anjwozye.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bzzxnaud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kbxjodfv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ecpsxaup.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2dfoimqcv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xxoicoyv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xutfhufj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2itlfasfu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wirdqwgz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nkdedklz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cptgljtc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pyzvjkfy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tmfgvsqp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lbwbdshi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sffbwezh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pudiyoot.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vcbtagnn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hyelwala.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2azawxwzq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dkrfbpdi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fgolfpmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ummuewsf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2svlgkaoh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sefkjmim.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wdcfrscs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wqzwrfsf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yjreeeyl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oofalfea.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vlyoipgj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pjpiegus.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xizamohl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eohjihip.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vbwplacr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2juantiup.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fglkkdgz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vfctanro.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hncmasve.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oduzeyus.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xfbvumwd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pzeksjup.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jbfrunrp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iyjegblx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vkvtkbuv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zcelltmc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wpalzecs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcbswzzd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xmcqugcr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bkhnkfxl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bnutsuhg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjtknpbk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bnvjgmln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bkckcysj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jegyzqlp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pbaeuvzw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ticrhbjt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gemoimdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dtvtxbbj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nmkskcap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lakjrtus.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vkadanlh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tlovvujq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xvvrfobn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zwsehmme.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rolbbsld.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tgubtyui.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2maxjjuel.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ezdjjopy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cybsuojk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxrsdjtl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ycaaoqqv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bnfybrhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2owlnkkdv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zgzmclpj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxfxojlx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hwfycuym.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2coeihmqy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zklagmti.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqtxobuw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ctslgwei.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xanajwjm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2iogjxach.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fjuetctp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mjmgudex.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfcnoktp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lqgneibx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2elxzbbnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pduecgam.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nchcmjcu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nyntwfwf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wtjuhgmq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qkmylify.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jheprqsj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2npzmqgqf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qlkvjvwe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbsqeyha.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wwkvgjau.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bogtvfmm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dvlkaslc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbtsgoli.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rxkqaeuh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lihpzumm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2eykuqvty.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajecyldt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2liriawbf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hedmvlau.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pntgdnry.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pojkafir.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ifbuambo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hmocqyqd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fmdgivlk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ztottquc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dapgxwtf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bydtahqv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zrmeiaug.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2vwxgchsg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nawmjurg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdqbgelr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2cjlidnkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szgdkyug.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2apdwcntx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zquruslb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2klhunxzv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xjaaxfnk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2idbwctak.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vvarsdmv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hnpjzesx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpmijbrx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2olcnhztc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lajesorx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvbfgqor.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oaqipqdu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zsbikmtz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mdrlisye.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2krwnpfeq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aorfunqi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kafrslgg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qgrpdazb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vxzxtwzh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2twnairmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iaxvcffi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qfhjnpgb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rymxryka.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bgxzqvjm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fdfygsxe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2onfaraha.html

esac
来源：http://www.52xcode.cn/Article/details/gt2plcrtkfo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxsipxhr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fomgtsin.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ectktukd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cfkyopnq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hlccvqrn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pryrhhwq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyliwknz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fprluafg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lrzrngvn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2riljwzxd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bsxosalp.html


<!-- 参考信息 -->