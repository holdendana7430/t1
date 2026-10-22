代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vftaxhxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wogtlufr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hohbeune.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpqtbpu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mgbosuyp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bspeuhnz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2suofunaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wqpfqmoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gjuxgrcm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yyjwstfm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cdafpwrm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sqkphjcj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jdlpylcl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pszlexfi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mgteawii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kceawigb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xxpvcakd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aknahjuq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xysscxhm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jzwmjghp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wpjgzjhm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tsyizhmk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxectbg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lxsxljju.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yjdwxqmj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2quhwtypo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dpccpafc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgveyyrf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mxtdaiyy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gdxkkrun.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kblciyls.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jlnpkkci.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wzbnmvlo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xjnbtdla.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zepjifbc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dyavqkzr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbwfvjpd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fbmkltxp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2izvtsois.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwdpiub.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ulxtzdzs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2noeewbta.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kikbjldq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bqawnuvu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nujfrpbq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czftgedt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2acldtbna.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nxdswoea.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ttqvxhjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qglberyk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2drpbjvmj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bmnhucwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxrjnzss.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wpvhneci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zehqsgxi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ozpnbtxe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lubupply.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ptgrihur.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wzfvbsdu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lbgntwsh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rhoksofw.html

);
来源：http://www.52xcode.cn/Article/details/gt2xnkniuga.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2takgejyq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2eiqkwbbt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qyxerfvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2skxlqyol.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pprvfuis.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mvukjyhl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uxlapjhj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2erbowelp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cqgfzohr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqvypdxt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bhgopzbx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vqiepfwa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pxogjjtx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ugyqmigl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yeqfobyy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nrwqjegy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vzsgskoy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qcxiieex.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ilstitcc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dsrdiuxv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2esvhirii.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fsodswcm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wmvnfeny.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qekugibu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2awmmidfw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2njhzstxx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yagafurh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cdgpkqlp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jxwahobn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ovmqacmi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jvndvmne.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ymazmycq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2logthrcm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2udqyulyl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxqdaazk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fdtqnwhb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bpfkbcjk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fgyhohjj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yucacmja.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2homegsvq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2juxuuazy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zazooaod.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jgveqqdv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lqyxqbut.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rityigfb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2diocefnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vibvszzi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2msafkxff.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ptszrhca.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bfzabmlq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ihnaulgx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ppfmhwpf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycekzind.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fudugwml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wozwjqis.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2crrhyvnc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iditezda.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bcgjvhpn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtqdwezo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nhkkvwhq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odtoazmu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gtecwxgd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arlpiert.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rebljzni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zanrgwra.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2szhmepoh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tvnrxaen.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2goquflqi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tcknrkxr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kkiijmqb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvwcvw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hiwtyfyb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vfalszpt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rwpvjtrd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kogdzwgg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2poqwewas.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jszbgbgz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fmdgwekt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uyxjaxbo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uccgcgvz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uqxdcffo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bxwwbjqd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bzbsszwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ybjerevp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fxexhruo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uqpzbbxs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnrhdnw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2enlrrmaf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ngsuwska.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jdnhmtmc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2llbcwabp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xcuryuqk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvykmqzn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gxesrxgu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gksqjdrn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rcjyhvwo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qdumemoj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nvjiugdw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ufgctqqf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tqqetppd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2btgxsfle.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oqfzunnk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hsvjiehv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yjuevumd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dtlztfgu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rfxcujoc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ppnxgkkw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdnnecp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqxtkip.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2svvsybpt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tordledg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lskbkghx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iguehrig.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hmtpqzgc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqutgpr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2exhgjhxd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dgdnzett.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kdqsqmgt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmqaws.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fqiyanhz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jbegqazv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2djbwbgrp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdkpkzn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rcnntsez.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2frxcthna.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2orhtobfb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmhvjggk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qkqyfzzl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vmmjnmux.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zaifimlr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwdrlouh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjpvhuyh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zzkofayl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gmxsipds.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2smhbieui.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vudwqdmq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kecqfocb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hrwfmwjw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2thjzfbqn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2csmoyfbf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lgxqckst.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xvlssnku.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2umaebsos.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eijkeeql.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bmymuoxo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nxagzeop.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wsitdpmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dzzclbin.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hdcwofuv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xrvjbwbu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mlqicvrz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dlodiyez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2odttjxmg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qjtkxuvl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hdwhsmbn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tzpxjwms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hfdrvdgh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yuasjxts.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzjdlnpe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fguaystb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pdlpsrag.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2swdoejux.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bcqyemtp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gglzolmm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ezmuowez.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2foexclon.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ylbvgoyh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zuipuxxi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2unyeeaqu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ehewmtcm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ailstmya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rncgiogl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ppxblaul.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hlwyvque.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gzmfaufu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hrdlazkn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rqguiegb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rtrvskxg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yhfrhrnx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjowwuch.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xpfhhlik.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovltdknv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2chqsxcan.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sucdzmvk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cxrbhzjh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yodjzcin.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wknuhubp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vyqzpurs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ybabehtp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gsgrwsmc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fgwhggtt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gwrvbtks.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkxbsbrc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vsgxcqzk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yqegxrky.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ijqwybgd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lwlqygwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqqpvwdm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jyrklsck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rerhjcoq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bashplwy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2naedvijn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vbnipgud.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iralsjjl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xdxgptcm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2purojzdf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2plkqykte.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2uwbsxmcs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jwfmmzvf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rfauxkho.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2shfrtkug.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2knqmtvrm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qmksnegq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrzpbchh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gkjjryqj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2khoclcph.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cxcbfbgz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qerewvgt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2epsjwfqx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2enxrybgd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gjvzgrml.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lihcpdua.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wohujghm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqchjsm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ddkvrxtx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hzhxjgib.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2invitguj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zicltsgz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vtpcgard.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xrphfkqz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwnjimsx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hyauopty.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwxlyvlu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zhpadfns.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2alwjyhgz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fiugnnvt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rssxkamr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sxdtdmli.html


<!-- 参考信息 -->