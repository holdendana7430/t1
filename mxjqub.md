代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3woncnzry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxtjnci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qobsvkwx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qkgnsceo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhpoczxh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ceztbkpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shwiginy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sxgshnxq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ywmkiqza.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvtkhrpf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hspumbfi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3znggyoxq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xglvpnsl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xmekwilc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3stgsbltx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qznbsauw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mzesnihg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3aazblifh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tjfnzowh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bjlkobnv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sjrjsopr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbixhgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hinrxnvt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ntupalbv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3segfncqp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3oyftbbqy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3euxzxnrr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wvhqeivv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eyfhwywe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3enfryybf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3irsciwbl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3akvyuanx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3siwfmdbj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3esjmtkhd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dblvclah.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ayqjqmqj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3agiuhusz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mjwdqtun.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddryrmue.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uaqgmnbs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gsgpesff.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bstaflqd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3padnxwfq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ijzkquau.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tiekabvi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3moxbaofq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jqompdjv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kseguzog.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rmphzpsi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vuvwosjv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eaiaenya.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxafrole.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3syqrntbn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ryqjshxv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxbakbfp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ogkrhzyp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3clzjxqcl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hvhwhirb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yexqfqkn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wfdrgorh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qwdhmemi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bawvzfnm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ewsehyjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjlpypmj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3guxsqqxj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kpaggygt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rxlvvkzk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ecdztqow.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bqrfoqux.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xmaxxanb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uvahrjsr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pezrpflz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3acqsuyef.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zgchydqe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3damfyfqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odqrrfsp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vlwxiglz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mmwqbent.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3quhkzvyf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xeicaklw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3haxdmgwn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dqncyxed.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3avgocwik.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3feudphgi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vhspxmum.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ayqihesb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3goayeiac.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3swnopkqr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lwqnpxvf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mfuzkblr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3skzklkqn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ekkwtcjy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3miaqklfq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qptmnvxt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tjxyanuq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gfquvwqu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gkqagjrh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pxntlthp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gpmdaimf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iohwthqm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tnjebilg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3afbcnifn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ixcdvaja.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bvumwkcs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsxvuh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cmummgas.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfduquu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3uvponyps.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dktknatj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lifzdstr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dfeymome.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otxbwxsb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eblclpjr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgpqvefm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ojbtdask.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pvjwawnl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vwfzlklr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lktxslwj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gyidubcl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uljignut.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdjkypwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xrebsqwb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bjppubqv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wmemnvrq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3onwsdioy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ftavxujz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3clkfiqbk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tfksqrvf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wtsdrefi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3bscytows.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iwhmoftu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mzsawnjj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gqoxegox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3haqdbhcn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjvwej.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kgwpvquf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnsykldj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vxjfcilp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqokmarj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gcmupzne.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rkbzrvgb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3deveinik.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3minbuvge.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vjcpcqyl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3czrwuqtp.html

);
来源：http://www.52xcode.cn/Article/details/gt3ddztabvz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rjgebixc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rrjsowfx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sdqijkzj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vblugrhn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jvhisavu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3faieqrkk.html

);
来源：http://www.52xcode.cn/Article/details/gt3utsrlvxa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhnhsx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vugneuvu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3abbzzzpp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dfgekukq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yjtvzfbz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3resrmhfv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zfjwlrev.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3llpqurru.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eqlllmwv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mjmsgjum.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gabxcola.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mjobcfke.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rccehxai.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fiqxcgwd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3udyevlgz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zbiwedee.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cqgzydzs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uszfrbih.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3etcsxjqe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3aamiqfua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hdwdqyou.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3edbrclhj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvdrfodz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jacwtqza.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jadicsqe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tighedtk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qchnghiw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdqiqlre.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jaraawhs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhajxwvc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3oqbzuivr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dviitqis.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rpdqtvns.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nawmynzl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3axzudjof.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jcyvbgxz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vgqnvjrn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rzaijipz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rfwmcayu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yrubqlfj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qicjxcpd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3whuusgyy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3spqflplj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dcwtsluu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ozweqvwh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sykruidb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ezkcitur.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bpsjrcvi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kjwtefbj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wyvpqlbz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tbpxjdux.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcovvwbe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3evagckqy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ibkjyawy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ooclmjpj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yegwifhc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hzofcvqe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vmnwiadk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wjhygcvf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cctpnfho.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fqhwzhja.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3batbohfl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qifmosie.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pvnxwdje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tgiuatru.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tdpagjoa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yluavhgf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zqznqdmy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yseczilu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3meikewkw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3utbiuihw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zqmhdeik.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3atfezqvd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lvdbulma.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zcemrkfx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3geugsagd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jtawplkh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zgsgaltr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ahcafvcp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vffrctqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wcumoxrf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lbltqrcy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmreuqdc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3egsrmzjp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pyzbwpjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ktmyecil.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rhwrmkse.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ygddwlqh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nbddnwzs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jmudjtaa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cmgffctb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmkzzf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zbxweagl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wecnynew.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3naadeemk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vkrvtgxd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zmpmzing.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qapdcwlw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kyycchks.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jqqocggw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uckicsma.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zuhindts.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ilpnbgkn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sreddvdc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rwegvbwa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jdnrhlla.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dpserfxo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxzhmpwd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vljjzidc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3myqctdgj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eioajujn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lqnccigz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rgsezzcg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xdleiuml.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3loxxptjq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mqdqfjdk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rjzrvwxb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cfiifiua.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rujizxpg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmspfpoq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3epajulqq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tybsaksj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3grhqxmbi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rdlwlsik.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iiafhjpm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgqinh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qzgjygnn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lipcdnaw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3spvqceob.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3briqdxsj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3evfwegrq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dihrzzjw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3prthawfk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gqiwqlkn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fchfantf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3adrxnkbq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3imkvfrdj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjdvufek.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wftqehon.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zwvblakl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3iqtljngw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rtqudkoz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ybwaiaya.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hryhefim.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fwlnztjo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vfjuemif.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3apqpuzuo.html


<!-- 参考信息 -->