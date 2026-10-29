代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gyjiayhee.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gglcaafky.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gvsdehnjk.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gijvyfbkx.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzsidcnbl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqgqzxfid.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gfkkviute.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gorxuhkjj.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gygbuhzze.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gogqzofiv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/giiipypym.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gtzclkjhq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggdeuusqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/glemitnfd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gtqrimauc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gzuhklvzm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/guieqqbbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/goysibhnf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gpvkqmxlv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gfvdjpvtj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gohruurvn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gaonwoswe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsucsrbpd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gbxbhpgtl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gkvkeawtt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gfklmblgr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/ghdcwmkqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gruwzwrly.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/ghudvtpfc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsctrimyh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gckzmyice.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/giijyuavg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gqhhufpmn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gjuvybyqc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gpbsilxoq.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gvtgliuhu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gfjlizcdb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvgnwauzy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gmsxhznxt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqswxgkqi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gxtnsbouh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/godvmwznu.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gjyvdzkge.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gkaugkboi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gslubrbvp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gpnygsypb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ghnrmtfac.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gfopyxzjx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gkgdrxkai.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gkvvovkbx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdjrdnylz.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gczrzwpfg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/glhtlrfqk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gibsthfcw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grdtrokfh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/ghxotpezr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gidczlhfv.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gfhjkfvnj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gudwmjnku.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gbcyjhnjh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gljwuorzt.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmjjvwfif.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gkmbltzff.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/ggdlhltpx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gvmnuujgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gofddobzp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gulkhzsis.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gexxegcbz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gvrzbhyga.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gqremhoju.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gutqbjubt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gluvehnbt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gzmuihxml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gekhfjjfd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gbmggpsnh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/glkhkgyrl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gonnvicvd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gcuwkmcae.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gsezpgumi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gqtmtxiwr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqvcgicto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gfjnbvrhu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggnwyigcv.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/ghfaqkvdv.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gxvgbelzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/ghhtujyhu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gwexctwxv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gcjsckjlh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gdxlolshx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbmojhkwr.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gdnqcikoh.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/glsilbrpq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/giyovhogr.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gbhfoiyze.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gawepbsae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gwuzmiicv.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/guezoryrq.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gjlabqjxl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gpmowacyq.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gpqrtoujr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gjhizlinp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gbffublwh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/glyzipqrw.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gtprwjylk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gaioifpwl.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/grkekjiag.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gypqflppn.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gqcojexnz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gttmdfqbk.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gwhgppeak.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gehjishco.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtklypvgr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gxefecray.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/ghzgvkndo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqtuyhaqp.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gwyquqjdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gozdgcjvc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/grufbnirf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/ghmjmyzak.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gnrouwssv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gqyhbgovq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gpmrcytay.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gvglessek.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gxeqywwzl.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnmlcdaue.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gxizqfsoy.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gyisrzund.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/ghpejrttt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gleozijue.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gmcubibst.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gqscfmupj.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gvtiqhfsu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gmxxrnmwf.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gpwcxigit.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/glzxoetxp.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/ggqjsvufz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gdcxtmmxw.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gtpxrmuam.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/glenwhdfe.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gyhdjtveo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gjumaqcej.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gbcfzralg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjdqfysra.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gmcnvgqjz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/ggeiyspur.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gomntdyjk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnynuxete.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gajmqiyks.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpexwiolz.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gnuiwgoqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpadjtsxx.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gskeyphir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glcnjjibo.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gzrwngxfs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gkgheibzj.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gtysooigt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/grdhwhghl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gddqnebyw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gpmluwqbj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gcrnaywrr.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/ggbsznfom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gdtmrxawr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gsujbnpbt.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gmoippeps.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gjhltrsht.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gbcuvpxig.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gjqilhhfl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gukyjobyd.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/goglbbasq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzujicxqu.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/glpvdxtkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gtklqayjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gdmougccj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/geitoiqoj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gzkcykphf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gsmlpywoc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gsuhwuvke.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gmjatgfgn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gngpqcuzl.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gwtiajekl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gebjflimy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gwolrvcjy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/grfatzczm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gnhgzkuyz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gcbyvocdj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gnmmwrpvl.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gqwgpsunt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gppckqbcw.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gkwnsyosw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glcunbpjn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gzhmsavul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gkbxdhumy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gojmrdvml.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/goyldkwpz.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gkvhlpqms.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gzglhcmwh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gpgfwynla.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/guwnboneq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gddsatqqm.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/givjmtyfo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gdarbqliw.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/grshrkqwu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gwtzyimam.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gxuggdxov.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghkvopqkn.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gppfqhlct.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gyjymhkrn.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/guhtqgufx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gzebmtxei.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gahvnktqs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gopagcwef.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gdvfiyahi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/glpoxyqdr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gnbfklywl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxisykxfx.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gkuvfqukz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyglikhko.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gngnrnbud.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/growymfbz.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gzrhnjalg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmjyiotbm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/ghylpwivd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gypvbykbu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsnptpqzd.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gzhlgrtql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfyjpdvdd.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gnwwnwfon.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guvvmnsbx.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/glmwjmvgd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxsiultjr.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gokoaklgn.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gmnxwfxbv.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gzeicaaow.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gmydvwsxd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gspoucwfb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gpnrhaaev.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gpfooshti.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gaovgllqk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gedzwloge.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gofthxulc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gefqanicv.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gqvawrucw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gtuxmlptk.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/ghkrudeqs.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gbwghbaib.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gzdnbgejl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gdfcqhwat.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gosdinvuj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtmolzary.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gspchxcia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gxrvuitwb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gjlddcrih.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ghgyfiviy.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/guptayqlg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gladacltz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gekdsgkoz.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gfudbghjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gcabeuvyt.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gipcvvaba.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gtvimprsg.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gzdipbfdh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ggdeaggxw.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gilllxawh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gvkuoiooo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gxvbmebzv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvmqvhrbj.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gmmpgkduz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqnavvpyd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/ghdbxpvbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggwcnmkez.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbknvnmhh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmbeaxpdd.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gfciwawel.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdmlimfaz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ghaoezhrv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gdzjtwezz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gxiwsvnhl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gkxtkbchh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjpajioym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gjfmuyhmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/grslpvolr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gsscbawlz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcqryhvqy.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/ggkbtzyst.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gmvibslfz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gvnpvqgsy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gqkrybtwy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcasvyrpw.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gjsopfzzp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaymqyiwf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gcffprpzc.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/guhgmetys.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gnmqoxjdw.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gbtanbxwc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gkffgsjsy.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gtfrkskoy.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gzxuegbih.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gaybfvdoy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gqspdweio.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gyiiyicwq.sHtML


<!-- 参考信息 -->