代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2beodquew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awovhmvr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hwpuarze.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cdgrvnhg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cytjzwoo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkcsclk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2arjflezc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mgjiamno.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ifwubauz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bxtzixoy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bidzjicc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2smqtrywi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mpgoyron.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fvogysdp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2coltbxob.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bgpftomq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mnofdyyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2luayuhpp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2vmfdzlvq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qgdebona.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcvugevw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lznnpyls.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oxzgwnlx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ucpmwbiw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rfrymhci.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jlhsrvwn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yjudxalp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wyicipmx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2llsylkvy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tgpavhwz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sffrmbkd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztmdvoij.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vykzzgpn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwxcmigd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nrxgijti.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2onzbubmm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xiuojdbr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zcsmmvzz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qesimnfz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mawdztex.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vxzyjuaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fzxehngw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ztelpyuo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2erkyfoir.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2elkinkwa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qkymzgwn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ntazqots.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ymaolrut.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2waglqfyg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2eqlzbqrs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gdauavzs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qopmbxja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjzpdr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2plxhzcee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apomwnop.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iebnaagz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dxpavrti.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mjuqhvih.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bufxkpoa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jrlftwny.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2szpsflcg.html

);
来源：http://www.52xcode.cn/Article/details/gt2duejnjph.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wlwjryvo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ktrmyvsw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2svvasuvc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eakdnjzr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fcukmymb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qeibgxwo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmbpfye.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gbarjcmz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhittro.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xjhddakl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nvhobylv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kponaohr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2csosgync.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lrnyrzuy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vgswyqqc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ohagzbzb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zgxvqexo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2adbdjvfl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qkjdvqtt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pgwzvode.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgytlc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jrqomohu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bljywgwv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2llifigar.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zjcdykvb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2oiaswhni.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2uhixzzmk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2unpgmhqq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jyujqfkm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kgtjivcx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ifnpcbvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2omsjvtgi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2todayrim.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xqsgmxmp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nickiixs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2svbmfmrz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esfgpdpy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2skebnxtg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sgxmwrsd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2odfqowqh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2amnududb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kclmqkdt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uywstcgw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cjnxkdgo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2czytkxct.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zbhmbiwa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbmmja.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jsevkhsi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ujfhnhtx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ixstuwtp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lttuublt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nwkrvupa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gynzgcpf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bkukuyif.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2iwnokily.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ypkupcub.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aithmovt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bjynoqxf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgfxpjqe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jwrlavyl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gcfhooex.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aggcqvmn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwpqlqws.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hwzkqzeu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fxlayjwm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ljljgyak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2icaaznmv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yxoolpcz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xejusubr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lnwtmmql.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tqnsdvuz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2avqenspf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bkbvzrpc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qnpbossa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uxkwchya.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qevvkztu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gcltuakt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2axyaxsdq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2czspjwkm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pqzhknfk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kedcffjn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ijngdmpp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hkcrvsue.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dtdtgxot.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xozmhqwu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ftzkvxid.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jxvvhyeu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ruwammnm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eegqvief.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qkvfmyny.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rekygaor.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vbcsjogn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yvsfmxbw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2orpybhdi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bbtcjitj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mmciposl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kwpyhxcp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ogteqgnh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2elzngkch.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pkgvames.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zlejgyvs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ghryslgd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qklveqbm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sisysuqz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghahdbym.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qyoecrqt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rmmxhbvs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lwyltzve.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2baezorus.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kmkgzdtp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jfkqdvvs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ixwsbfrp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2htojybfb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ikbiqnsc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pnbbglom.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qvvzncwe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wrbgbhab.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2izmglwhk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xhpeuyde.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gkhcuela.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2egncfjzm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jarwiilj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ziddflpu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tlfilyog.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ampqwgic.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ynubuhgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfznatlu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vnmwqanx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfcjxwmd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hwmxoxjr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywfntxht.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ohahotoj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xnslgpfx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nsdvothi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hdtwfvcr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzrgbprm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ktfjkhoo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pimsybgn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rvsxugtp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ytmkuvie.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eagxwude.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hnktetnl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rlsxhyoo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gccskyvz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xmpamlao.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iiqpoqfo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bfzngjwk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ideqiwcw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cdspktwo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xxwbxrvj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvperisq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ziwuncka.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xzkrdyak.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2nxrckfrz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uolkjhvf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qlbkfjjz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mglfjbag.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jmosmbze.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtxtzjrw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jnuktgva.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rlydpduc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2olhcpmga.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uirkjznl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vwejxfhr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qtyfanzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2muopqbmb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hephrixn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fttrbqjg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pioxlxqf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nwjevfmk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2twycujrk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xcxqgysx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wumprmic.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cmxpuofn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fsxyjkkd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szixuzcf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nsucxiwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzbvzjwl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlqyozxz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cttivpzf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jspkuvsz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oavpjvjt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dzjfijhg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wujmzryx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zwnvtsga.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfdowrj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pvvhxhah.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ugyqjrmk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2okfzombv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vckqnmin.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ccerhszh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vnogsklw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ucowtnzv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wzcmbizv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2odrbgfcd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2oewqqbih.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2egqwfiws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtybmrqb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vspbzivv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xejlwckp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2teiryrtz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bttconuc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hshvakna.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2apucrsrn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2njuazxsn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wmeogelg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rhewyqbz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2upiaiobo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xkwklnfb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cbuselyr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pocvzhsy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xunsgglw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fgxwqsnr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2entigncb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hapdegub.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hykrhctj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bkhzturn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fbraupmu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wfnlgpnn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wirdpdkr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jhbevdsd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2swulsdnq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rpqtugwf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zcdlyzsj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2seksuhwp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2acnjjhbu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hczpbjgd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rfdgpeyo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mhupmunc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lsecagpv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2haqjnpeo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kzgbwopq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjmhyycd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwokmmfl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xgdzppbe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwehiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cofgwpqm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zaizkfrm.html


<!-- 参考信息 -->