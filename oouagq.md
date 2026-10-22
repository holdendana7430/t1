代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rbmryibx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mwoourxg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bnktwfep.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2annqhswf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tuuwvbwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bwgmvagn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ojcpmwey.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mifdovuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upqctlvk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hftrvsdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqitqpmx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uxozqmwg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wqiruzum.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bsqhbyee.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rtwgobex.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bnguudwq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tkyisycv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pxcsryeg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ngeybaok.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fqatnkpk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2omwfepla.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2quefpywp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vlvinvgp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tqtueeyi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dwaoddpx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qbaitxbj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zzqmwxem.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2roseinnx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xnyysbju.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hvkhygkg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ayvtkzfs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hnoytvfc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2aukluoth.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qgqeekgk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zqavzwin.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vxcrgrny.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdrumkpt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkseodt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dihwklmh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2klcupgxk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yqzncudp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mcsjlufg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eudrfaxu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hiecsshm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ioinvuac.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gpcrnecp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tqxrshrh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lnzupycr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wlkmengb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cohizjyv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bsphqwyq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ozokvbcn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nkjjafoh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2acznstwx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2iaqzgytg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2znqkvluw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2agzfwlfk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vreasnzt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yhjfqrka.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nwdaitgh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2drswbdik.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pbquxlpz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rtgnuwus.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mhcyoebi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2keibqtke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueqabgvg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nxwaicyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puioglmr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lcfckhcd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2whnobdxh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fqngaclb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2csrxmmyz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2orrmvcdi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pabllbjy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wcxdbqoy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fkhxfmzs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tmzvwyla.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2helyjfju.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ljqryfpy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cljmgevb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vkuxzfzd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ztzrskbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2twkgjxgt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yvdsvbdv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ldurocfw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aghillbb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzhcgsra.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wsnxnhsn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tyzhbypx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgpwyge.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xqdulqqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pcizsbqv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lzfsjzmm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2prqcizkc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qyfvvksi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tauapjdz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njcatlgr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dzmiihxm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xyvthvmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hsffiuzu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mmqtsmrg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfxiktb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zvkbjhmq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xiolfxeu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pikyralx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rbhejpzv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mzxbejes.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2csoiuxwf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qfaepswh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vayapskn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wtflpfti.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lsiigojj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2llxoqboa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2cxvhrigy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fhzxrmes.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2adscrkmo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gwjrlmsc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jguclrvr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2napiwqjp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnvbebfw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ppgtujpf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bprvdsut.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aueaiaiq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nsltywil.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zgkreqbl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aqulilvx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ksibaomv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xlhgvbwx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rflojmxh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rnkaxjej.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2blhhihdj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hgbsvfad.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jmvboytk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2laauvojm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zaolhcto.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2svuwmmwe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zqdbxgvy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vzsjryqd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mntssfjl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yotyyvzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dinvksdy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fepcfvsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhlmscgk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nwafrnts.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lyumzqxa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pddilbeh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gyuzpzib.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2awqnfobw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yfahvazp.html

);
来源：http://www.52xcode.cn/Article/details/gt2mgnhvqdh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dbklpitf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vjswzmbo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kwnnsgdl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ucztaazw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rgqahldv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lyncyuph.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yregmtbi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2azwrkxhe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zolefgho.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ryyaiqep.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ooujlruj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2tlucdoqu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tvdpjaye.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2npmqgezd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tqadvysq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sjzzdvhc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2skeorycc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oxzlbyfg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cyqowyhe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iturmvpe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2waamzagl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ugrjrgtz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ybnpbpow.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zaukaefy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pdttqdoa.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vlxajzjl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xocwypke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2szfmdocm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uyyymkpz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2huhyhogd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2utnfttrl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2budtmxxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ntruolvh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sqtmfeqy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trvjqxun.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uhqpbcao.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iblewnag.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2euogsltp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xjmwmcdu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fzkmwctm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eyqriqds.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wooxybri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2kfsbuuxs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eaxrmnyo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2obvzfsue.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yndgrhsv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eezygwdm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jhuosqna.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xqxiaxgq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2upedlslk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zhdsfwad.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2siuqquyp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqmaqay.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xmllwyjj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pqcegywm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2whssfxok.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2swqbqddk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bsdwkojb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxvctkcc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gnhwtcnw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2quirokwv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ejnykvam.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivxwkfzl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vblmojcw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hgeqpktz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kggznolv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bssdzxxa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2siqghiwo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lbyzxmyx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rgqlhrym.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cwvjlipx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yjzmpfer.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2whotgjhs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pviczzpu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rsccbynt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fpeobhrg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2svadvarm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ajgiidca.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fcfzwetx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwbxgnvn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2muzhonnp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sgnrpgym.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xlhtnxii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rqpvzkzr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2djfnrfnm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qxsjksgs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2razoqdxr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hsbrxwfs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ffyfeutv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gkycldpn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2szpkcyex.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wngsyvny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2snlwkyln.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2eiyfxouh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2akdegxon.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qjefzxto.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hzmnqpcy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lewgsoge.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rvbyvdsq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjoxcid.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ocsvigcc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pddvnrum.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ubkchngz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iseaoeij.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nymzedge.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2amzzujuo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2objnpely.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nnutsuls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xahkksgq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hbqonvhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hbqxrrjv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nenrmkev.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zksbntnt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iwmikbca.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tkveqzmb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rdszgfxw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nsvtmtvo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2clfqgkrx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wacklyim.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wtscrmez.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2urbkrihp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cymerlzd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jirqsyvs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dzablqze.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gwcsbvyc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mhcdhcdp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqrlbeau.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ufautupc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aukouxwb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2isljhejj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lqrvsczc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wcyfkokj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jjmiyanb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uqirmbct.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2huznlifz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2luhngbuj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bjygwhby.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tzjgjych.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kklczclg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2utqoomkv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mtqupneb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vmhsyvhf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvyrgr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eilhabju.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2evaendvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kgelijgs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dzisipnh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mjjajcey.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uhbcrxza.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rhrirkys.html


<!-- 参考信息 -->