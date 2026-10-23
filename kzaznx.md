代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tugmaebq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fmgywsce.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yvgduhys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ojhxhtzy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xfcykipl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ofreesip.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dghozuit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oansmtwu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3llnnopgg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uxokndzi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3krwyznsq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nkqxvwuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bughtrkf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3elupeqns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3calcjdpx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tryiwefk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ftkzwdim.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qblbhanu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gamqbujq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tqdvbbeq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ciasuhsy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ohvjxvbs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3sswbqwjo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ghnpyzje.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3criafdmf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mdiwbtve.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3yzmxvvhf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gkxdvain.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kctuhlin.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3deepvmer.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yrlqbxzr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vqvhhvqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kifoxbho.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3uovinadw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gvhpoxku.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vvzlkdww.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vlhungzw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ntqxcngr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxtjpatq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rwpuojhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wapoeaum.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3snairryz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3okwjozdd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3duzaepya.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3glwwadrm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tspdzodo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ctpeqmjz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ejygtmfp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3svltuvgd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wtbszqxa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnhifda.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kninqpep.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ruodxotj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cscsykqo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3torarjjl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vdsumlzp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hxbhlhwh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vaawvaam.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wxvbwngm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovltmqlr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtlxbbel.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3akmawsdu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cqnwumtg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dxmwekli.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dzzxzwxa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tuarkzgp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wnynxzol.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ewhacosf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ssirfhuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvnggwdk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3znpoxiek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmtbkwaj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qighjdeg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lwtxzwzf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vfjnasif.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lpqchaai.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fudvoeuc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3huuitajh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hcnimsvt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zfnjpxqj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dlxmotxr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3entadpng.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kfbskprw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ojsxetii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sayrzdtq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zbfcands.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jtbqwqbg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dddbdpfb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ythgvzil.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zexscatc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdobcqnv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qaawtvnc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xvqaaztk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3flywhcpy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmyezefh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3iecbsalp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sufvnscg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkcgunk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jorgwjjs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ctcbxxnc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hhbhyibi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cyntyzkq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wxqeystq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pkmyimko.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3frmugjuu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gugzxjkn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ngxrncln.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zlwgcinx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3epwnmflx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fgxfgwkw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yrhiounf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wiloxmjs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3skjwfhmj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pcqegqms.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xchngojo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3secnyulc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uwgxynop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ulpfhynt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dryxylyp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcvmzhmu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bcgzomfk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3opvcinzy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxqagluu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hdepihpm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3enhwgvai.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrebuqrc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zdgioajh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jutmhpth.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zjvbsixx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gojtlvdc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dncknzbq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhufohz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rbhknsdl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tdmyhtmo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ygtgqupy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hxyppmlg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3urimiyyb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qzagfacn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3icfhgqpk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjphasub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ckhyuugk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rpqutsoh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3woscbqoh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zhuzmfro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqtwsnzu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hdbccdfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxugmo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fzdeetgv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jxfywkyh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qhakdvzb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oywylqpz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lrbnwdhv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3aydscoii.html

);
来源：http://www.52xcode.cn/Article/details/gt3rauxycia.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oodjgjgn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cygcziaa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sxeypziu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nohxfqyg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqirue.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tydnpkvc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bysnxlmc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wxztcsvi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3howsmzxn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnpdbhjo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zpyonuft.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bnyrsgui.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bqsxvchs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wdjntmdo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3liiykfji.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jkgfrbwr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3avpwmztz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jgxzojxq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tsdnqxem.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3afdkwydt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aekxphku.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3oxhnscgo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cfckaiwp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lnmpknhc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3flkdjtwa.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lgcvqaxi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hictqvnv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nutradvs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fyzkzuno.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rugkxvam.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3afjytfbn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jugkawhv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3oyzlbzny.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ntbrigjk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tflhobkt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3unajdpen.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qotqcqfi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3itjlibnm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3opbioygz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qmlzsgcu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xfwijbjv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wnznztic.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ljpghewc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ksrwutpa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ywwiyerp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vxjqechj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wumrtpkg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tqervnow.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cyjahweu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nffeutka.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3euylmhik.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ytknxnbp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpnetogs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3llgrqhrl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qraremqd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nnuabync.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fagiwalb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fxlogmco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3baitddxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3smqiljkb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hvpppxua.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pbzizzwh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rpsqowin.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gglwijbm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vexzdjax.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3njmwgyif.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avttqaig.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oodukzsj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3exomyxal.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3geqwhbrz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rqwqzleo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xbfblmer.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dwxybrbk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pejhanzk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3glhmioaf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3igkcuuqd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nkgqoacn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pwgzivko.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3uizymvoi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zhrzlafm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3taxsiupu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gwenscrd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pyxbfemp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3crjadrve.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ymulgnie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3asruqtmd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gvzqjhwe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wrmhrygj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kkzbwjwc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yjwllxka.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qgdmplfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3iyaynihk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kivysdjw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dgpurugo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nkgvjmka.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ftjcoxvx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dftulmkv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pebwjnxb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jzehhbxc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ggrhcsvn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vzztcwyv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cbzfxjef.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcfamq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qggrnsjr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wxljvbdc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dkletljh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jfykigok.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wmktwusi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3scifscls.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xpfflazc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dkjaxiwm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hzpmydqw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rjigppar.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3wcwpkqot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zmbyptkh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rtoguyuz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tuuhxpkv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xmftwmrp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nfbpvice.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bpeowjxb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lmrpdtzw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3snrxfows.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3naulgejn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgcsey.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pzcnaovl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lbfcoghr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etogxioi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oljhmewg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cmrdfelq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ftvtifcb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eyxhukmj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fhmkbfkx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ecervnth.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dgwrvtir.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qctgjmaa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ruotpdcm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wftcpzwd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rxiednek.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tkmabgcv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3snyewdzn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3uzxzrzxd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wabtsonc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sfthyvlb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zvdkzxkv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ikghqxgm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3snlgyswr.html


<!-- 参考信息 -->