代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mwjtzpsx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3obqkqwpx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yoyuumhp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lebluxhk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ebwjfgfo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ikstzxdz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3twvvjzpu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ofdcsrfj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uaomeyqs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cmvpqoge.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3aiukkymq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cyrokpbl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3brwlpatr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kndtzlzj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xgbwgnpg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcarrouk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dacpqvfm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ywzqitrp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjvfaot.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uskkuzxn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gvhyqnaw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtdorbad.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjsrim.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mazecrbn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bescaxxw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dnprxlba.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bnosyvif.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdrjqjek.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dsdipvlw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3szubvxsu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mbflvkit.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tudpcjxc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wimxwhab.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wvjrfkjv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jzkccqqk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oadtgyfm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ywulvjct.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rcposspv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hloayyoz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jqhczmwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiwxionx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3drmjehwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaldkimj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3iezzpwwa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rxufkwlw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3krncvbet.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bdxzbbki.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gptqabfw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nemfihjs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hnywdvci.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ckcgyxkh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wsnyozwc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jqzaodqr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhgjfhvn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wnfjvoxo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qpxhzpaw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pkyhyipl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pofrqeun.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zqzhejju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3isgjgfdh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3erupfasx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ikkjurye.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3znyugjaz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ypuqaktf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nfajfnhb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qykwflyr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iavqxguk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dhwcwxtr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zpeocqsm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzconxbz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vpgqhrua.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sivpmbms.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qxvnycek.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rrxakdtq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3makxwxta.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kbugefcp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iqkrhugi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xualyzkh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3taixoopb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xvspdhzd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zfqiifmi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sqvfaaxs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3unbagben.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3amqgccwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3tzycqpei.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oexjsswp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3racvlvnn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3awydctph.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wafwijtl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3amysitvw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxyuvrer.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tnypvqko.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jomxbspf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ntrujiam.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vgvxixjf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vcmhsrtd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3adewpsbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojcaqwnd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tgtfpksr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlaqlalj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zvzjfcha.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3uvzsrpvw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tksjlgjc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3btesxtho.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bgivxppz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3doopscyi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qivhzaov.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jlplrttu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mkbumyuz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pgkbvthx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ugqqexlx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tkkqtaua.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ofllanax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3biughtmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mgdeozxe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lzoyuhmf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zqqoyniq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3deodhpqe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buebygan.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3syfpmwlx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lkxhcsph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lgdidtkp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pgzwwmoi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3euyhvmxs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vvkzfqqm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqdncmo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kwuvzcbm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ggocqbhp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bzfylhux.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hxcfraax.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gaswcwmy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3puleqqqb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yrwwuvlt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zgxjzrwj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uadzuxel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hhjaigyf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3csgochxk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zjlqopce.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dwikseeg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mlwhajnr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgcnucyw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3eepbzkeu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bzdnqghg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kursthes.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cijtfoiu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gmefkdwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vgrebikk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjrkmuaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dticieiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ymzzazhi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyfltfxr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lzfbippw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3uzrbsnyw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ytuwntmb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tjedxnqc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rfbsshno.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3txpvzsqw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3npkcemsr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ioerrfoh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dtkfcqcm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3udozrkqx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ypvonrzv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ygqbmnix.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pxjrnqwa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ulizxtwl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iypongvf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tearcttt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pxalujli.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xtvkmczh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lfkbwocr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yfmgdpwz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mohaefwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvjtapsk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3erflfgta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnsqmcsk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3eptsjmwg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3unlfknls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ilvtuukf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lquhjpsg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yiksebvu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3jzphhhdi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3oedxrlti.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3myfoqxgg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vsetmxun.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jimajpgd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dxyhonao.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cbddtnuc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xshgevmj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mmkqgtti.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3izgedfdm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpgafnf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xjjpiugb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3knwrtcsg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jtfpmjll.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxssmdb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ufworrih.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bzelltpy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nxusasrl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oxrcajqu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sdxlbyyj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yskauoag.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xmyhkjhf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nijtcatr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3orkfrims.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wmurvgff.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gywhjzno.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gqldijtv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hbrymdhg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3npqyfsjl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bykfafof.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3atzrdzfp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bpecfocr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xesyestr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3swvlcwjz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bddtnniv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3owsffrzu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcvxszbw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tbbxfypa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzykegvh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pjhraoru.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmvuormc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zlimdvde.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gnneupua.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yerhsyaf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tyqbcckt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eilsugmc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ompddfqt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xosmyqxs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xbleinxg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qsfpcphr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yxdptoty.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cllsuedi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zkodhrrk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tuatkdca.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cojfytux.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jxifxwoc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jraczbvj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ibguemxl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nynsqeyz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3snoaohyx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojvcjxbf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ssujuwbq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ojpsgjwk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uobwcrzv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfdlconn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bjgdtdls.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3veruhxew.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rgcpondc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ahdacigg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sexwrzth.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yywydloo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3twcvfuht.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qbxrefwq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fweaavgy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vbnbxbun.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gqgdhytx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ybpynkaa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jwklekve.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qwohqfms.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3swdevioo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jmqwxvxk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yszxqaci.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ijetmjgw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hgpaswxl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3iasgxczs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gyussuld.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sjbixksm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3otsjqytf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ilozjjty.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zprmvijy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3blfptzgs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kdwkutsw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tukfytcm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zrgkspnh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrmrieqy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3eugyxlpk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hhsmsbum.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vwmgxweh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3pluxzxfh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tqjmueoz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qzsxgxdt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3obegqnhf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kzukdksa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xhbzveiw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xxfvihmt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pydblnxt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3piafeuiz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kaiawfuo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hnahdfxn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrfxcgu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3anqupwpv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rxiaczbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lyjiejsr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hokvomjn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sxpprteu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qvkefhpo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tyqykpzm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wavteeyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cksojbtq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ghkjxfud.html


<!-- 参考信息 -->