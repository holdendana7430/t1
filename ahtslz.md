代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tisoagac.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cpwqyokn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gummzbxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnctnyw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fcuygtik.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ziweoamb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vjfclhhv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3msqteylk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ypmtrslk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cmqitfrx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fsaqcyqs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3stpnqptm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ncrrfagy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3korzeoov.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3icrplbpt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qtabhghb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xpmqqraq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3njsmhips.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vpjncsku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bvqsahwa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qurvcgsg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rwjdiomx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3srcmvzjj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kowqozpu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uaprkbrc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3sdmeelht.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uvgejari.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbsgfobr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ydlrdlro.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pqnoeuac.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khxovzmc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3naqpmkmh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mzdnqlqe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bozbwteu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xtitcjgb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3afgrjubn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ghqjtzqt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ounrsury.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bkiujiag.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzivageg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zutgqiey.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3urmqydqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wqgpfteg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cozwmzye.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wdjstnzm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ixcndkfa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lvhitxiu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eslypaoo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nzpgcmdv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fudaayep.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ayrdrqfj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fimvwkpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlgwdzxm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3uvfeosjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxflunnz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mprzyfzt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vhbnhqkr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nhcubhpv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dgjdciuf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qraloxre.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ntoyjbpn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hjgxkxno.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mdzivrej.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nfdtbmvo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ozzwavlm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ybrzugdt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nccjoihd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kediyfkz.html

);
来源：http://www.52xcode.cn/Article/details/gt3ezorghpe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tackysba.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bcumcenh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nvnuhydn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3avsibagv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yrssaais.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3szwoohct.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gzvpkmir.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qhgyvmdo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xrbiyqzg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ahbvtbgc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xaekskyi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qtdlttmj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3bwvziurs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ygnohvzz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iyhjgbil.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kahnzekc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nmoaaqev.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xdxabpsj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vagqljir.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3isksrpvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kovvwqoe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3llqhlits.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wmnohtka.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3sziialxk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ohnuyeii.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fhygxlta.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lfdsamdg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezlsvlsi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gkucbuwv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezlrmbyh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dfqruldm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ssfhgsim.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kddhlxch.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3awnedxui.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zepvcebi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3olqesfno.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvfsyatv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3olsoajwl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sqtcxkyu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3alqhnkcp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qpvdqsor.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ugilngwo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bvdnofat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hxlvtbkt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jlmvjjnk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vunnaybl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lcjmcbwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3stqjjgjk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kdxcscpb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjtxdmvr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ylnweoyk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozwcwhcd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bsxcwmae.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lwwmjwtc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wbpiwmfr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgpvqjrh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3isinvukm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3czmdjomp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wiuyghaz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dkrjzxvn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jyjmrxfp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hxcairso.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3csfunnmw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3unvsgxay.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mqoeruqm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lvjcakft.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lexwwbjx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wedsercj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3exunqdan.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dzuguunz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gewexifg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ezgzdkqt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wjvkbzxj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iwxwliwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fzskbrdg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3powknqxb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3evulnyol.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jkcrsmjr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vxiicibu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fzjfefyq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ustlwwrb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dhrgumtx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mnkuqqda.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sicvskzm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3adibvsms.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kjocyumr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3leywqtun.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xzvimxcr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3psvqtjdu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nudqjxti.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sqohfipp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3upyrqakh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lgbdinly.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3phschgvr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ppdztlri.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3erirycgl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zkktxafa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hilzmfly.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wreobtes.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jkktidcd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pfftlots.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ckkwxuro.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ksinbapl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bjzhazaj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3tkqvlkyb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xxrhqaeb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qydqimbr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbvvjh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ytwttdhn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3svxirfqu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bljoylbq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rwukngrl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3tzeqacbc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cgseklwg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ogswxmto.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3osoboiji.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3majxbtwb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gdbrsmvt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zfoxapkv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edilwavq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ffuqlkeg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uempejvh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ztxjsypx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iztyrluq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3awpwkdny.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wncgomnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qlnuwrud.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3eupfbafb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3swygbdjy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qaqyzkfp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hrwdxkfh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3edtnodvq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ytgmhylf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gckjovia.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3teaimksb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uxnqbceg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ppleqkgi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgzccu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oudgrios.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3idncnnhs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tqlhraes.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kemytbhr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3aikzurih.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3znsagdoi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qvbmhvwr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3oteeqqih.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hsvblxgo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvxsuoam.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rftdbsul.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3sknncxvc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3awhgbzqw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkgcwzql.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xnaiemub.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3encwbgoj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mzzuhexu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vvdfdhrn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bugerarc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ykzxmrcc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3miyrnqio.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lgxsqbng.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tjskqlvv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3upaekkev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lyukcfca.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vsxdysex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vcdsdkup.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uajgeohm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vdyekaan.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qvzqztdk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqineqtx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uhzowign.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzkhkaox.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tocqvayk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwqmkxmy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rdtadpjr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uznbbfja.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zlnqruce.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldbtoonr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3muwgcvwh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vxtselwm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ylpueagy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lciyjhxm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbcrdwxc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tzmwzkpc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kyjkrtps.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3celysyrq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imlyxcpe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fwlpbtuc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mxpscgyn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3masegdpn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nadicnvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npdhetde.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gyoeprxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vydudlkz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3varlirxi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cdznuusd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yvdtvqxy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nmcwsjzt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zkdfqojp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sekojonw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fuczotfh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkbqknwx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hnnvovdo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jsrawokh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jamlluue.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3erjlltlx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kjbzjenr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncagxesy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mowpitow.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3snrfesxv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fnljgaij.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ylogtnzl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mnixqfev.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tiznhmtr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jxrshbhy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ghownbkf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vdlxrsvn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3feqzcmrp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ijvzmwbb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gohzptqv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dnlpqkrd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzbeydqq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vospsvmh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbqlsces.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vabpsopm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cerfbssn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3srpxmsbb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nrfqnndv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xthoilzl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uqaflffh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3phfaudsx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gazzjcmx.html


<!-- 参考信息 -->