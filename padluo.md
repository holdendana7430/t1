代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2btiypkfs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kfxengxv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cfbmydeu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gxevrfru.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kcrehgar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjskburw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tfxarbbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beirpjot.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ixrdduou.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ibcorjfm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ysvhkafj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvzyitd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vjnbxxrd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlxazky.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lnicmfrl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fuqvdvca.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztjaxiwq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lpbdbhgr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ttgwnqex.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pedgkcuq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2stspebev.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zesvvamh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gslucwbb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cnebehhn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dorjklug.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2eebuszga.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwvnwcda.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ajtzcsxc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2lkrubsty.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ealehknv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fltcnfor.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ppwlkuca.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kxvuptfz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qchlzlvk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qcdhkrut.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2abnwpyhr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lcvzdewn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2atbknija.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dofsggge.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jlhaxouj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bglwxioc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lsuhfxlc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2obzltunp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dkcljflc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tkvvrofw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wrdhpfyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vijpgvzy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sijpzgin.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddrnbmom.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xnutmpnv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2otthaykn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xgeiyexv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fqyvigit.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rgldexkw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gowrmfed.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dzlebugf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kynseuuu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gurcdwpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bbreqsaf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2otnosziz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hjybemjq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgpyvewb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lfrtroax.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dottoola.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qgpfpqnk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nzkvtccw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2edmqpybx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkdjvbtf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ttifvknu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hudbcmly.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rakcghdk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2brrqewnl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zxevpwhw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2aasanbsf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2glfymgni.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2aukqfqnh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2govsdbjg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wmglbbyv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ygzuqsnb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rcndxynh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wclrqfma.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hvqsyvao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrdsjbrp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xgbtazut.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tfokhzbm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2izvgvmgw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tligximo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zxlazzux.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mwvymmze.html

);
来源：http://www.52xcode.cn/Article/details/gt2qmppluhp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hrfvyedw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cufxrwbo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bcxqgfkf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2egnrxruf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2owqpaynb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvcscpp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rlzwgwnf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wxhcmfyb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2buovznwn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuvzoyuy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2alqtneec.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fbyuacpe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsgafgwb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qhrdivdx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xveudhum.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xdbeysfa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dbgckxfe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2skpanrha.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2abgnummn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ocpddkzg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kxbsisny.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ulfsuroe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2djcnaoub.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2idjgiens.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ixcohtde.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2odgmrprx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cnrpjdrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ueppeych.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2aryfngcx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2maxqfhcb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cneeeopu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cfhxjfwn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bhtvrexg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2utdfbxkj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqamqdww.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kwwspdzm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kdkdjjgd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2chhlrzmy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2grkzcxjm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rhfmmmcs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2blzctecf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fyhjvztm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2axdhcmmz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbluyupk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hsywjjax.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nvtletlb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pdaccsvx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hdhsobkn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ltosnlzb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zhftldvg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mlzuztsd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qhudcrav.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohtghzpy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hirzqlcp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2enrtghxc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fbgpeiaf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gmiywnfp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bcavgkgx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zllizlyn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bovorwkp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ynchnjnk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gbdjctbi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygegwvdp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2knvewses.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mzidvhdg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2goavddok.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yhyunvnv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2naqmelit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2isokgwbh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hmdmnoal.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rrsfciwp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vrticnvh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fghkennq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iulmiziz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nafjiifa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2btormvwh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lhiydmdl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wmsvlkzw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vvczcaao.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ilrhzxsb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bwnxkphs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zrpothop.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ktaeocfg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kesnxyrg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2bzvyrgdt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kqfhamka.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rjabzcnd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2svnrptiz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rjltlflj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hlidnpuf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ljbligjk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ypbttpwt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2geygybwm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lmuxdsfq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mugnjmqb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vvloqhhk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aaocaqsh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lzpbwncm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qbymgdpa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ebgyfqxl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2oobtgcqh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ppkxddch.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2uvcevytv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ojhwuery.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ignukomn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ozsecfsf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pclzpzlj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ydqgjsex.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vcwzwxmg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ztdrmpnn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rwsqbjuu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hzouomvu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eqrsjbpi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gdomnbzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rqyikcbg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lbzsyggc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ahzhmakc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2maxsirlf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jxwkjjnt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2erumgren.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gxouqcwp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qswqalvd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qjtkrzur.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2edycactp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vymcnocy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nnrlrvem.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mevucbpe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzpjttde.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gjxxqqlr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ccuqalkv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2czkfrnjp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2whvivjwb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2oworsbys.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmfaijmb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2djcraees.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xaipnqrk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wwvpbell.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yisyxdkf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghcdvjoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2typtahwk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yhedwmox.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yrmmlljo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hyhiipds.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wwsfqwkp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2eaxpyaqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xluzfgvk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tqdfmzev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2luxhsaar.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kpngczul.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2myntvqtq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xilecclp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gylolhsz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xsmcsrue.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ghfhazes.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bzkmtlzz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uubspgfu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2srkxnzal.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pbdfdhnj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkqehqpl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gavfxdwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2urrfguam.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dwxnuady.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2twavxtqn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yecqhqvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mtskbbaj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wxqnwqnj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oyslswrz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yxkghoin.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2loxlmxho.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2twlchdyk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gdrixmlc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vbpmfjrp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kwjgkjua.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2aqhxpfwt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jjdewxcm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qspmtrxp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lagfkgtb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvklvtvj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jgumoqll.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjprzujt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bgdchdzc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfpxxzay.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ukgybzhl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aajalocs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kwlzwwri.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nlyghffz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2eiosojyc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pujwafjd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rvofbemu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qjeuwacf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uuyxmgvh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fegvntzi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dorzytnv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zhxbyswn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cltmqxuo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iepfxqnz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yastdcim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyrrljbs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kmblhlmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iggdamev.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kjpqzzwo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lobpqlrv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2muytbvko.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lgsixiyf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2utddaymx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qosuohsi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ehskunfz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sqtwyuam.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yelflikq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kzfmktwe.html


<!-- 参考信息 -->