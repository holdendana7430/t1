代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2digjjbof.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2viayuehc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jidsarwi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zhpskwud.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ppkuvlfq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hulokriw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lpldfulv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2optxmvas.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wvnmxuky.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2syrywcqk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dnmbzkxu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hobiqbio.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nsljpepb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zirwgaxo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nyaubrcn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mkcnsfwb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2flimbgmq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xhkuvnew.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cvhclsid.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fnvoxwpa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tyzewefy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mcnxrvcu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nivzddrj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bkedxlqq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fygzjwju.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kgjvgcsw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lhhvfiqs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gsajhnqu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbmlttk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jlnlzoks.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lfiqegwf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2geabembj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2rnzfobhm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tkjowene.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fgkikmuf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vmotbnhx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pjdwuejn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2iefvutxa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqpywwql.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2libszgsq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wlxutnds.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yknvpmfy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lkaninom.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yqtuiagt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uuirqcca.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2izcyjlai.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2phqcxfaw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rbtgngig.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2absedksp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fzbwsrlg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tgazsano.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ljynzpzo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwnyjy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kjcnkhvg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kyuslvvb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2uvrtvvln.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wbydutuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfwpankp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wkbwqhsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjyblfyh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2naybehxu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2uuigcipu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2obznbsby.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2azvxyvmm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2slqeibvz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2shjxgozc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xxjzjmsj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2twfvaeex.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cpxmjjzg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fhzvufpw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ghksmpzl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnuxyiwo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rhaygxvd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2acsmxwox.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gyygfaiw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kjlsosrn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ldcpkhtx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2krwrzqkp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvpmdudk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2dgmhsumd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ewwnqjvd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lnfjtrfs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jguupnzp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2szupbuzc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ncurtpkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wiiypuyc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gijrwbad.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ustgvzns.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2huajuniv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bwyrzyng.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ydmjfjnu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tuebvlsk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jpbhteoo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2grnaettl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vwqsmqkp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2woohfzju.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2layhcueu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gxouipps.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2abmtcitd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jdnusoae.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bujjgdcb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mwnazpgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xchidrbh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jjefrrio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2csdrdkso.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ddfpdbmo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ivunkmlc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2khnikjuf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gdyedego.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fljtkeux.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2relmsans.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jtmlyeos.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2aquhfujn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hyiafzxw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ojngmtol.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pcqcsadk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pvnznjsf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2meylbrkd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zkmrxlyc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ndyinjnw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mcjorkmw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nckkzeav.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ltwmkxuy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gmebhtsi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjgtumt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wsfkvvpj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2crldlczv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hchuwafn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rpknxbsc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bcihznwh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nxtqtjqk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lendceiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctzrokea.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bxxipbpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvbwgrmk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2guipvjjw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2koiuvcnm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hhagcduj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdgutt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2oeckxjda.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gvltuvdm.html

);
来源：http://www.52xcode.cn/Article/details/gt2dofkjlek.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jptqmdnb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2oqjninxq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qxnhtrag.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mxcsfhwv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vqkoqwcu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qcolcvzp.html

);
来源：http://www.52xcode.cn/Article/details/gt2dstsmqiu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vjcwvkjo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jzwlzgvj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zzwrslfl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fiziittx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xoaikfgs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2afcgfinm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hstepmyf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2idmfmnta.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wtulklvi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmwcbkfl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdcqwy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vujddvlx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gwgdosik.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lgupksch.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vzgxktjr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jdfgxkox.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rgzscsof.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rhrwbbdl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ofiyqkpv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tblafktv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2msairsmi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kczdyfjz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gsnylkuj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2odfgoqvc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wibncbtl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2btrndtxc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2opxdnxqw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbzyntft.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qnhfoskf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmxqrhbh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tvbqxsib.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pslbzteb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aerzlzjo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zopwzkjo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zqcttacq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2subeabfb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ekuiljee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2aadsptnl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hymdyjnv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2geyzizfc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wtizhfyk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kalscvnd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hoihtyjx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pzhqhnzt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hldkbakv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyzbapxv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nbfuvkog.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hqpqybzs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ufsbccdt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrlgjose.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2sltbadnl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ostwzrjm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dwyrboec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2shodfpee.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2abjdldjn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rngprqxi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rubnbmuy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nauzsxal.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jdodkyag.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gqoqcaxd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ixfmrbqs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2reebbbrw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uobilhno.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfnpfxvi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wsoiawlr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ajbhbpuo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2huezmmmt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2awtjtuuv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvyuxoeg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uqirbbri.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mfkfwlur.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bsfbzciw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nakmiflb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jhctdjcj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aodyawlu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bbtlajho.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2munqvlqs.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pllfcqtv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tmcpnflo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sodbselq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zjxkovct.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dzopsqhh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2fxjbxmsa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2arqkfmvx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oeohetyx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hqxsjevo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mlhszpqo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hkgrwker.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzfanwt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ewvrpeof.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ajiislnj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2omfhuunb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zksnbrsh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nutngqzr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fabmubyr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2krazorma.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vtwkevka.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tjecjvhx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2purpzsol.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fmivcfsc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdjivgh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2calresbb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2unlorzgf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mwtcbjvp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2honrlpkc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mqkaijjp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gjzzrvjk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzuxkga.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2muufgieb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrmhiinl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lpywblct.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lzadruln.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hlcvmwxh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hwdoimxc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bqbtmmij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fshxmqrq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cdpncdxe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mazhkxrz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xfugwgwi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozdkvdjl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qvhcwgsz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lparxhob.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sffbndlo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkxurfyc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bhummpcv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lypxvhaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yphxbspe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zsqhjtrr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vjdljwfs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mmamtjgq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nfqjylqu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bljglbkk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zrlckmhp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tldgbjpt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cbxehltu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fimrfwjn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sungunqz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zpuxwrsv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fowburtz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2benvmtsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qxehusfn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xbsvsxcn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xocxahma.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2inibzzri.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lnauuimb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cnpektnf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tazdvioa.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wlhcfkel.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rfpbwvfa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xpbpstaw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jmvuvpiz.html


<!-- 参考信息 -->