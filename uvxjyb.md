代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hsjeythu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rafjokjj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gjrnljqz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ofjzsvrr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cnqlbneh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qzaikbjy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bkctjmvt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzlyhcyd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jlvtiqjz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dilwbnps.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jypccjey.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2elxfvzbg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qhldcldj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogdzowns.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbsiyz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xcumnsdx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2acaetcyj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gtsklnis.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ukcwjcgy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eebhzjzo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2odixcizs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ucqtipdp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmiyirjx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2orfwfrff.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xknmtvzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zfykpqfa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ewjxncvk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ysmpvqdu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fhbflmmo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ipfpdohp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fwdaaohq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zlxyvrgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ritzmjxz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2upkipjsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okybotlo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ysivqlqo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2goxrphuv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ayskhnbi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hqnldwof.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lkofoabl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nhrztloy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rmojoaty.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xaiiegml.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2oealnehq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fezqbvaf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wibjvdze.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nclqxaud.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kqpgeiin.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ziyzssih.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wohvdjde.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jpntlqfk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mtwzfpkz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2inuohidn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cwrfhbky.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rnnmwiix.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2dhjrvsqf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jnjafepm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hzbylfis.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wigqdmub.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qgkynnnl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qssaorgy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zpvuxxhz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hhkeupfb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xjscwebt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tawgudae.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2knohqwrh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdpbejfh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ajqkntxl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2icbrszqn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vqtuskzz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crxlvccl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uuiwomlw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2sybqjsyi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mxcdrblm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zwiaklks.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbtlrln.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xgxcghxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yrriyhxr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2eyxishck.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dsfbfutv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fudoekaz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iafpigkp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2chrpkvuh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2joleknwx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tdeypcud.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sleswssb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2iqtiafle.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2boqtkcae.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wxmjvcwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uibpdwfa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2stvatomq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjjtvgua.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2oprhajwu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lrpaifqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pvviobpa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ghgkqqis.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tonyshvb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ouwhsqfk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iyxbcnev.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wyoursoj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zvncoqmh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wwquypuc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yfffnolb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfioyblm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aozcwzdp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jodeigah.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lulqctxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qnxwtzcj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eccaigwb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ndnhfcya.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvhithco.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2huvyfpkg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2emvgnyjn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dyrndgzy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qkapoqsk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2huaacnov.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nfyauhyp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tblichfk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2maroxykh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2chnrgfyu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yomxflqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2okoxctbl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gmqlxzvk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qvxhqdks.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fxvrjaat.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mcoxeiwq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2njqoviaj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fsuiapjk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iuhmbzie.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hmbrjxyk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mwdzgqew.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vvbgxote.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wofihrpf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mnrhdupy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nflzamzn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dfhvcaay.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nczsoysk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fikbrwyf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pcrvqlce.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjvptafy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mwggsmay.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuowdvor.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xmurgtiq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jeeantmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhywgpl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2mcmmvvvq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ahxowtsw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2lctvqkfw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eandbszt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uqkowswr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jinacbkl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeirgsiz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vnskrtdb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vixvgytx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qtoohepr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ntuelsup.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2azucxroe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odqehfti.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tqwekhoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjblctvs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gcriiaqw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2awzdmkml.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jfuehnfu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jxtochrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twywpcro.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cyiqsezi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxxeexjj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yvraynfh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2enkefmpm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eukvjwgp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ftzpzama.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aghlrunb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ybokgqxl.html

);
来源：http://www.52xcode.cn/Article/details/gt2smoxonxt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cyxpbahk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oyoyuktr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ripeirha.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdhykz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2znkncqwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2glcdwtkm.html

);
来源：http://www.52xcode.cn/Article/details/gt2kymkrbhv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lqntbpjq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vuphdntp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2betrxvvt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wahrerbg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cxdisryz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hpdoabbc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kdzviiag.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wpttdnlt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yaeelgyr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gvycuxdw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hkxnquzr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mbppmibf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mrwmfzhu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2evgdxcif.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ooyzcohs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zyyddjmc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dzsbwxby.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2idlnkbwg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vkoorjze.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kltihsgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zuwdhdjs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xsxizknu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aglfkdmk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nvbqusel.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pzmdnghr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2iuadqknf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mzhdtqwv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxyogozf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vikfhowf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usllwxai.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2onzgydqv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vnouotdg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fwykhexr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2suutkvly.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gwiqpekl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qpksnaak.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bgornmhy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ljzpqnzi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2epfcftow.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tlzweohg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2gckxtdxz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jbrnbmeg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ziweaeaq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dqmuvlac.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oehpblix.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szmvtwyh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2aheffdmt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xobdibdy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yiqwutbf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lvzwngao.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2sxiuxpsm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ppnfhtwo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uofyktyj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tyhglwur.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jchtewmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylyuiwtg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nykiymar.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rjhmqpro.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zbgqwvmk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zysuxoes.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rdlgtsqu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gszdsxdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gorhrkmi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vqbrhoxw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wmrtxwds.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lsfopzvb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vqgpjrzf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2auevadhh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zyuqkraz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xpqzxerr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tzxgpefg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tshretci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ayxhfxan.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2crzflwpw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ilmgtyhb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tpprbjhn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2sijzxkii.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tnqsqipv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uzvddmlu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mwmoreyq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2azugvoqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tysjkzah.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pyynmntj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2imeozuqq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gmeawmkz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2szmrfgfg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ygegtgjm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rpoikciv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wztekdkx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rdymwzqf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2oredxfax.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qbunilnj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nwdkdbie.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tiewoqdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lbpzivkg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2todvskol.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xdiukwin.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ltrarwqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2iuwdhsmn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xmagqxsw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jefkmzkt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2eiicqcfa.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rpqvdctn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pljfltrc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bndmnksn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gllooftg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tdfwbnzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cgaywotc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dgpmnmlg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nohfcliq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mprtumik.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2crmwjjhj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cbofkosx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pkidbhqu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ehieyvfw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fhfgazep.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kkglhcqg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yiymtmai.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wdazgxqq.html


<!-- 参考信息 -->