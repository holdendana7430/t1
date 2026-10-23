代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kxipqdkd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3abhzxdbo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qcaqbknw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fonnotgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgoarooa.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oguhuhfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlxayfwo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qvkoiawa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yyrzdpfh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nsosnwcv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mtumsphv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dtzevaya.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3asgnkpws.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ycryfvrx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3eeiceumy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cipcghti.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nohpzibz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kdngtjmn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3siiovxqx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzaywk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eykirury.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvckpfxf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kqaflnpy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qmslgsrp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vcrirqod.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tjixjujc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yvohdtyg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nokfuplj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zfebkdoo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ornmnzhy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jbdmnxek.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mqclgejn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkhpkxz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xukfzsjl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3adcapqpw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yiknygaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dwtxxfru.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfqnqhro.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3shycafku.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3psoxriza.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ipcghatd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3boqjlrbh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmxtclu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3iaypssmv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfxkvma.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zxbgljfk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fahkmgaz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aulngvhv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cjpgpjku.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cnkqumlb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qndvmkip.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xjslicle.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bepdmsun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vjldrsnf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3voqwzmss.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dwgxmpip.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjjmkler.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pflkkigh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cfnyydgx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nykecfvk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bbhbtkyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gunbvmpf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bpvymone.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtxclifu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pvnrfdfj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zilonyyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uktoezbg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3grfqcoku.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pgsqijgn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qmmecrqa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hwhmyjyw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vttspmmb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3omiipojm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ojmpdkow.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3inajdlgz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yelccgbn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dqnittyu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qtvrgkjc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcxsqp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3izyngspc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xlmhdrpt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uieoxmya.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nlbskyyz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wpkuelmm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3slymrqpy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3omulxqga.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjtpqcrr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ggmwitxt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3cseksjrf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vmyakhjw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rofwwqfl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cvngibwi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ajrkmhmc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jzlnsweh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uehbohmz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3swifkirb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3idaffqgb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxqixfh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kwxssqer.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hgwnorqr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jlgezbeu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dkfkcspq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3umyvmlxs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gwqeqfnd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvlruik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xkmvmvqs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3raygiceu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jvsllwmu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vkwabtvc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wqacztmd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uendsxlk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qehkywjm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bxmstqbm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaitltfw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qbcphrrt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3aercmgmc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tperwtee.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkgqsovb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ewdhddkh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lnruwuax.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3puawlypp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3isnqoqda.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zjomxnrs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bztfphvk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3twycbvrn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qexqgyyj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xsgtomwc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kmidwfnb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hjoflgrv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mkxbgcuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sxfadqda.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3voeztvqh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zgxvpqra.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kqbrdoet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xyajgvby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hfazdnzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwgbtrga.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gmxrzmpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovncmhec.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3srjrqfbo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3skodfbyq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kdeidamh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pfcbrolr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3adfxxfpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vjyqiroz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxryld.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zykhrmus.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hxkhtvny.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3svufuqsk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3utkaqjxy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bckhetxv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cbknibxa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xpwvijqo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jryhqqxe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mjvxdcii.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vjfsxnzh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bdbpzwul.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fbgblwpl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mvjmiftw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3cfpbvgmi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tenonxkm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mnzfzbxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gxbtqerk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fbbpmugi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkeyurv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovonennz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hybugbkt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3uxwnwtfs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oohzkjub.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jybuhnjx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3utlpvwkt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zwpecued.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pnqlwyoi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3htoqwgvr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3okxbjmod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqoqefdf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rilvrtlu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ihyaakia.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qrurczuz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vkalwcsl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wmwlyxau.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lcvzraiu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iirutzdl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fbluegxe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jvsgtqkt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kbmtixgt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3raevjgat.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jemtpoho.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3miabuzxj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bcafsopx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kwtwhgug.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vsjmudmb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lizhmlyg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ilxodjdd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hbqroyoo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3twbdylmy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fjqeozrw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ibfrlawv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jotprahc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dyssbmig.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjxdtd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xoqdgbbh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfmcmagt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mcujllpq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ioxcfvcj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hlwqcpah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdshfpwl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3apnvmlep.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukqhmbvy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pbzdamyu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xihkzkmc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cmdjqbwk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lofeaaub.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ttiwmpam.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3snmshvcc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qrgdgcvv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pnsxedzw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jqabnela.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ajqylyer.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gmysspwq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jgflmolo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ziywherg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qglucbbk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3agjgkznh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3quukyhbi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mxxaulom.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fmziyryo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rhtajjhx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cbjvqfgy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3atliblzi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xixyelhc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3puftqmrh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krvqlygl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gnxdakrf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wocgippp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tnyaabie.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3klswlgpz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uiugqhmn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3msglhinr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3smjbrdfc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3epicnicx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3scoccvnc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jrqtdlbf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qfjgpilm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xknryphu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pszrovzy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3atnqvjqx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zscjyonz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ofgkmktm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qbtdvamu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vktdnfnz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uydjtlze.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rkddpnss.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pgsuuqki.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cmjanjxr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3umeekdck.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pqjnacyi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yvgvqrps.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jpostxtb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gksowntd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uqyormlh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iyapdzph.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tcmdlnci.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fdfxkfse.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ifqobeqo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3aezdhpli.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rvygwszc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hktkuhjb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3evisazop.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ermbykpr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3quwbjkyi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mlmzlccc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtbrocby.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rdivgszc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ogepaebm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nqbfpgfi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3efsomzwr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fzmrdvaw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3coxzxjxu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gazcibsw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bphkxrpz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fyiookke.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sghcbgcu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dfpkkvxs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ljtdtrrx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cegxhuzt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lnbmnsvw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jixphnat.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pghagdsv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ehnxqkun.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pnfvleow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aowrwffl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ucswfrwm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wyppkord.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3oohoiagh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3abgwezqo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fxytjbwh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ycwwftdt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3diqfseot.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bmgskgjf.html


<!-- 参考信息 -->