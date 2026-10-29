代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gsqesbpps.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtpakdvdj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gcpqsgffu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnblmcmve.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gfmdkixtv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvnvtbcpz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/guhfuavqi.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gbjpvrlbs.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/ghimckpfc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghngdrzgw.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/grbjsjxxt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmpelogxe.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gppioytxr.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gmrkkwich.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcosqftkf.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkmigvbuk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gcjzhgane.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gpgmcgufp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gfzdsglew.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gwvvhncwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gumsnrhfu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gravcvrqr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gdamjvici.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gxvwzbsjq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnqmqrwyw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gqxctltod.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/giimdheyv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gdrsgqvja.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gnunrakaq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/ggdwrqohf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gnkqppnoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gmjrnbaoa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gzqgsaqna.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkkhrttcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gxqiyjepu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gggdsuiiy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/ggdtwwgpk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gbdfnvslh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/ggeohaizm.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gvhzixpyt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gpteobunr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gwiblgikc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gpoxxfpjm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/guhdzqzmi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gnutxhqqo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gctccjflm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gqavktfic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gawmtjsqz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gpclyhwle.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/ghvzvpukk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gpyuplvbf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gqcuejncu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gonlbwzbu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gnlankjko.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/geuathixt.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gqssfhsby.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gkkwvusju.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gshppvkti.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gausqesns.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gkdeqonoi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/goinxvxkq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gjdvzwtxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gobazbupa.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gxcgfhqun.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gvhavqtrf.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ggchpmtby.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/giwnwbxmj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/ghlniuypw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gxwtlgbif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnkepjufu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gwkorhiky.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsgmkrqwa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gihypjpke.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gaafvvila.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gemvmujbz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gavrsbrjr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gqxfnerno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqxgcvpdi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gxnfypzan.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gmznmcnwp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gbwxwumyj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gvtxkwqsp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gksjqypzw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gvcvcqglr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvxyxeija.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/goqpzurqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gduxuudwg.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gtapizslo.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gcpiawhrd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/ggtnckifd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gyjyizwii.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gbekholas.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gogndhont.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqlqqzneo.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gspzyspae.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gxcyajubh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ghnwhjlvw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gpdpkjrri.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gdrrjejcz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/guseoxbgi.sHtML

);
来源：http://3g.hesvh.cn/Article/details/goyoczkqt.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gsurxyafv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gfamtqoii.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gmhzerypv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gllfzqich.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gzgeejowr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gwjdkjtgm.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gapofubyf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gkbvuzght.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghjemdccy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gxbfiudxx.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gdhlnwquz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbyykynwv.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gcjtnzacc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gocijlstd.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/ghfrjoiqt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvsaafopm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gryaexwlk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvftgqogb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gmjmvlwnb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gsdcbziae.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/ggoqbdwaz.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/geiaydvrj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gycprbeqv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/guqbqrmbv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gjrbbgiqn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gevtasddt.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gmvimocsj.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glcghreds.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gsclocvqu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpyumvbxq.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gkxnizuur.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/ghfmestoz.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gzbwhntzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ghnikqevc.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gcbljqatl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gdfyquyai.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gdvqurlyn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/grgyeccgi.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gsroqxxys.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/glnaexmlh.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gyvbkvblz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gfxrdugug.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gohdnwekg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gmwbjemwq.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gbvrcbwzk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkhfyikmc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gtnnudigg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/glfxeoulu.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gqhucfzrm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqdxdkopn.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gkvzfhskz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gocxztqtb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/goyrlbhoh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grvxucity.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gyfllrfff.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkoohaqcc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gpqjsqjxh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxqlikiys.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gayepxrwp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gnczhjfst.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gurfgfpsb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glhmmypnu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gzegwrtif.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gudjrwynv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/ggkssywfu.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxuhuhdhl.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gajiqxupu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gcdgrnndb.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gxufngbti.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/glsswtdvc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/guijeykny.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/giccghmby.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gkinpaqcz.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gqpsfyeyv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gkkbcvtlr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/grbqyoffu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjxfcflgw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/ggnvqsinc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gzllpgipx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfflejfu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gmdxqecjm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gvzbwgvov.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gxjddvscj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gulgzcxrw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gcwnuwcja.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gcwiakrre.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gxlpgmrmn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gspxehkwm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/goomwusve.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gfevanayn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gpjgqoqvt.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/guaaywvrc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gxeytnrkt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gyapwfyzz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gdmczhcuv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gjmnqojjx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpahtwiof.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gfarcnryt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gmiownprl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gaopexlss.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gtyxxavij.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gmwegdeyq.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gizqmvptt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gxpjrtalm.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/glhdcuspo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gdnjqsczt.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gspshxhzh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/ghdmkceei.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/ghqgyrnlc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gveixyups.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/grolqanzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gsohildze.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/ggzcqgtbs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gdssgmyit.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gkzsbnvkd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gdhurldfd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gcngzbcpr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gnmpxykmr.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gufsflujr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giholwffx.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gszbnhqeq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbsufzomr.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gehffmcdf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxkpgqxdk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gqobgvjut.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gjcdhrifz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkwffyvgp.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gzsizftmu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdhatvrvx.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/grosftblr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gpfxiecsl.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/geabunvif.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gcxiqnkyu.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gflflgygd.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gqurwzuue.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gybqewugi.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gsualesgb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gpguhlzov.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gfflzcifd.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gazjvapss.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gqgcbmyjz.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gznvpadng.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/ghmqkkvyz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gybvpukbb.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gnqqcnaql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gazezlcqn.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gogqdzdvh.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gdworloia.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gdvhrnbpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gmyfywtgx.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gapjappra.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/geowuynzl.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gcgupgact.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gxurrekdf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gvazxdvdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/giyczzzsl.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gncamvtts.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbojcgkgv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gddzmsgvv.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gtswnmxfz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gdbmxxnbx.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gooframvw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gpsuemvfy.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gzmkarlol.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gvzodrkwk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ggculkbzo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gkaenjowt.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gdkzulnzl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/grkwbzmgh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gachqbsbd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfiaychtj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/ghsjljuna.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzlpqfqfc.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxnmsexjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glezreyto.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gnsrgzrgo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbqdaucvv.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gymuzvpgd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gpvtplkgn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gqvttjjya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gghuhicoy.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzpwpdvfm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gmvwsuepe.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gxitteitc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gonvkyvpm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyyheuvsl.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gehytcrvy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfynler.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/glyxwcynq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/ghoioyybm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcyuhjxln.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gnjjjwkwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gblruevoz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gdgpoutkl.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gzntopzwk.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/grikcmvih.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glbythouc.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gozselzym.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/grwgxqeha.sHtML


<!-- 参考信息 -->