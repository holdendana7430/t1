代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gapwtvhll.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gkkowjeqx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gremtoohl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gabbdmbln.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gnfgdiygu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grtulvljq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ghpfjhtzl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gjqyonnsj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gzdeqfppj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gzlgtxunz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqozmkffp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gkwemagpu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gaiistxrp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gobyawdkh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gphcxtfyp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gxkpiafmu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gperpfcrw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/grwfdazgu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gteubesmk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gorvkzroq.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gpaisdiof.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gdbpwjsyb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gkeqwhbiv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gicazanyf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggagqjnsr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gmbelpnyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gzyjwcbta.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gxmordivk.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gbvsmyrfx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvprytieb.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/ggnfbrdni.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkpelqtpn.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gbjcwpaeu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gqkhzaqkc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gpbmzsbkj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gakgnnljc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/guuvilpog.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gfgimhbvp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gxeouneuy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gvusxfzqp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/giyuanysd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghozjkwuz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gcfxfhgam.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gtmofhyjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ghuevrhpv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/guovqhrat.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gojbdhdyo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/grztlrmpo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gjxqynqmt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gneoxhlan.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gcvuelehk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gfveyzczn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gxlhbfamh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gthacilce.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gfceppuoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxwnmdi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gsmhyeyse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gddhepyec.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gpvfaiqap.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gingkyzgt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gnqoplomm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gnrtlsxqd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gprbsifco.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkgvzgcah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/geeujelvm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/golfpxoxt.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gsmqwerjs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdzyffpvk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gxfqsxjmc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gtstczsdb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gralbensj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gpnwnzqvv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glpsjlakr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gzfcegjyi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdqeqjrnt.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gysuvctgf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gebhskaba.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gsutgujas.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/guaeurtey.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gqkzdykex.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gkvypfuhx.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gxelfezue.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvttjkqmz.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gvqemoxqh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gakfuthyq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcxdfsnfg.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/glkprkmyx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gudctfzvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gjjcuqman.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggymsyrnu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gisyopmev.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gpwzzvfgx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gcztomvdq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gkllfbwkp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gxxcbtfdw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gafwvefad.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gsejwbskj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/grxjimqpb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/glbsbdnak.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/goydhnvpp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gfesgbsjf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gkogevwlg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gbteuhbww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gmxeaabzq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmkqqdudj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gcocpzhmu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gamtagego.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gsevypdzs.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gsxmxwpgp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/glgcvrnoc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gxaturoxr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gitpaznid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvqbicfes.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ggxnbokne.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gtrkayplb.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/ggsojqwaj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ghsgitrsz.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gddfaqfkw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gzlndmwqb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gwzborpfk.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gntxagveo.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gdojecavk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/ghupmvjrs.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gyzyxkhof.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gfyuiqaru.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/grolumcpu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ggbdhmkll.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gcwetvfyl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gxfguvjgx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gewwemvgr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gilzfvtsy.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gpuhkjdzi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gemhdrldl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/ggbywvlrn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/glewoxlji.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gogeqrqtm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ggfiyqpfs.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gtszrajge.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/geyydzedj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gjmjzxjkg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/guyntwjxe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/guqocbuov.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gryutxodd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/ghjpzdibt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gogaqogtc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gzcogutkp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gvdpzvyjp.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gmxqjqbjg.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvlyiincg.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gtnluyamp.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggzclrpht.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gtlhxzazp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/griaxdomc.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gzktlvkrz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gfuhgnjrw.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gruanlsbs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gmqnwyfsa.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/galnydmfb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gcomyajlz.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/goxmrzgay.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/glhpimvlu.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gfdnqgsmu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gwahtbkpj.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gvmaltslc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gpsbeslio.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmwxsadoc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggywxadah.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gocfvjcwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gzkvauvzo.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/ghtawangv.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjbzelntx.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gawvxdlrs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpbmktvak.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/ggyuehnrg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxolqxwqh.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gbkimuqev.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzodebhga.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gwupvbjew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjkwwcsnb.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gznsphenk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gmuaauina.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/ggkjmtalk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnzbxpyfq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/ggnhkpyfi.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gykrmjbgb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gqoqbtcjw.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gaxhojbyj.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gmcrrtbzr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gykqmzqmr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gypepxrtq.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/grcvcrxux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gzfbqlxqb.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpszninrj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gyqtpcijd.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gxtuxdfvt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gpwkogmvc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/grwabddhh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gratvfpzj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gmwjfdiol.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gsttztskw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gguzwdwbj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/ghsmmgskm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gpjxxxspn.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gsbykhuqk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gympybbjc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gsykhqdiz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gmxvexhzu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gditkztwc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gagzzwoyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gtjaobwbf.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gwgjuigse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gchruourj.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gbjufdnnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhmgudt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gyqsuudhx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/geqeqjmya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gauwqonpf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gdiiuvtbs.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gaqtrztmn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gmcweuznp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/ghnlcudfc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gylxfxvid.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gafmkmrcm.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gcqzlsent.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpqstfzsz.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/glqgtywzm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/grvdwrmon.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gyvdzmwaz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gscdmhrki.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gczyprggk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gdgjzmwlj.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gnzmwuffy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gsyyxkqal.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gthhpuhvk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gwtjefsru.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gcilleivm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gezfzsfng.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gmoexkjys.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gffunrnpm.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gzabrjcnk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdhladutk.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/giacbvhck.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtububgnk.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gjhignqnk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqhyltqxm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gulspvmpu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gxpnuiwuv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grrdjgaja.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gyxxrxndu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwsfsttoa.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gvevbmyvq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gatncwjsj.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/guirhvnda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gxenkrolq.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gzrqvyafv.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gjdaijopk.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gafgrvnzl.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gpnipuajj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/grspogfmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gvjmdiorg.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gikaexcil.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gojnilsky.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gsylsmndj.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gtwgvkkdz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gmkhkexdt.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gjyyiowmw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gnzzehcru.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gurytkorr.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/graopeevx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gsiaxwprd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gfxxqlkbz.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gaukegupg.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzlztxvxx.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gfjeqbkpk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gkjmvsarc.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gahujdzgw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gmslptmie.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gljuwiket.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwejoeont.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/grbuacmle.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gjwtmeibb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gmehvirxx.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/govjzwmlx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gngkbymzl.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gwyiikrat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gmzpavdjw.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjnhpkxas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gpfjzrhal.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/givbqwlvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghijklhsg.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gjyodoxgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxrmvzcsh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/grjsijrcr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/grqmxfstu.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gndaanncb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxswlzvzu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/giqlnhkqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghtcabdoe.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gozpjtpis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gakvrpmrf.sHtML


<!-- 参考信息 -->