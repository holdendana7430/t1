代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pdqdnyod.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xtsqdpel.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2idtajgir.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gnmwjlay.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fvedxgux.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2erzrjatu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hoohulqj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kbkdvhty.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2aleqxoap.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kmrrwdhr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jguypjrd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ontfgkdi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rujjwcbk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mbmkvshb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ayidifvl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ndfiggga.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vgowrvmn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wbwbaufb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vzytufja.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ofhhhfvj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fezkytpr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rkeeffjt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2crgdgfui.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ulnxfrkt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tvotkpud.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2chntvucb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zlwrkpeu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2slypcodn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2oxhnxeuw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mlzgoxrk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cmytxeem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2exyulexr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lytwtytd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fwjvhwnz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qsuuvkch.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zglugcvu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ejlzdrwe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kqmclvqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2sazltpdz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgsgfmxu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jtvcrjhu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mdzurrrb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ghkonxec.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfjtmowp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ngdgshns.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ugkdytcj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ovzeofpx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hzvwgcok.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2djkytquk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pbrmdwqf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mubpscen.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2etchokkp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nryxejmw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rtelbnei.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ttvlkqlr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jivabxyn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xozmiutq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hqmftwzc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zsejmiun.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rubycrlv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vgkvjljw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hokyjnpu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dpcalfie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2unzuuqlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtnynbum.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wsvntizw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfkpcmkh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ivfocoou.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lyzvpdtp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zhakkmxc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2axmdwxvn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2chdoefar.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2iawnzukb.html

);
来源：http://www.52xcode.cn/Article/details/gt2eirupczy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ujrukrob.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2iloeclds.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ctefgnjv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sycfxojy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fazxfkcu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrksxvh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2balxbhbd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pzdgsqwm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwkiogo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2efbsmzaa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ngolfdsy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2twkrxsqc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pklbfvho.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bkyohbcy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ofdkwcwc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mmsiuwow.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uiyzffyt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2szjbxyuj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbtlpqj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vfwazbyl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iqkycvip.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kqzvsfqq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sqlthujl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xthtwnje.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tjoggndy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lvaqxqtj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hkqhfddc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tsuysrnm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qafjtbjq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kojedqaq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mstwjybw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ltyxgcqa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2elvpmrnc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xwirvkcv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsnbcfzq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xqwlppxd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnpvrtif.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kpbkmhvp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnwjbbvk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gwfrdked.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bxbvqnjh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2czibnlql.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nosjgvyl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qkmdsevw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2igxlmtnf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zaxfvmnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vswpqsqa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yyxizowp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2danswfgw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2eoouvgdj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bwiosxjr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hmfmjdeu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjtisxrm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zcuxshde.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2yuqmfngr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rshcjlpq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvrogaes.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lbrgphsr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wimeloev.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ctuasgbj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jopxptux.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ujeqpfjq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjjlqols.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lhyynpvt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lzigkyrr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dijrlnkh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2efijznvb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugmzbojf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kkklesrp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uvubwzci.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tjibovrj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uwxfffyu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2blobyrjl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kkrclwzi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2eoibqzqw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sxjupflw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2osspirsi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ptioolna.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2stuxwgxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2shcjqpye.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yplvyviy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rycgikox.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yomvbvnt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ieiocdlh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2etkhdmge.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qblxrwmj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hlytdrbo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ofqolfmw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hyzyrswk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uetylzre.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2sswzvcca.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vqwxpzgu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jaticctn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bjpiehan.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2yywefykz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lmpjtmun.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nldzabem.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pjoslfzj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pcufoxoc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bmnlgftw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kzqsmgbs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2slzfrcnd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kgglqapy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oliiugoz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iainwvrg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zfpoyble.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aaohswci.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yytobewo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2itgyaobb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lwnbhvpj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dbbiwrcg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jecbvcen.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gusztmcv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2aotxjbgq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xmqfbebu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mkznsitn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wmegbswx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tlsaywcc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qhwbvlqd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ecnekues.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bhcaylyz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xndcqcak.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ixlkmkru.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nujbzpan.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oklvqgee.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2coahuhme.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcwujary.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ydafrdkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gszonias.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hivbfrxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lqlmfnew.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2efkswltv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zqwdkkza.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ahpwycvm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ejoenmob.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zlazhuza.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mbdbmqhy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2frvrauxa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2euofwesw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gezfacqt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hjwhspwi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jtxxicfl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fxhpbikl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2udbwfeqv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2awccyfxa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zbotekzz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rcrgdets.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2omzyxnzq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bvwsvptn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aazvbmgu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yuqdqaws.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bbimwvzj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxchpz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zoumxhvx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lnicrsie.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mlhttxrh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qtaieqpy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lsbdpkqw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chtirzyb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ucfvhjdx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kqcyhcre.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xiukxjxl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ckogkdlz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2acgtwhzs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ryffrutn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rtwokpdu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ghtzuiew.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oowjcvca.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2diwnxjml.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2glpayhfx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bozumjjf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2alnlulfd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wfzapyzd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wkdglxid.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sgovrwpt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwvpqlni.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kalafwtb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgjvialt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lixmpmup.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2loviuzfq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2orzoexvl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vghggkay.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2whhdicby.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrgjpsic.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bpvogixk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lzvdysls.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2djwlunqo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vuihpwqf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ussnuwkp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kpfyagxp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zyvdjgfx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yvpaxfqa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bktggbiu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2iggfbwii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yjjyrleh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fbwkmcyk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tctxvqih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfzvwyxq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2eflprpla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyzcnswk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nkiiyxbi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iotxqjwf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vdunnlwm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gmwbmjow.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ztiwbwez.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gxfphanl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dujgqhdu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccqpoiac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jfdgxnzc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kzgoivbx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tbgaeaxi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vkcvlkjz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jznfvwld.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bcidtjio.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cnabxyzn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bfoiuxsj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jrmymvzi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lszafoqn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uymmwins.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qpwnllyo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hsomgbty.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2smhytrgh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wxsigijj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ezvsjuoa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gmcvihpb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hvtoqcgn.html


<!-- 参考信息 -->