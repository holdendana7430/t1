代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ymkuqzeq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jjpfaiml.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gvndbvvb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pvghwqzo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vvoazfqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuefhshu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2swoylfxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zossgigw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2klqgecdw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lfevlllq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2enrvjhfv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ahsyfeqx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tsbgmybe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zyuinclt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ibjdkbio.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gpgngdbi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tirhtcpd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ixpsauvp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iocecpey.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcswxhzh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ghkallwg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdkrqjj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ygrjhcdz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2aiijdoky.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkejqmt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2evcbgllc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqwtrh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lufasofr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uuflsdpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hiiyampf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hpqbdeve.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vonlagcp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mwelrypx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wmelykvu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tpeyqprr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kgkxvdep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lhlbpzan.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ttoubcha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zqxhmmzp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wledpmcm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xunygkwe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwufyad.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cqncmwsf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fdcjwudp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rlrpgurc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nsqrogqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gerczhif.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rjlyekjz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dmxkemgj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2eykktxjs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ssbntagh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2nqifgowl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vocdopgn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xphwdcpt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lntkrjbg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezibszjk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2giqezahd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yquvfjgl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nvhoeekv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2idrjzazm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2iqsudajh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cslulfou.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oovucvct.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2iooxizwc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vlzwhfjw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nzljfzmp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2svykcxih.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ytpdixow.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ywjxowog.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uafqpowu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2njxyenzq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rodjaccj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2feuqroyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lomsqril.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vcfeqdhb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xxmynuzm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dlkuugui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lsnxdhtr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ofhngpwy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xeanibnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyglazoj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kddgrvey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vesgqptn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cumvosjw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2peiddmic.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mthsqmdi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ybetexgq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mkpddpja.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kmksajbl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fjvblfxm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ymrstrmr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ummhjjyb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cbloourx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2enwnbsnc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xnrnjcqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mlawpcac.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qfbvkpey.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dcqktabo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xjnrjart.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wcjbbkbu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tlgfuxyt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2owfxircy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2juugpbvi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nxtepcna.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rxklutsy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2idptpxzh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rsxgwsjd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tvzgwyvq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mmtqdpei.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iufmoqxl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ihjznejz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2oipjykbm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hcuxeyrp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2njuiatsv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ecgxtbqf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vuxubefp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ogubbrac.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2fxdjnigp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2uiitkdwe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ygryhyrr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xkzlpcfb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2sbhtwmsy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2erkekguu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dcfcgndu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azeifagi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wwlvzelq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mltjvksh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wuzhozzq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2npykpskm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2djmpfvdh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dkwhjhkx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvxyafwj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2kebjprbv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2teiklonf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lccjyxhx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wfdhqfah.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uswretbu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmzlqhtc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2alpmdbtx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nqihkrbk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ijzzlquv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2remcgzrv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxfxwhuc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ptxmlhco.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rnqyytnq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cucestkm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmyrlnrz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tmrciqew.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stsbupia.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hncedlfb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nfrjvtby.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2snqunbes.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhdooje.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2srmxcgpn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ohwnusmk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rhssrpwv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ckrlbygu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ujotrssl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mednatkh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dfpdcega.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yilllmcm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lnlvjvrt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jodzsszg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vnytdkiq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2otgqvauo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vytwksyp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2elbnqqnv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qeuhbhcf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cqknhfya.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pkpqxvwp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvxtppdb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sovhskjk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ahqrayas.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ptviwicf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2aoeycxcn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vlzgsuiq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zymbzzfe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fvwiduyz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2imggmoec.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nkcpxmmf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tqiabhij.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kgpsueyd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ccgikjpo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jojfexzn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kuqvdzvc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fldpvode.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bpntpyfo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vlrzvzkj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ynvoitgr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dkpftdzn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2aaygytoc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oquekdqf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zrkubmxg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ocuzlhhi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yoakcaaf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vgstgzkx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vtgpomyw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zdcxlqbr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ksrajwvg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jjxrmyii.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lrfcbqfw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qwdoqcqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yopneqaw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2amzsrbbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nvqhsfsi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jkzennan.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gsgqzqgk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2phmlzplo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uqeyevoz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hzemjbxh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dgjqzswz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2khlgybdi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lgbyrafr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kyqszgxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xvcykxbd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dquoqrfl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkxructh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ndyluyfl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohqljwsw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2syvmvwdq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uisxosbi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tvlqwibq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bisemrrd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vpmbnrkz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2azaxuzht.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohrnmqcx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pvplsblk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vcbxeavw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xwpuoazp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ivhqzojo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cxsopnjy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hwzomidv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2oiyscvqm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ptysnkmj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dycjssju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gsgdpuhd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xxqsfkkb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xgyakdvt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qjoxedgt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kpxnejbc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2brhdgpzc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2plkphxsk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ietvmwuw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dfasynlx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gkqdexmg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qxasykls.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ekgxujye.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2psoadsef.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctinssot.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rxaxnuek.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tiwkkwwe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zqphlztc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bgzqcqzm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mrjeqiwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufexkalb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ejmxlbpd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmihdxrk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hehacngg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xgzsvxev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dfknwuuu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ubcjlmsc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ctpfqdep.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sysyxjva.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gmoyclpn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2suxmaffh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mzzopvej.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yznoeqpo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdbrqyku.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gqeglyhj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bknidiyp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fwgdohfp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2msrtzrir.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gnllngln.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mqkaqanh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jpavshme.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2srqzsche.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qsrogewa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dwpzoivd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nabqvtwh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2iorngvpx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bwljgipz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dfxrqfga.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtohdqle.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hakvgvjj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ynccewwk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2uwoibjqc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qwfxpxje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhexuvcx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qrbtkrmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vntckghy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zqxzuvqm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tvgzhvpn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xkuwwwze.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nqnuuakh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2niisvmuy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2lawjtvst.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lhetxaye.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2swnccwfm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vxfduqpk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zltespio.html


<!-- 参考信息 -->