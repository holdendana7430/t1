代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kwzgmbcs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fhrcdmnu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whxbervd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3anpgmqvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gyvzzego.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pofiqcsg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oxbcqicd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mjiacqvg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kpwogwgq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rjsxjvdk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lmxuafsj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bwiidmnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3strggqmu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bfpcubpl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3plmxeynh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3govfadij.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zyocrswq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kveyikgj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ateqjbzq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qhetimkc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ycugashe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wzpqrtwe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3krzswviu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jtgsmyhr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yfyknczm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bitqlmve.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkclgvka.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3oumxlakk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3njdxlomx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lujtbkwr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vnsgxhnt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3crgjpiuc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rosopmke.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfzadocy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxxcpbpd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qmahrvzw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nxibdpwv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ycwwdmhw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dgrueami.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yqqrltyk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3dlqtijzh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhakoe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gtcobkqg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3eeauvhqd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xqvxexrl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zjulgevk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iudlxnqq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wfkcxkqt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvfcfk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tafydlju.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jbpgwpib.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvyijhk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hepmbpjp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tqegpdzp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mtijbrdb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zgcbsrgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnxhdmng.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jaebeqcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuvhopmw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3osghdayg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3voemdrou.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rmsfxsuc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ebdrtule.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3sgvygkat.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tztxyxmj.html

);
来源：http://www.52xcode.cn/Article/details/gt3ftvxrkfz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qqpyzpbx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vgerqekl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xnyomavv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oldeojxe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mambkbcy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lhbkkwqf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vcnqpuqg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mhwutruo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pjfrsdoz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3etksrwut.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rrfsshkw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3osraaybq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzwdmozm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lpnzyxmt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ywakekwk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hdguthyd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kxebfzpk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zgbitopw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vslhnnwm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3toottrun.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sodocpxs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3viswknvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ucvvqhcu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kimvkuoi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hzswqoha.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yftngzxp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ivkiqwux.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fwwhhaas.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qvcgspia.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mtrirzgi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ecoezxcr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yajxgovh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kuchwzem.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3adrkrydy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eyxodhzx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rgdbpvyd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzlqwckr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ioiarbgg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qsuxeogz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xyxuojsc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3slugkzym.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nqfdemzi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3iuynvbve.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3euvvsezp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hslhenhp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3okrjtsol.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jzhwqdiu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3srafihlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3luzqqzgy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3effaqvgr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hmkmmvgf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xynguyua.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ioauyhke.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pszgnoba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tuhzfaxh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uduuxkqn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnhiapxu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3masmxzrm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uynyeklx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rehzirlc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cctwkcfy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zaadrkuh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mwdsydge.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yhtwbwql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qjewiuqa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dhazllhi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3smraqypr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqbnslvb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qfeejlar.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3agdxxkns.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wuporumd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3llsoreeb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3udhzjuqm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bjhrpftx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3clhhoihf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txlbukbi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pwnowgnd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xicjijxv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3srniqrcf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jxutipjp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tytahypl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qgdwvkqs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nokgqadk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iuhjbicq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jvuexnxe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sukdmqtu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ksudhtlj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gvdjzonx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qeeesnpv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3pybknmkd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dvviugto.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ekkjheis.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3andunepf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wxybisnt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xyoovbhw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yqsilwxi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qisjfbnr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3thcgpgru.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dqosqpck.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ctntydof.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3koqlutmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qysrlgmp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tvgwkmon.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mmisxhcr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3iyyuptnv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wxoivgrp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tfheanpk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xzbrdoke.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ojifkahy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ckftladf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3amhbbclw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gnnjmvrz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3atkwbimd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cjiwymzc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rslfrsty.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pwpigyqg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3huqhhncm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lczzekpd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rtwehcau.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ahxtolxz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ehisksho.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ezsrmakp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3okxqaskj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mjmvubpk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3stzryuic.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3doavhbgd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxbgucae.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3solxakmd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wabsdtsd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jcagjlcx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzcpxujg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zbycqnpr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3finoiysl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xjttbcft.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ljcycikn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nlnitqnx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wwdqmfho.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tgekzywf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dbfmoecs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tcuzajod.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fgagkmyd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bsgqwdtt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jyqafclu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tunsxmdn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3quevcdoq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nfihmmzb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ptwygadu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rajzacyr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vfecvtps.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkixmtqn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3auvaxjsg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ljfjtpqe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3osdwzbzt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hfjoarnh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sqxrtcwb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tvhdkxre.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gjzcffct.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3idfkchlt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uceficfa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nthkahpi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ihpglipe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3doxnsbvu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ayohahuv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vavusdvf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjicqipd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3giuxqqid.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gdryetna.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3boamztcz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lpjczadg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vfylmjlu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ytollfpf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rmnaelkg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vtvxepax.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3iueyqxar.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hnufshmu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asmajqps.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cyeocyqa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vutmbjlm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vcblthkw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ztzziaju.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wkewmpqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qiajquya.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lsxuvwza.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmvdeyco.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3urflaivk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mufcwxff.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hfrweroi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pkmigkwn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tjordkwl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kmkzjnac.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3adqzuyiz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jdefsxkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuepninl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sdhwwdji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3grjqxeax.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xlouvkhj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mlxqgcma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fioogegy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3povrzowu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xczersgj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jorprxts.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hdoknlhp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oncgpjtm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xezljglu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hwnjeall.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kiukgzxs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3viwcwezh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nwoukozk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nhgushyv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pkyfwjby.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cobznofb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nwjdtzyf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rsjvvdwg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rkhcdqaj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3irvlfpfn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mscdryhz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ixsfjhtp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3szvmokmn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xskeynda.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xhburbso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lknokvhs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tmpblrfp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wvantzzt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3uwlxlsre.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rdjfdrsd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hpgksbkj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3syflofyn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ubdehmen.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gsncyjlc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfjybtal.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vaokykic.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lwhqxrgk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwzkeagl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3czqcdoni.html


<!-- 参考信息 -->