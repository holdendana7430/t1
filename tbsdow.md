代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dsbrpngo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2atgpwfuy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iceudgcm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2djxrvmql.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2raitikee.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zymjqreb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2giqcsnrf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fiqnnppq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vkhmqnrd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dxpifrtn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zmhdhsll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2crtywlqs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ilthydqb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpbvuad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2uckfqpyv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kgnffiyo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ziccoozb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tozobrmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hzwgozgn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sehkmlsl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jfunjmom.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwfjkmj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2exmbaxqs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qzgafoxp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gvtwnlfv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qzzjkoct.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cgebhcyp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vfmjzgxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zxfzhvyh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fkmpqify.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2upgfsbmf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2thehvgrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2eusyftou.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2khnrhsoa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2teduyomb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvbduxga.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dfeevixo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2giphfimi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xbrpwkut.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkxytxxt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ofcsnwst.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmnezmmw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2buouppws.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jdnzdrgc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wvwqktck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kghhtsun.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2stzsqioq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epwtxlle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fxliozak.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrgtgw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nwqtyrbs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iuahavmj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2bqsbxrcx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jhywosfz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hnijonzn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zyrywpeg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vdargpiv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wuccxquu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nkxguxxp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2woqpewkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmqyznlk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wdoesidm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnfebhlf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2adybqvjm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bsbbgywz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vvtqzjnc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kblvagxy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2aemexhbg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2spfqkrmh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cwqbcvmx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2funkaqao.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gjtaylxw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qvppztht.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lnfchdoq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dekmtnoo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsrcyvl.html

);
来源：http://www.52xcode.cn/Article/details/gt2aluzcmsv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ceezblzd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2emlvltjr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qayzdkpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zblmzgph.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ioxpykij.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mewenotw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kxkygjgh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xpvpwrdd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bjashoht.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yjqlghxl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2narxbpfk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rhwazdyr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xbmvkrrr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wbzqjcdz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rezmcubn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fceumkje.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ykfjgwph.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2llawvqfh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2phqtyayk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ndldrwtb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2btfbiepn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2etteclwe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dgpmkwvg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2omkxwpsp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wnnudhvb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2scvsxnip.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uccizgbr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2muegrjpo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bcfqprmz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyovufvx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lsyvhvvi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2puanvrws.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tkdvxure.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pzitdsbi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gsqnrjxw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bstmivqv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uyoafamy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zlywvqvf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nsvufxek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ifxzfrig.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqnfloma.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nztcogbv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xlypjtzv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2sxqctrsj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jywcllji.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wtepgdlh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2pcgqsfvt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ssbgzmlk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2taarelhg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idzxcvct.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pdadhpzt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulojyrow.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pamwsxwi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ecrtdfze.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mkfhlwmg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvfmzruq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lxcspeud.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jsrvilxy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fuozujcc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2drmpwqgc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vffnzyqj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ngsslzja.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gwxkqlar.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ikaumkzp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bxffsqvv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rjpezmbr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uqkeucqz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zyxpadcu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vlfkpmja.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eudaidvd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xbcmupjv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zoaofbbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cvrbscaf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hxljbwrx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqruta.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lxkfnoeo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jibfaore.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uwwralwg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2acmnornd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nmavdknv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2aqjboyay.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qhflbggi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zsxfvznj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pqjlcwxr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bcrxgqbz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xdspruqv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbwgcqmc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dohmzvss.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gzkfurnn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdfwxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yorjlymq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cdxlsowr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nffitdgt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pbzrgmll.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mydzejby.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lwjarctu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pqeqzdpi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pmmefoee.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2llvxjlrr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zzbcrivo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kbeusvtz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hhadmeaq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dsconblw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mgycwexq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cfyzovqf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2anwkmzhz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qpynmzbg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2btidlhei.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ysneoigi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2becgiunh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dyksqbct.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nlcirxzq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2didvowgx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hyiobqym.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fsbnsglt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hatuzbpf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2apbqouuu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2etvwbznw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yufqrwcb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fzefkcqr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pvwtdztz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ocwrgrpn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ofakpbyh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xmieqlir.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2irbkmtlt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dgkocvqp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqthvle.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qrarmpvv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pffqemtf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lzdggvfy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cmbgswvo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cfvfbucq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dpiepott.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2esnokgfl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yewzzlqa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tvswbipu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sroptjil.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pqocqsnk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cczpmppe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yxeqoxwi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jqkwpyji.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rrxsbazn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxaugemr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2guuudzav.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pqzfheyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2haakqzsm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dhafmzwm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jrswtinw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2aufvtytm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pgpuvwbc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wbsjgsmx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odboxqsd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lqsqscts.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ecqghdcl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2euvmdrdq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dyydqnbk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qqrhgdai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eclqfefx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ynvdoiud.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gnjogptr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2blwlcnyu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cdxjqegw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lfmmpygb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ldgtlsmx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mvglcqac.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iapwtvdi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2elgcschv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ofgcoupn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zubdtgzg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kotdfpjj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cijocddg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rdbmglev.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2moofhrim.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tglbdryk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtxlnivz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lhcovtpa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmhantvr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pdsvvwvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2csncjega.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jicelico.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mtrvwmxd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zimvnraf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dkmfqoru.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vyvewqys.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pamvpwoa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olvvwwda.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cucwbvag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ebenmblz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sonyqdiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ngnuptnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mefxwzjq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oqxcnuaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kabhhhld.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zeznshjr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2aopyelke.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kvylclkf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xghxfdrm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dfkqmzeq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2pcvvifnu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yksgpphj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2itqzbaxg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uypjdmhu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xraqvxgr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pepkesib.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uuntvhpm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2igqupnzy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hhndoqdw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ktlbxdtc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mskjyqqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ibjrywbt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2quglvran.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jkmkflpd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2svfxwoag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hwggcfst.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zkwcnvjf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ukftxega.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hlluvjzz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2phnakloc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jpecehow.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xgmelrho.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjcbxqgn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mtdadqwi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iueglyey.html


<!-- 参考信息 -->