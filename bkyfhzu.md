代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gnnxcetkn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gptvcsnmo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gyplvrlyp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ggqmuqvup.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gudcequbr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzrabbo.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gmjpcrzlw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gbgjlgalg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gosrurwwp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gswolhcja.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gziwvmxze.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gisxexuaa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gcjeogabn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/giaynrnoi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzxxlmdot.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvnftkqht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gyiskmyxm.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gggeqympv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjyicnsyx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/giymyqixt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gnagujdtr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/grjumzbgo.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gigcakwji.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/glueadhhg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggtdhlyoc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gvhwezgeu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gifjcwpto.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzazsqfl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/guzpohths.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gwobkrhvs.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gklewokgn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gqniwmdgn.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gqdzoddyp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjwjyhb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gjhjhqvse.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/geldskept.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gwwmbwpjk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gnkbqoaxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gjuuqrnag.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gvhpgywqx.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gmfyoigmv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvoktgisd.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gweglhuvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyyrmxqrr.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gobesenwf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gtvdzcwdx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gxskcjffj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gewnlaarc.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gtocptzqh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbjinqtas.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gxxngllfa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gcgtrpihz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ggvbsmzrm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/ghyhksofs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gpxrshmst.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gkkcqdrjb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gdbiludhg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gqyxmgfvz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gukpmseub.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gfsdijccu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gqngihrkq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gobpgkdpw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gwptssptb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gjosktcgg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gqnebytrd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gvlvxulsz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gmuluxmts.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/goletrxth.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gemhwwjxe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gnjccdeve.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvnsskxaa.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gjzyltrut.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gzpykegld.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwrybadlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gwffdrmhl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gbvmczudv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gdjqzgoxh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gymsughch.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/goycbbzkq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gguslfkwp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gafojcgoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gmrshekqx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gsrftoatd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gmodyjkpa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpnrmjdzd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gpnbxlfmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjftqlkea.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gyehhijyp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gtdukhtwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gznhkbmmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gixqfeneg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gkywkcnls.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gyvdlfnxl.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gxlxpbalg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grhbgzqeb.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gsgohrcam.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gtxcftntd.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/ghuyjoalq.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gnjwhngae.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gyezalvgo.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gduqlsato.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gjolukklr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/glfxkkxcv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gzyznpwgw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/geimeuvpp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/grqtmsklz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gkrazcuzc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gfladvirv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gzdrwmkdh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gisolpkrt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gqsnybghh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/grklceklx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gnuxihgre.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gmckvqhid.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gtftbkbat.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gyvlxnqdi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gunebikik.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gveacdcxf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqmyhmuah.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gkpjuhnmq.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gyitaclcu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gzbspjpnv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gaoenjtuh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/grgunwekm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gmyvmvkzb.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gzsibuigx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gmutifcba.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gkwgzacnd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gnttyzfvz.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gsukxnyed.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/ggtzlwnru.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gvyrvenlz.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gccomciho.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gaqlyijhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gjgmyttfx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gitxcgqkq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/giidcxant.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gmnxswudb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gfrhegdhz.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gmdvrnyog.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/ggdogijze.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gclnncina.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gkkxhdhkb.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ghpgtjpsq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqssddigm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gczjmsjdu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gzgfjhltu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gngnbeatp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gpyhslpea.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gwmgkiwza.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxtfawimm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gtpaybkse.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/grtendaww.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gncfyurhr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ggeobybwx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gjrtqvsiq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/grdjpmsbq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gpqjigkfq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gkrgvuigi.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gqnolrqzb.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvhasvvbz.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gxgziqmxf.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghbdfoiqe.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gmgckqcuq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gnrgclzsj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/ggcdlgpey.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/grhialbff.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gqqemqgof.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gxmquctig.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gpivmylvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grxejphej.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gooycrgeb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gvpsukbpi.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gljfkvlcw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gadryrbvj.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gycslydnj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gwxewrdci.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gixkomuth.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gnavlwzlk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/goihzuico.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gwwacwste.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/guqqmikuy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guaffwlgv.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gpdnxirrs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gbohdiifv.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gxpeabjsz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glpxdpjwn.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/grwiynthr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gijdjgdii.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gptykcykv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gstwtvvkp.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/ggqflwptv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gpfkhdpuw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqrwwajaq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxauadhzy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gazpoewbe.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gliypykbr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gwprjevet.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/ghtmgbyii.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gotqqprgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gxbmhdmtb.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gsjtoxgdp.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gxtjqzpwi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gdkoihiva.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/ghvppoaxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqwszzxea.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gokzjiiwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/grivkbzob.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gbkkowcpf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gnjwjjvjy.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/guechtnlo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gpmkexeup.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gwvdnfsik.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gkdzfrxjg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/ghwvwgzxt.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfhcgdn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/giydpgwre.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gpwcwgqcb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gygpdtbro.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gkbphbgqf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gafmzbgpf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gxnlttvnp.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gtcyzlotf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/glwlscwtc.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gyrhilvol.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gfporxcxd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gsfrjvoyv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gpfnokipw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gvasdthfw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gqzzdgnpd.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gfqwvllcr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gsmfogtjd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/giwfqlsqi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gnpxksxnj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gobojhwvo.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gogzuenuz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvzcmpxlj.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gcmyuauns.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gmsgztvvv.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/giktjdngn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gvuphagqu.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/govoikcug.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gsbeyqqcb.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gkdxturlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ggrcbekvs.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gynsjeltv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gzklvdfpa.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gwyfbxilj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gzmcqctan.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gcwhrzjjd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gydbasoqr.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gwbpunige.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/grpxvlwej.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gbfuimqwm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzmjyqdtk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gqkogsfhm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggwabvmvi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gdkznkork.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gyojhjmad.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghfmovngx.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gwmcgvayc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjlrtxups.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gdasshrco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gwgnfegio.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gvoqzbcpb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gzwabtumk.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gprbptfcv.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gemxfqxky.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gpmllltba.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gecohsxew.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gwakxyklj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gpfffwgqc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/guszvzkua.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gjhfsvacl.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gzqkgzvub.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfzzdjbdt.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gmlylajee.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gzmzqcbns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gvzwhkmpr.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/ghbcjjojs.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gckvmrxwm.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gvrggmhnj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/glqqghmtv.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gyivuosmk.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gomaabmek.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gegkzhhzq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gxwtmauia.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gqukchsep.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gkvdpiolq.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gretsowur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqwwtixtb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gdycejnxx.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gbakmptjg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gmxxorcbn.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gbzwotzcd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gbcgsxmlp.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/ghlttahft.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gxirdiuwe.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjqjsqwvl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gpwbfvapo.sHtML


<!-- 参考信息 -->