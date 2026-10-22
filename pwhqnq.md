代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qjuijsfc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hoiqfqon.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mvnxixfc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yonexytg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksiswbty.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zswmmqhg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2opgselmk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wiajfcwf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gqoguqvr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xdcflqym.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zplvdpzl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wfxivyzy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sldcufcj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ulkurkiu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xqyygwqd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ugbmjfgq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2leowddwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fxipapzf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2atoobmfp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vbyammgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2finyzabm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ownqkzwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovmfebtj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jpyhjmey.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2twzjltkh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zpsuojws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pmqbrtco.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bjkifwri.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jwaqueuf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ztkooaio.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tlwehdfm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vypnjivl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2heaepskf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tiyqblzk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ctlarxbv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zhkgzmil.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wmrzlppl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sduwcebc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pqakpkoy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nnweffpi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lkmkrazk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hbhzjkql.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tgxwtyoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2imiumdpp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2uinajduy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vtaocdee.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ksliocll.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2catcunbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ckrbqihe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjpnbkcj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ubvtylya.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wgzfngba.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gaizfmzy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ntewuzjp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jryfngeg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ulqlqizh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pnmasjjp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bzfzxkbt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dimmwmwa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zyhxynzc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hsopnloq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pagggmlw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qymgzghv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xznlojnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nslzjbya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kcjodyve.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qilufjah.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kytamxgi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zyffwblx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ulqjiobx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ywniybhw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hlphqiny.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iphaoyhe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2neqxntxq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ketlubbr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gjdgydns.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ifbuajzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpgrgubf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2acsquibt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlfgxjtl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2poepyegp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2anuwloko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qntifute.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wyfhadxa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mtzucxfc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2keoknkua.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nukavxim.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2weiwtqrv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qujqwxyp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pmunujop.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jtjuaoaq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbicidpi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2napioapr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fpuarguq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jmzlywvv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sirjkqlq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xodaxosn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fkcwgptp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tffbiqag.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kfoldisu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pcxdtirp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ogsgpglg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svqackdq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aeipteyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lknyyfix.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoraxwy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fplxlfct.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vixtuvjf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2igrjbeci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pbtuaute.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ishhghzm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fcthutjp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tazkszyo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tsyqygcf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vgemnetk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iznwuown.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xclgtxdm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iqgjkjdv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wbipnksw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qhckxvdv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cdlbytgy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qyvpqmdo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2syujsrll.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dtgabdgj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2trlkiivn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2guuvaxkc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2itmnbset.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwkrriwy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ezmprums.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcubkhkl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uythavyz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2axqskqdh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzldnp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbrsmvqz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vjlehryk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2izgolodw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eyquizrr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bgglmghq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pbvkjsvs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxwptngo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gpcfxxrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lwxjbmkl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ctbbcloe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ooofevhr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lfdqpgkd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2karggsps.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wkiegacu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eikofkyv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xuspfhay.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ggnsgwyf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2iniutxgj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2azgtbmxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqdqldsj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lpcijmjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2natoqdpa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2donqlurq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qyclmswp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xugmodch.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2irhbjden.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bzmbzxtg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yysggddt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjkduvw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2prdlmrrk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oypzrzai.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rxijixjm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lntkfkzq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lyrejnpp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ladtskei.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mscelbyj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2polbptze.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2yiukwmtx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2sqfloxhg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gqldwldb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2naiglbhi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cibghcbs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fvnfwwma.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2shqdqwhc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nzkuuron.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2rxmcoukf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zquknflg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bmuectmk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ldpvqcrh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hnpaqeud.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uihutxnh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yunkpact.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jqunrdop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ccjvfoet.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fnamnvzm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ghhlaesg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cnnbgmsh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mgccykit.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fpqbcmwj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uquvsjem.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qxhvmsvr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2alityrgk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pnwguntj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iptbbbcr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qjymxafs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulyfyqsy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ncnqmfeb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ehtjvryq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tlnapzur.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tofuycja.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dyvlsmoy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ecimpgrh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zeifbrvu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gderpxwj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bipdcqlc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hksdndso.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kjlkyjei.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jshzsndi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qxxqzvkm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mofvxxxu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rtvivzsi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jujfwiyl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sgtxmblh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2srurwpzw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dshdqwfb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qikuyfqs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ugmnzsrr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckcvzhju.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uatkhfpv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gwmgbzpk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xjgjbfvm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2slhjangt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hgjvgdly.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mpdkrgte.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fdgnthku.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2klntolve.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oqswekuh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rbroqekg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2djbkazga.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nugnymjj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iezbtffn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hnwnhutl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ytkrouuk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jemnaxju.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dugnawnf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ukeywdev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ptypaohq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vhcvehbs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yenlbuto.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvrcheju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lkokpbgc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pldaazsq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vmspdyry.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dslyfwwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fgmkibdj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dkellcad.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xhfdlnch.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cascnish.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cdwzotig.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bjegbunt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rzmypnth.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bkoipood.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yevllwuk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hkmwdeoj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hsclkwiq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2fcwpoqos.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nyhcanqm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2stvprpva.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jkfywmuj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkyxjrwp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vuygswjv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2febobdzx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lzkhwddp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kdzfuihm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bnypakrd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qrtlssex.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jurgqiaf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zkavvplr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fcivylhx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gydpbszm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ejznfnfd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lanebosq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qqbnndrz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mbmsfdtt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rwomcquq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sodkolfy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zhlblevs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dygukpxa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vxpmmubj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dxtsngjj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2prckoqjt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2axsvbehz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bpqqbkjl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oypkzava.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ykraufmj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2liyjpxql.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ulicuxjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iykzbpkq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ppjvrsii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2igxtjzvp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gzzynwln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ohaebbmr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aqyltfvx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rqisuatn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uezqihzp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gwevixal.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dxzgldks.html


<!-- 参考信息 -->