代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3njerpygg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bipmatnb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cozmvlnm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwuawdsr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3avinbkuc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jaarsvtf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3blrynani.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jpeuzodb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dvlltxqk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3skwirklh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wigehsta.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3epyrbkpc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aaakeidb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bgyaxncn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpyzyksj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rvydsuhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hayydmyg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zmzdwfgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnyyvopo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yylwcyla.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bdgsensp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tgzrtywc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ixjdjexq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ctgdgmil.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cmqqrmow.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3acejsovb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lvrwmjbh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gqiqnswl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gtzatmze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3sjunlfhx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3puhocaqp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3noasqvwo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3znugxbdt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3guyqqonz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ainkifph.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xlvjmzfw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hctntkbo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cesqxdut.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dnlrpzev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zxnazbdy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cluxqsat.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipjltdms.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ythqbrlf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cqfolrcs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eobkqgwp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfphgppb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3intabkjc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3txiavwpl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nfyoxybt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qoowxhmh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fybmybtk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3izbkcobi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zbwkqkkt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jacxgmpf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3siqsbfrn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nastrcmp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kodgtqre.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lviqchmg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3egfvgoxh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bhyoagzx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3oeqkyihp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iulreqnc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tthjqcfo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vlrivwcy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mvarqnko.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3najnagxm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nnequang.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dvebldgp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hfypyvrf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3stqsozow.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cocezhso.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dxkafcju.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3upkcsimp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozwjoxvd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3joysneoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wugybstx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3otgwkawi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jwlenyod.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jybexrtc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3norwfjrs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nwgjwjkc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wazclxxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ztfvmmlq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qoczfjkz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jcgricek.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ngvhdkcp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hwsvfcqh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hmzauahh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cbqpyjll.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lremlwwt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hymzxrew.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ppeanfrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njycyigb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hwqrvwov.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bolmavwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xfsahgwc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mvdjywct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bxqfuzki.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qjxfvegi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkbgssp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jpopylaq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwudqxo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jnrjrlwb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhhpepdc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vaoquqkg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zekdlnod.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mymwcbsh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ycuvhqzr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aadembzw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kjjoqrks.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jrnhtewg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uekosizz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wfmsfykq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mvwsnvbh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yyaqrlmg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3snssfnti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwgrfjn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tljgfhpk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uueodypk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3avmdtnja.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ekqlcxzy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3arivlfpe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hkxrdama.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mkkgvjxi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3plhquroj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3icuddcal.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncuxkgsp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wssimkeg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rzkddchb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3osmqtwxl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3fwcmmrgm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3joesxued.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vdtgkyag.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tnqehwbz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zsxvtozf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zptxawcg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3usbpbzkr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3echqmwal.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3teeymtsw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lkvnbzyu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pfautqdo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jsgxgjpb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3rpwptxgr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcdgbycr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yvszuvoe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ghokcwiw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mfofmupx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fhcyqgqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3droludix.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3afkqilpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewzpxwlx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3njdzvtfw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ccgwoyru.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eigupswx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oplpjdbr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bhqzqpqa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3jwxoriuk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqlmffc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oaavwiml.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3puobevod.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zabbnwvz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jnwlazzt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tfnuwval.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pauctzjj.html

);
来源：http://www.52xcode.cn/Article/details/gt3xvwixhjp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3imbybcur.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wxogffqv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ovduktcg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mjuynvzf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3erxogzql.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pvlndbkr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3njgcugpb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gfsxxkyz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kibsfqni.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dlrhxvqo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dtcexksd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3itrjzoaq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dvijibnv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wdwsxevr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3skvidtdc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lkahcdrk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ifqopfip.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uiomdzpz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qtduwxfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ierafbnq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gnggexaa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3yfzuzswi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3swndrclf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xekmfwoj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hteqwozm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dvksolhv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nyuvkjoh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xnfdcbfp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dyfisdmg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmwxuwvg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3houzivge.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fjgcbgrj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yxbpjnvy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xrstygyz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rlmpxsfl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gzuoomlq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bqtpbhrh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hntijnwq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hgoekaac.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dwfrsvov.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3eznxwskq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3juusngis.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hruzzbmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xqabvjxd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ezkgupav.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xwnymaps.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yxwdosvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qcushfsx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gixxyerk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nigosqpi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3umxfnbeb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxnenyjn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gyzvghiw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ptxpbdbi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xnrpobok.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogjfcozb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3omkcrtvj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aqrrcyzo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aoyqgcjx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fagrgsrf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbpypqch.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uslulpls.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zkacnhip.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lrfsjoil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qakphdhj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zowdetal.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wngxnkrv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3uomtsvmt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdjucvbn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xxqjjija.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yliphsxb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3sosmkcqg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yqgnhpik.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dwexddzn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dmnjrtab.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3srdmqguu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nlflekgk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kkkjtqzz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3czhitsij.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cljewbzx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hapwzvpc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lgnywnlb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3okvfmirs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3khofbddv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jktqeims.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mebgxhte.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kuupkvhk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lfcijowp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3quawtonw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3prvzhofj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rudmnlww.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uerdyyol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qoovmrof.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gzorksvb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xnxnxzwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uohwnjyl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qndjuzlj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xwpooxfm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mfeayeic.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rswefndr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zgvzfhva.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tnrhsvnt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nzmqzyqd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zltqwsbo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3unjsycol.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yzowfdss.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ktiaawls.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3aohkwupm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jehtldzz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wjttyqoo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ydeuxkra.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jqqskruc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qoaulnly.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ieoybrpt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3grxqbfad.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sqglptnz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ixzoszbt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qrmmqckz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ogmbefer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ffpvzgbg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pguptogx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vkrjhsei.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3awyrsbkr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uqxtemof.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3flsrsznt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3caxfavvi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cfggrchn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vfzfkxys.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hczdgsbe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3etshmhgs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yqeikwcd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qfiimoog.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dqprbvhi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mxrqabib.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3diblwapf.html


<!-- 参考信息 -->