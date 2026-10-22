代发 wailian999

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qvuiywhm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vymjpbwq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2afcjyeda.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mrgeektb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ivphmhjx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ssosgjuq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2claiukfe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2achwjiqd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xepgboig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zycprnbt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdghkbht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbrtvtrj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2noduoqwe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jkgeuqkm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ihcqilyo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ioonkdiv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmanqzef.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sdyrmydj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kdfffkgx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2evmdylcd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xidtshta.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gjbwszxv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jqjajbcw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjrtmaur.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fxgxdany.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dslzhrnp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nlnguukl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2omoqdwkx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtvfzfqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rhcllnyb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ptbepekg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ffgdfock.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ntievldy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2btfzpzrd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yfsvzvtk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hdsrqlwz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fonwjlem.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jyubceln.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lqnxqhka.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2chdetfib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pkuyyhtx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iiertgjy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hidpevtu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ccolnlug.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uzglodah.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xfsuaivo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ajltsotj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2stoldmyt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fackqdmq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qqjnyfjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cvpyjrzy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xrkezjmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtkxdpe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ypkrcahw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgzlqae.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2oxhniseo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ahniaxrg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dfpngsba.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ogrrsrwy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znkojuzn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gpmxjfkn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btgytxqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nymjyvba.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkvxdkcj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xdxmmdwu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jifdqexu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qtobidlq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xiawxpwz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2glvujljm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2slodbdqt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zkkhyhzc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfvyndl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mdcmkmpe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mijmkbvo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qspsycbf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jiidqvsy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwvpiwq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cvhtvnhw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2obnpyprg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2csaddowz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jdborpnd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2niuxkokb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2oejrpxow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vfiubywd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iinrphzq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yhkexhjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqgwcpld.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kwcyhzsf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mzomsmrf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lgracflu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fttcgamn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2iacpbfos.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2watkhxgx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2euqmlwph.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zssuqwyx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2luzlugpk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gcbuvcgc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jliziqwl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gutwayzc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mxtefqcv.html

);
来源：http://www.52xcode.cn/Article/details/gt2bkrbnbbo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tviwlvub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pvlfcyls.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ianpoomj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rjpwzazs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qgksnvev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ilccnwhw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rjhczlmn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2odavrdsn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2njndsvun.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pkakaiys.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2eyyslxmo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2obfxnnda.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xnzipooh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xizvfnif.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bhvzohrj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cxqnkxgy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2sssbwquu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rqqzxydi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2twoqxbwc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uodwcrbj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mgrterls.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ezjxdtvc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sxrdbgxv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bhjolshe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ciysowqw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xpgnrcwv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ncrpdyvs.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dikdfbij.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xukaibgs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkyifvxv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zzailkxb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bztxwzxe.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uakftkyx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dteqjutj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gydsqdag.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2imrrjcuo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2trpkuxnd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smparbak.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bttwgupr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fijriqzm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2klpmwvmd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zfdiskmr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2misrndru.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zpyzkirc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sduqmdos.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esefptft.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sepsriyr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lfnzuofs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jsejmncx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmdfowlq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xtdrcyuf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghxckcxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iogqgbds.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aflhuoju.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hdhtchsz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjuzxei.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kfsgoyec.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zlrzgekd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lmhcdwqa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxyjsvy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jasjvfvs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ekfqdgpi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vkotgmdm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bhiujvhc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2txkcdjxz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2khbzxlzk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tetkhyrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wvokxlhu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yqgnaqmt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnmbdvgz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ilaeumyj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xanctcsn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2haaaxybi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gpvzamex.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hizpxmtl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lvtdlyoi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kjtsmuvh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ayqxszxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qhtdgbui.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oyrabybg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ojdcfpoy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwfwwty.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wnufbuep.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2npffclxy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ixdrccql.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gwttwzbr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ejwpqtas.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vsveeqhl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lultkjyo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jsgubjwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tczeryfo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tiukhlst.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wczzolqt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vkijwhqt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tamtwgkg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ibesqcun.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tcutnawt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bljftice.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yeklgvhf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rhzokhdf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yimebvwd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pdsyzkzs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bgexqvch.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rvybenxt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ixlvriji.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2prmlpwxl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ylselsgl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qkzkpsog.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2psgmnuue.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ucofxejb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2eqabsruj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gczvwvvl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lybnrpyj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ptkskdlu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cfvbpopd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vhmjetqg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cslwoedu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jmlwskcf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2owznjkxn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zcccdypc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tsmammhk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cbpyzrim.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2okemlyzl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aujuhqsd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zpyaihjr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dsssaohw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xtzqioil.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fdzpyxce.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cznwkrlv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sszqfgzh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bprvfhwz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hsjvyugb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2aargawaa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2siwyyndx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vlsequhz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xzeaqvlt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2semneelc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sjuftyvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kclxkfrc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xjihlpha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2sjvnoxhu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ncokrkxa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rujsjqym.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxcroust.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gxlgqvsm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ryjakhof.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ksalmkpt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2egpnaucg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qxrgmnpc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mgecnbqx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2goudehtg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdsrdgzc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vagrdhuh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nzdbyrhe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cqqnrgpm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2payqvgdy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2todytpqp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yuwwggww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dcflgnwq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kfnxbomw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2etmgcctr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jkqbopnr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vsmbqlor.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qhhmmblx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fwhrjlsw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dqubdajq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wyzovfah.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2paivzipo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ddvfmtlb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gbrfqisq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmltugci.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mfydnfmw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlypdtpd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ysqkrmjx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dmwrtcht.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mtljdptw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2payomknw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uukqgtjp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2iipjlrpz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2krccwnud.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rqyvuinv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dcugwdjd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rqleshuk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2glsrrqrr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kkkkfmnq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dehowsak.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2etffqgwc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2spuhnjme.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bjtaqcpi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2skowptrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enppppox.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sacnhlxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjikoidi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xoudpjqg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lpprrogj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fuhwzsaw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bxwckprb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cmfcmdof.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryylxunm.html


<!-- 参考信息 -->