代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tuyissal.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bxzfzufb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rubnrbdt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zplwebxn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3okhwkyer.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wawkienz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqsyhbm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbgwefm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxtocij.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cbmsuiqu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgynvjgp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kvkrgmhf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wobtzodr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3skqjhqbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3blodrvtq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdzsdkef.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jxbmnkch.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wozzwnvx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xriwywal.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fctbmfsn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tigxqtxn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3msslwhna.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3egqtkwlv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvrubofu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nclshjky.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rwkrinvq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ydklyocp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pdlitmkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acxpaxls.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xgfausyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irghwkns.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ruhqgzmv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hbqwipky.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mlgudmdj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bqvwhwtx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cprhciuh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbzmymsy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ogxabbpp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lykvahee.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ydwytjzd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vkuqtohf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zsqgvygh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vxiwqglu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fkccgfbk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tlqjqphh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ghidpqiw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ouinjnbh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eyzqbyot.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fswslsxq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jhjaryos.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lmnmmxte.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3afojxpsy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yssluvur.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jeoftrnw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jroytrsy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fqpsjcue.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lkfcjzwj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3odywkcmi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lkedqgjn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rsowhmwl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tofbtxmt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iablnaqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cwyivwbx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rhpejwqy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3anfmkyfw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rvuxrgcl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcacwhpk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zlewrful.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gcueoqjv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tlwmpmdi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iaqlrvbi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rbbfevty.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jkyldgdd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mbgbmlal.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eatddozo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3khkbjtue.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eiwhjuvk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3loudanqp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3soosazon.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yqkimtkj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dcojfjoz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rjrrydvx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kuyfflbe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bfomlksu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dvzubipe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxfpypsu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uashahee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgoeyxkr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dczkjwrq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bbumylah.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3swuhdnrf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wrcbqcsh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pusrmwud.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rtovwucu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jdlqorxk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xdobqwph.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3njlfafrb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yghfcgax.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mvflznxw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjajnvz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wpkymjpg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kkztcayn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ngztkxdl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3quzxhfru.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3axahvmry.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3evowrsda.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkbwquor.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aqckcwby.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pcstovdt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3efxhefrk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gowyaolm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dtcedhxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hpnpbkiz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3foegdzrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iuhvlzzl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rdtsqdpy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kcbjogco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cnkguahp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tpioptdw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uzgybfvl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ydswcnzy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vxrvyuzh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3iymmsgjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kcofkkxj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ngglobla.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dfkdykaw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3upwaduae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vocbujzg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3afrpdhtp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3moacxwok.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3acfsluet.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xdhzfswq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bszvmahl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3oyucjngr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3umkwvlby.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofpjwxzt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3svjjmffd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jtivrllk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ebsqphxi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqajzmei.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3okquhxjt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3myktdvez.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zernbzfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hyvzxxnr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uejwjzao.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rpgztcdr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pgmapdef.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jsitjqjr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fmmsxtme.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jmlkomum.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3iogeeatu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3srjuwyxe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gmncqvmd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cltaurgu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wqlxdkdg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yxfcmjtw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rnovjkwh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tpblklwm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qimrpxnc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jbahcuyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yedfjxly.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fejuvsml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odrhpqyd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3slroksbf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vkvutvyi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hzndotwq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3azohlkaj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3sybaxtkd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yxwqcolb.html

);
来源：http://www.52xcode.cn/Article/details/gt3hlgvdahw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qcdmrwrz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ierklekt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wboibfvm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qporeydd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fahkzsgp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jqgqsqlr.html

);
来源：http://www.52xcode.cn/Article/details/gt3utossuzr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lwgscbcb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vyjoemnp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bkbzvlev.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtqown.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ngcnwsly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dujxqyaj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tugmxlse.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kmkypget.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3iberztxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ozrziyiz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nvuzibcm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gporbfuw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ksjecsqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mwavrhir.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sxxyiyor.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ycqcrqsg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wfmllbyy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gjgziuyc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vjgkmexy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rsncgrpq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xomlkyxf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dxqqcnzk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3txjwzgwp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qvfyxblb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ewrbcndx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qwedtcwd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ofhwrjcf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pulxwcsw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uctxwdmz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbxnygjk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3enngqule.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdvxfdqb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ozqujmpz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uitienjs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3voosyzff.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xaavkekt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gpgbfjxo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gosnzrlg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3djvbdkxp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3entzwqso.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mtkwnhgp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ptitcaju.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3oltuhgsr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3sukcdwch.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3sqtrveal.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rawfzmuf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cpovpiyx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eaodwrta.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rfexooqz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okbryxqm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rjzrjhcx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zauhfqfz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ljxxajaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sjaednrq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wadqolbk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzcpnffw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrajqh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wsnfagtw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kfkidihj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pixzqimu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kqiaswij.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mwjzlswb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mldwxayd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wltedgga.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lvwncfpk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vktibvhv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ifydnwwz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3equndjgu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgqbgqn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dvhoivpb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vmzdzqtd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qboorict.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qbaemlfl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftofzjkb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3phnibhsf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uliinoap.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rrrvfwpw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3twqcnkip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3eotkbaiu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ffvgrdsm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3sjxyrgjn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rijnszup.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gmapqwkh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3foecuzid.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ivoltzlm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ixnclcca.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pgrhjovn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3htrvtggc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3imhauuyl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bwynclak.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3liuebbgt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3heghrpoq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nxeyebtr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pstfpyqc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lzngptpc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3harawwlb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zhxvcchh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vemddhzp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nvpevvgj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vvqwqrmx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3beecsycd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3niqclgug.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3juihtvym.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sssfwpbd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3billkzem.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lrwcxkqb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuinxtjk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vqtcfxiv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ibkbugfn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zhfdbyvk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xurbqtyr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ccxadkxn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bsryrojg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qomejkpd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mgxdqgyp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wrexhatx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3odvtugjf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ufqupajq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ypzvexjh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvzdloiw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jlqceolr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byyfhrfx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3juxabhza.html


<!-- 参考信息 -->