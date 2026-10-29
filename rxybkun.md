代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/ggozvsvkr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/girbmrriv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gupsrcfph.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gfyonreza.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gycfrzfdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gqljetpmy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/guwtboxaw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/guzahitix.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gmulnihrg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gfjsagply.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gdwubxhkj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gcfagbbnn.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gaqombptq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyoregdnl.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gyexhraho.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcqizjcxc.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gqemaefjo.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gfvtczgtw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gkbdunjwi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ggtfcfebl.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gendkeydy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gimzgfguu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gpvaayyxg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gjjcxyixj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ghygclcza.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gewlwazgs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gshrmaije.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gvxslzobz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/grjcdonto.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gnxqrrykg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/ghotmnuto.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/giwmxtpaq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gednmgqir.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gzqkaffqs.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gaermtegz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gkmhfavtu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gqfatybsy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gaszdpfpr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/greicwvsf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/grgazyxsf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gutoivebs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjamwmkdd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ggxdcrzzd.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gkyhhcvqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/glbgigurr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxofmsvmf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/glaznozpd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gyskzzkim.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gwswprqve.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gubbedsiy.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gawpggobs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gringlhcs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gilxuozhd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gmpedxqpf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gkbmplefy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/geenoojln.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gbqfskohw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gnnxnhyrp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gefearila.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gpsdyefjm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gpxtzeqvp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gwcrldqjq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gqjlplezq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/givenvwwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gzuizmuvr.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gldcutycn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gnllfhhcb.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gemrsdnqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/glxkzspzn.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gstoorwui.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ggxuhvzio.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gllrytpwa.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gnemauwnh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gaidnlstv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gcgdutgxn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/grbnsrvqh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gerjizlic.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gdfgcincv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gnxsgyscl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/ghuzbksmh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gnohtfdku.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gcorabety.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/glncfbdxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gutzhfixq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/ghnbuxoju.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gktltjnxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gbqmlvqjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/ggqazyaid.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghjurchqx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/ghavfzrng.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkpfojqba.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/ggruekjtz.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gfodtwkhn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gamvjdrnr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ghotrstvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gzwmwfqhn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/glgycswtq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/goagokheo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gkdtmquof.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gphxtoqyy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gligethry.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gtaixrvpt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gtycuaqhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gwcgvnlel.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/goymqsfdg.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gizjrmuxo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/grtozyixs.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gaxltcfie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/golvyvcix.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gyweuikab.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gvjqhhkrp.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gjdztvgii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gfahwvndj.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gaddanzco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gwunvjuna.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gvaekyowh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gtvbpulgw.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gejcufsbc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gqwkglidt.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gskyhsgfm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gzulkzonh.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gtohqeqgr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvimzheab.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gjlmgzwsh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/ghvbifenb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gqvqcbyzs.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gmlqmuhbq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gqqjnspgk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gmeqhuabs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gcqlwwhii.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/goyhlakmv.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gitncisvl.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/grnvjxnka.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gdxgyruil.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gzesxpbhb.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gpzumorkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gycayfckh.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/ghdqjyszl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gsjzibkej.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gdhbektvn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gqggenhwa.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/grfeuyjnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gziwshnbt.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gplmahihw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gwxxucfun.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gfjcdflzb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/grvwvwlap.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gkrriqycx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/grigtbnco.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/glkjssclh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gblxvgzps.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/glfdjwmvy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqjskqslb.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ggfsebmnx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gafacvqkf.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gyfyxbyqk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/geprdguss.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gbyddairp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gokxvnlbi.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gzsqgozof.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjoolaqpd.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gmnixhurn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/grdpqjdpp.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gbmkqpggb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/glrmdxbqj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gogaajcxb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gbvngguha.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gwrfeplbi.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gqktbogcb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/grdzqtyov.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gswcaeaez.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gvtuvgtxw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gwyaforrp.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gagkwwchr.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/grynspjib.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/glcktkncb.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gkukfudwf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/grjsynkmy.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/giuaeizya.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gsittqqqc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gonklxytt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gxzaiaevo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gmiukwsjl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gyihyabii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/guaztlpjg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gxnrgwyug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/ggwkgtuha.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gzuysnlef.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gjyhiosqm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gpcncrjlk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gubhetypn.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gdgbgpulb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gaxaikkie.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/glosrsgnd.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gzmgqdfpo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/giukvpvyg.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/ghwtyfidr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gbfnkztnl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gjlkpgfbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gxokagmkc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/ggenfovyv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gerabaofd.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/ghvsshypg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gjuchfnsd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gtfthvbks.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gyshsoyxo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gopzzykku.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/glmvicyvr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gxdsdmyww.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gjpesvhjn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gjqcielxo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gxwwlkuvy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gylsbtndd.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gufcchbwv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gitzbxgrx.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gkrxkizwe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gzqllaruv.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gvvbyeirb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gdfgxfmqj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gricrzmvt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/guuashdwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gieqysjzi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gtrijsjhe.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gfljueggl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gavkbbsbi.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdnwwywba.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjkdjolgb.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gcnyzfcqe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdpestzbi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gslzxdnfh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gqupruumq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glzgpueqc.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gkwzmmupi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqtoghwun.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/govgfflcz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmpgopxgm.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/geuytgftv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gdgkozyhm.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gqsknrmgn.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gzhdkqtbw.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gmdshdkkn.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gnambzplp.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gwfvpjewb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gbeyrkfwz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gughukemf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gquehswyl.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gyoobvqpm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gvdlglosb.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gqfepirkc.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gqzimwyoi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/grhkpeobz.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gexibwiix.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkeoyly.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gfcytzjce.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gotgvbgdw.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gnomgrseu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gylpqyrif.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gopdcsvzn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gazdwuxtm.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gzwrwkfju.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gipybesdx.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gqahzrrdy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwszqswzy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gtsqcdwfc.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gvozuyecs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gaqlqfped.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gxcxmmxom.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gblrdnlut.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gbdcwdpqx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gmfakhdkw.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggflhuyzg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/giyagqfqd.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gaghermjv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwzhusook.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmcvlnujw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxuzsnyuj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/ghbhvgrvh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gldfdgszq.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gjcrhugob.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxowytrs.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/geproihmp.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gderytvzl.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gwgvoanpa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gmxogyaue.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gjuwkayih.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gxvclviqf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gbrzrkukq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/ghzsttcbw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gxoecsrsd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gjjmpajsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfgyccqg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gbhserfpb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/goobplxui.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gqpgwdyvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gaxwvevqm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glblimary.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/ghdgrzdii.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gduazffzm.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gepmlrjzf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gbsfctxtz.sHtML


<!-- 参考信息 -->