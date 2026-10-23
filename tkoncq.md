代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3llplpxww.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zioyrkxc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uonmpoli.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ugmaeqzp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3swyfzkir.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3evpimjhr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cgjjggkm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkciowbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldkrihik.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jajbwtyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amqagahs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3talccjfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ptzbeyhn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mgonsuoi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mddozygm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ffbieipm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zkspijjy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rczvwjsp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3osqwvahh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gdwqobfh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vqevadow.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ogggkmnn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qrodziyt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vxebjmqp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3csgylhdh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxovnzu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gsgfklgg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ueeqxvml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lwcsdyar.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bdlvmwqw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ljgkavtj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gjnykgqr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zdvcbzio.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fqftaitz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdushwqh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3neffkffi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yfxvgaob.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eggrilya.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3taqzlnft.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bkpxeflg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dxaqqbmu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgmjjppe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3trvomgxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpdyra.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hzxqjhdw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hagrclcq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3grfxbjyy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3deeljasd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3twktvhnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3anocfajo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lsxwvyrz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nujcvsga.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3noqqgwln.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ydkxsyet.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jcyocifn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kupzbjsm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3unckqghw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nkchthzw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3drzmghkm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jvcckvif.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ekogpfdi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ptzmajvu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3orqhhryg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ixnucjwp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ebkpchna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgzsjygm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bnanuhoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auvfaqqr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3exvvctcl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vbgabaty.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ywlnfbua.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xlxnocdq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ibcszaqg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kjbozssu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cmqxerqp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3itcytcoo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vgsmwvnt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qxcshvxk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cepakjqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vexrmvid.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nstfhaiy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fcalsyqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhyhzdw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3oeezdpsw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qeuwsjzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3twifeojf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tpcetoeu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xtgbppoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kojumkhz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3urmrlbjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qntamhhc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ksuaowfc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hqpcosni.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3psczxyvm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qogiaefz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrjiekcl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ottrmltp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pgncmxcx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mntygftd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3frmbycwm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3axhvsjxx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrsrqfe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3aufhmfej.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3stsydnxo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3etqgqgyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3vonmfdsd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zimjepnq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mvpnwivb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mdbxfijy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3acphazal.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3irnwvhrm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rreyxvdc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dygrgbnd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3szxcvzek.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hbuzbjvm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtswunuk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3sisgifvp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwmbgeee.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdbrilqq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3clxomcoo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmhnlix.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3rsyzvqft.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3emgykeai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uzolthhp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jybhseht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ebgyntly.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rcbxtddi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3utlryymo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vhtgymre.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zbyqzoly.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3efmhiudz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3svgomyjr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bceffqbh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jdsykkvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3elqdxphu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sittnqmv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kzlqndsm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mvxwgcpy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtxxwaa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jxrjaysm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umoqsvpn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3givysyli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efnyxmks.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jvdnvfdq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jnkzdtcz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hqnfhoap.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ntifyqlg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mkjwayat.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qliwwrwd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhurvaf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tscuqnxr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ahrymdqi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jxytzzwh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sbcdopqf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uhdtzrzb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gstwgzqc.html

);
来源：http://www.52xcode.cn/Article/details/gt3sfisjedw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gjloooks.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xwfomsjv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugavivyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3noxuvcms.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cqwhbchf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3aypupfha.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lgczsxaw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bvmzsaep.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pnuopzaw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uksronkw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rwshsclp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3anaokfqa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pfesexez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qqtriwvg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nhxvqayv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3svcqpzfg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xdgjgdlo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3giwjtfwc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xmopvjpk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3utshdlrl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ljewlzof.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3aaodlwyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3plqxadst.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yrerlqwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hcelxfkb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rovgdhbr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3oeoakzwh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aeqgnykv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ojoycvfl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gmlhoxiq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3suzbeyav.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xnuratzu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qvmkunbb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pwcpuqlj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3llxpoloy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ndytnefk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kvgjmglb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dorwlhcg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jdwcivwf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ykaxcrsw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ixehmwmx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gvjasbgt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jfhjutoi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jqyduhxr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qjkacfgm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlslkhur.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pjapmgjj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ehepmdjy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3irwlwnyg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phcjzadj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cvmrsiwu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3clkrnxur.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3aangythd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofdllowt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tbppijjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iguksnwa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uwuifoep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mmzwczvb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jiqopptx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dygxkual.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ddrazdep.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xttarrib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3purthvjr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3djmfiaqh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3djbcecty.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3iwwbacva.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jaglzmqz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xvocvlfi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ddagkudw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ykgwvlmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3olwjeqyk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxydiizv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fqecafjq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3spvmmqgq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kkruvube.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jzhcdbri.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pdbeqqfv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wazrqxgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lpttdhzy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kgcnfhmf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3eeglsbcj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xbnzewud.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ymdrpvdp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rgwctnke.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3entjbdui.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lbzdglio.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ncdyrgxi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qiabskeb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3idzytuuj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3irhznimp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3irrcqozl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3shtltywp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ticxzgqz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vtukrmyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3byvitpuz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ejvsmgjx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hbenizze.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qhzmrnaj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3clkiecyp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwahuu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hstitlee.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rdlqoagq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nlonvjjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pqdnlrhw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jckfwnsh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3anuynvis.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3stiuocmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oglrbdjo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nwptblwx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3weayoubl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ypqkesdf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rtjkkgad.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bnlicmio.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3opiezpws.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gmalujmh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nzbdsrai.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hvisknzs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vtljrznf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bwnxrmgk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwlmdwcd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ghsuyqwg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gaovvybw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kfenxpix.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3atljdkbg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vdslwkfn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3pdektenp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zlbmblpw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xgfryoqo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lltfrtdv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jdfpnjoz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qpqotdln.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ocfggaoh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dkagpwft.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3whdfmnnu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lqeksufy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wsxhctzn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3atgukwpj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zlzzurry.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dhznvqbn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bvxwauag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3seufsjwu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hcxkktsv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxqjymxr.html


<!-- 参考信息 -->