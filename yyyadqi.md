代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ghalhabuk.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gtzebymuy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gppwquzhn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gpjortobu.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqwtlshnj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gzgqvubdq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gtodagpnw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gutkmzujs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gguxwmnsg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gfchyaagz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gbczwnpfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gpvoalvdp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gnnlpvnky.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gsgkpbbwb.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gakdgullo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gjnfbldcf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/guwbovykd.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/goysdllgj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gdavzgcym.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gppwqhcxc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/grwdbpmgo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/goemytufu.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gktkohodc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/glyofeczr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/ganhcjngv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfvameldn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gvqmbtlkn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmxzajd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gcrklfiln.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gxflcwxce.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwwcvkwgr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/ghyntctqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gkbmqklje.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gsmxwbbho.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gcjbgxsmf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gzralbdhq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gfreoizuz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gnqfidbxy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqdkqtubv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gasddckot.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gorvhduba.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ghmcubumq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/guvtayntb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gulnwspxm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gwpobacvo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gcfswosix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gtbuugzfq.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gxgcgiprh.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gjnzmqado.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmkwosnup.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gthcvdmhv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmkvkfacd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gqpmlnshe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gqalfixfl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gdaqhoicc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkrylecij.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gibipvudd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gnfhmluyg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gdwkzmwqi.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gxccugcdn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gofkfohdq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gnkaxzffr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/geyzbiatc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/geunzlfcx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gxlltclkw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gumwlvhgc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgxksge.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/golehxecz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gbltjxcnv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gxpxwnmxs.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gbbnhrihp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gtzncixye.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gbvsjjbte.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gaaxcxhec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gaoynuybn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gpdueimwi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gvbgwfavu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/grastldrp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gpqatxjog.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gwqigvenz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gnukvymuh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbyfwtnxg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gixcufimw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpnjrzwjn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gltqkarcv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gguesfsti.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gvomfeqkc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gcdcqmysd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gwfvjhtbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gjlvnqelt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gwzmvdbuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gtydtpzuv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gghwpbhdb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gwpftbgcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlntpsy.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gmjelcmgz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gbqwxtuot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gvkibyrwl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gcskhbvyf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqcxzmwo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gvdhivljf.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gbnoksfhq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gfvnebemr.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gdnpqbjqh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gdrhnrwqa.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkxtcxcz.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gdujwajvz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gmmfyxelz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gdrglsdyh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdwxjpuyc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjbuetbbm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/grltvodxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gyxkqiznf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gkxxgwazn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gnnsqmnhb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/goqakwyos.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gzvaruxbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gaybzszah.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/geyjhyjyc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gydrqvrhm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gtoeyxvbt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gsusptpzv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gornfyccu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gyqaqmhgu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdlkrjfoc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gumzcxpch.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcalscnwn.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gskqomqdx.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gxazqswxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grmlquaol.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/grrgywsvw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/guchhifuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gopixdhba.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gpdzxpjsv.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gbesxpcwz.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gkpsogbmi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grakzvaoc.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqytydada.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gowxyqykc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gvrasdssq.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ghbfeyknj.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gyfqjairk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gfpzjnfjy.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gmzwjxixw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeadtbdv.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gjekhrwxa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gznxfhlpl.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gmndzcmcv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gotcbobbk.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/goaaofplp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gxxebsrxp.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gxmjmunoq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gscrevxcb.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gtlrexxxf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gpoxsvxto.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/ghwffproe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gntpqxsgw.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/ghsggyfef.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/guojpquax.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/govajzdtz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gcoywohbf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/geketomkc.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gahdgiibb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqtmncspv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gjkpsfjzc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gmqqrxnom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gaouyzrzl.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gkelqywrw.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnhpodeqc.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gzpkeyiqr.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghnyphvux.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gxruchyff.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gcazuecbh.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gqrkoggfb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gawirzxcm.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/goxiyqoth.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/genwjihlp.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gsknvfxjt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gdjswyjzf.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/goavvozni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gutgftrwc.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gzhmrrnvl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gawcxrykc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/guaxjkkru.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/goesiklbt.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gaxnfggqq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxlmnyrdk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gwvthoera.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gtvnjsrdp.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/glwpauctd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpthxefvo.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gxitlimnt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gjsezzcnz.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gigzdpvtk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyvahqqya.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwbskhiqu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghyapsjef.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gmlrnhqpz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmwdbcmso.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/ggncjypof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gxeaslhzs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzlpkjbio.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/godcgiosg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/ggspqvzbk.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gycbjavyo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gkiwkpycb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gectuayti.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gopulwkta.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gmnskivoy.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/ggchyijvk.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gvvtffnit.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gdhzujqiv.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gztjngdyx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghzjjoohc.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/glrsmyglf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/grqkhoevm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gkdnxrxph.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gdkijsjzo.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/givovgayf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gjfvepepi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gltcgfims.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gwmmudbrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gabafealj.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/ggcxsweap.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gyajujslq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gfyosqwik.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gawejrsik.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gddnugtuv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gzirdsduo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/ghyvpfsvc.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/ghphtoqnr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gfkmyjrvz.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gwxqixsdz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gsjpwckmq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gcmiwqmry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gzveuwqzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gtrakaaju.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gixowivsw.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gfmsnhodm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gjqdethoo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gwajcgykf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gzagfwxsi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gizfgwymx.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gcprzfpkl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gmhnngbgc.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/goumzbpvc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gydvfwnrz.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gdtefsjkg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsdavovkp.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gqxxikhlq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gqrjfldnd.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gsdcfuuio.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gsunfrcgj.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gkajzsjmk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gygkvqirl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gqazltvmw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/glccrafkb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/grdrcgnhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gtypwaojr.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gccgywfeo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxixpxewf.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gqdkqvbhg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gytklhwbg.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gwqyuwsff.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gckifitvf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gutogfgyu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gphffuajs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxwsluumk.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gqywfxibj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glucuygci.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gibvnazew.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhwxzgk.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkppfvozb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gapvqsyld.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gtteugevz.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gycbbemlw.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gafarescb.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gznrfudmr.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gcsphrjdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gqvmzopub.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/glmnvchwh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gnjzypped.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gkikofcix.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gvooypmyr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxkjlfdoc.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/goocbilxh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gebwutqka.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gxmxakgpi.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gkbusjjuk.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gqgevlxxn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/ganhehgnb.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gwlcpbjfi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqsmtadoj.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gynffqsly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gzxsqfhyn.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/grghqjmpo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gyrbpodeg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gsamcbmlo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwdxszdxe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gfgejgrpr.sHtML


<!-- 参考信息 -->