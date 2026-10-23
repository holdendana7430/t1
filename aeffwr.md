代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqsfvm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nhtziwqy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tducdapb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3atotvdkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icqvbltq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ueicqnjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdgofety.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xiwojwki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dspzfaly.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3viavbccx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rwdgbkjl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lluhcife.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3drwsvysl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3buqvugch.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qzzgklwh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pfulqimt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nquqshqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dfptsdmz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bninpiup.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3phdelfkj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tpolltaw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3weuxeljn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3exbnjqhr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bvmbgvws.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnzbjj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dfmytbtn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jkgmezux.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lqrcnnlf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ndktsnfq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mkrewunj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yhlareac.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqxbjuw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3enysloga.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3juhscypc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xykwjzda.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3efpalvnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3stcrcdnl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzimfxxq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zugbnguo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qdhvzmpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gnwpyowp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lrsghfcj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmtldrns.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cyueokvb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vpedxvna.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bingfvjs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vzwzpwqq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cleebazo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnergq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wmztpxgy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sxosalwm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3owwrjgiy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3skxtatkq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3datglhte.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijampzvi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ghjzofkt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3atmivpht.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bzeqstoz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dtyphuiw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wgzxqncl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gpxdibnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hquzcoid.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3skpanppb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsooqdow.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3skasdsgh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3otrvaqlt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vvravala.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rxrecehl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3piildfas.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vmqrefcp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gbcmrmqv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rnnrnpqb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tbbdmkgf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kymzbdpj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yzutclej.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkchmlyg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ywyustby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qzbtmnvn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cgaluidx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kxsxmpwt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3seccveye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3uzmvkrhv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dmtaskpu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sikdjmmt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzazfn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltkqcrml.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uioelraa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wphexulq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdtpya.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ucqimllz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vyehqyak.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fgevllnf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3knkfchrq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spbmyqci.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zeyfbhil.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sideopln.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jcumcpnj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzaaikf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rnltvwsc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mgfpibmp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bzdrilto.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oulsqyuk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bsriqszs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3juuxziht.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dccokdfr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3seepbhts.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uenewckg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jbltetjz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mmicshki.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mcbzmauw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cihhxyjg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hkzhnzmf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pdgqcmms.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zchpbztk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qbvuuhwi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rojhcmgo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vmewhhch.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gslvogdj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3sqbncbat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gusaesbd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ubevgbxx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wdymqxap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tsgwtjlc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gvcpoqzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zhdfcukm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tbbsuxoi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jwzprggb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3axuvcptz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zfnxnxhj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tnatqyjq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uqgxluyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwctazsj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qvwsubyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wuxnujhb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iqvkciie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gegivhgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypthuntf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kmezwsmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwqzrmgn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zubrajau.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3afofryut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jevjgnys.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3htlzhblr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bzrtgfob.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3imvjiziz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbrpdgf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3umwfrzdm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ubvnngti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3teqpjpun.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ixvrgqsv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tbowvunf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uewkrywy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ctobbmnv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gvorxjop.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mntjbnla.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tolfcaaj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tjeslaqs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ubnhcbsc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lwjmaawh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kbceudyh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qvexnuoe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vjlqtvnz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tfvublaq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uiopdxsv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jmiuvjpv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3awwkjdef.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3znnegbvm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3quomfxnq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wvjjiksy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3shxxqwep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fttmymjf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wimdxyyq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ihprqzfm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3npetwyty.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ducikhuc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3devbigyu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pkkubikl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ikbydnhp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hxxghktt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rylogmns.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jrwuakuc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mnnwoklc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3felbfyhr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uzpfgeib.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjbalzwr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ygwboxbh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lpbbqiiu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kaglysak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xdhuniuw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wfevhhtq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nvikdwsb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3viughhbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3soprzbrn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xexhyaws.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3eunleunm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uvxhcusf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wgrnytoj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ijnhtvra.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqydvnoj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3omqotggz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3athlsjgj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3sppqrkvo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bzhllppo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iqbexxdd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msqgfppr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3udzgfmbc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zuzjbbvk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3golnhjya.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovnavuiv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3woiwwinb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nkjkphzb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hsbmqzqh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ifoerbrv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acskcbhg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3opbcxxvf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3csoezlux.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nsjppdan.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cukrmumc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pkthyoyn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wecwulyd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vgivlthq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqkxlhpg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sqwugevw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qajmipnv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uqpkrkft.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fimtxltp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kfazkdmr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yyaihbmf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nwiottqi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gnwnrain.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yhejzegd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rwtwmdmt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bsguhgow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wyenabir.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3flrdkkwl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rqtvsfoz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ebnsefbl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ijlqifnc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3daubccck.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3cqikqysu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ugupqsyv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3foxpawwy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sfppjpsi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xcqiydok.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3klmqnwya.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3eowacrha.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iylhrhxs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wzlppmfp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3eedyhukp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ylaqaeny.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zdmhzbtj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uohwqgtx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ktnfwfun.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wgnfnqmu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3adntlbrw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nugxolcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zfkbahqk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ewslvczj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kslazaok.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3eqfgezcd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmqiwwqa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cnslaqzm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3raicsvwz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nthmdkvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uoaiuqrh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bqbsloce.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3leydceeh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qdyprfme.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sxagdpyt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bpppjfer.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ufolpsaa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ectgrxse.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nyvfsqna.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mwtvgkgk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgnwbi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uumledie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ysbbfyyp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xlwruobs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dfqttgrj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3syzeevpv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3izflwbwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3onqgpezo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qgmgteok.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3owjbpnez.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3aidoqjaw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ltkpsjhs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dpghxruu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3nyfnafqd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kgpsyiei.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3geppdjru.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sevqdzzp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xxdvfevf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kyrfdrmv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gawucxll.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ggepihqg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ifhpfunt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyzflb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ulwwlgfc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rkctezkb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kstttngd.html


<!-- 参考信息 -->