代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qkgzmsdq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3scxheabu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hmspqeyp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3woepwyiv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lziwleao.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jgwtdvdv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmgdpojl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3deblfief.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioecowjs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3idzqddvw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ltgwxinr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jovllmia.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lyjbqyiz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3slmanpjr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fenlxbhs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vvdcllmt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hjdyeprr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uhcicfar.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3whaayiku.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pjsrcccq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3evoxiakq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3trughcou.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3icfemezf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tpaoikcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljfunfyz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xtzdrtvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glyromdq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3adsmnbqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wnlznnij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mfgsuxav.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vcwclmpi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3abfhwcyf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qmalaqnr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bwirrwhy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hlcgdthc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dnmlkmkf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qajlbper.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zyzxbfuw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dzapvqec.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vlybcyqn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sjceybvv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pfpafbsx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gtwsivit.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dwksddeo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qinrdoqy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qgzffnlp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyopzlhy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nmnlxydf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cyjoltpn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xabfqppl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxzsdhip.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pzmxvuqy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3okwljfgy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvpmqsd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rhpwwvlj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ulzfmjsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zxnlrkhu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozyvellj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdizhhok.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dwrddvxu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mufnfzgh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iobwsetx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pmhyoxqg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rmjsojvh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wfobmdmq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cholcebz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtmnhbs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3deoandpz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3abrggdas.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3awioeprj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wykgcjab.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwozuzri.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cnyipkim.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3weortlxx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zskkluri.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3prbasoob.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tojlpgfl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3heecsrsh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jrndemow.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qhjsoibf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ysmcgscm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxjhcacc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mooqseye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlkibzoe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pytlnkab.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wrtlddhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bmdkqtve.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ypygekgi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zkxzmvle.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ypmqnrql.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3geamnmwn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3unqfrtls.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3toktnmjt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nsveeziz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cgegprvn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qjfvbhyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jbedmwba.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gomxmmfy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3auxpeter.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vzytuuqt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrhhdma.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zrhythho.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3svigpeko.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yuhtsdks.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yrcdqzwd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jptpybqx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nptmjxqn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxbqajw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fkrbcpic.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yzloswuu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mqiqkvoz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ekfwzcwd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wztxaxix.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vgkyqjdu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3babytbed.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nnqdkezx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3snrzzitj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxmbfme.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ypkppspv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pejaaygw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jaxiqzkp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kjthhjom.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sbiecleu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gtcfqwuo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bkpzjske.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3irwecucv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnezlbia.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wymikhhk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kzvtkhdv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3znoixqjk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3waaqwicd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lapkgwrw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mwjlhjkd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmqzlifi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yrybbncw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3avypfqln.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3enjbznvn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndgqefzn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vygsfyze.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sdqusoyz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gcmhdvxe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cnkhfyoh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pmwbxhtn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqipyzhk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dvhtadea.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mowjdmrz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dnugqlzi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3njxahvtr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3erlbtnsc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ffhvqaqw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mupcmauj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qauxayaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jpxhqfab.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3muaxgdrz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3psicuqfw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wpwhevby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neogdeov.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3huabnone.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtzphjof.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sjabpltf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ljqxggfl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uchivlbi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3basosscz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xmuzebei.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gpohbnvi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ryzjilxp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3foylnmvx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3htckprug.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kizxomuc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gicrxelr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3atjbemwt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cyhgmalf.html

);
来源：http://www.52xcode.cn/Article/details/gt3fmrusrej.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fefyvuyh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jsvskdzm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zgjfywls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3csexzith.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ywzzyyiv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dgbbmlee.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tkisjenx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fkimkqka.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xtdtghiq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rfbtuyzr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ooavprai.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfiguka.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3frlsbiuj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xldqfpbg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gwqlplel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3koziacmy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jktsfioy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eebppqve.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3quojtnhj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3uthhimul.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ialpmlxe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qdcxtyip.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3idfrkkpo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3agitnths.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vebthbdd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lttjmxyt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qcarzjed.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbdnzevq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dxupgnyy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfkxailp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qyjybivl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucduhjxs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zbzegmut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3duvlkicq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mxmzvxiv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ijihpgmu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ezwvydzv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rcxxqult.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3clwdjhfl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3esxtgwlp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ebmykshb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xxqfmkvw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rxiayvoz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fmmcvjku.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3frpjexgg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hkyzvcjp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rclyxbqh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xkkacvsr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3alwvsrds.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wakpnyfs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mqlrrsii.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwcubciw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtvgqu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ujvckynz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hydxrpdf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjvbgnsz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kzfevmpe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kxdstvps.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ybwlccje.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3clpmtfby.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wetducvg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fsputczj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uqatzucz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hyzlijbo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vsieekrr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3javgqpyt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3owypqjru.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wbaobgrw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jtorvzxv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oxgnfzit.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qrsujxha.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tthbwump.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3adnxflkx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vjgwwhyn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rbfeavwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pezlmiep.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zyrlqzsn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ckrlvxhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3avxvjjpl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3seiamxhw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hcgagqzb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xnhhsyex.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3iyfzxqys.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xrzdujzb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vxehknpa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3junrdiiz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tribkgpi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hvvwkcon.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nwmyyidp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fbtvbbmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nqywaqaz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3apmedmvi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rzycicpv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gvqjgdpm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dgzoejso.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3owcnvdqs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kyrisrgs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lodsgttl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jlyoszal.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xuigzuex.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yobtkupl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xknzsldj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dtthnlvv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kpptvrsy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gtavwqni.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nfyainod.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hzozczmg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dsvngoyl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yohyfumz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aymccyfa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wvzztbup.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rovgganx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xxmznwky.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ucvqfwux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3txkwgxlx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zviwpxgc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ybecamxb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vnyojdpb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mmjpkdgt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfliofgp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ywgcqjak.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wjlvlxpi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nsitjgrp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nwineosw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xnhciclg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dwoskrnp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3baedievh.html


<!-- 参考信息 -->