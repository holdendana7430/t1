代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ziufhwpo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2atdruxbn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rqlcnjyy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocorzegz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypvvawdh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecozoewj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2utuxeuzd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fbthqjtm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pxgmvufa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hrkonluv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oocqjgge.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrybxgfz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2iioyadxm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aeqrvwkl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ljutqpoz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uccefpvo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cdmsogvb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fkkmdlqo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zkjcttmg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bfakhfqa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tukuvpgo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkixlqqs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ojwgwnzc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xjnldzhs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2eonerpol.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2otbohkhe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2waixbxht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfbesfqo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vygoqona.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2opkukcog.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jolbqfuz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfrqnxgr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lcxhusdn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2afngqwaf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ciycwcwj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vpwfwxsw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qrikznzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2elpxfnax.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2aoqvuzih.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ejdfgrcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqjvveow.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ijtpiact.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwjdhxqy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2chjzjqiy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eceiygbb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oajsymdp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lwwtrsgs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yfgssmyy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ounkpfea.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bimzwktu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hlpdgogi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kvqwfbgu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmcgcmod.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bdandgtw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wcyrvuqb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ecpricqs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2axjyotha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2othxxqya.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vbasayml.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zhhbmotj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eezhgqiy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2drjpilds.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uyytxewb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wbiwkbqn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eytkopwc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2avgnfrec.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbccxahl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lmcqkden.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqqslhx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhamcrzw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fwethtto.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jqwvajhq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jvkatjtd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ywwldegd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbcwcdzi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uicojcrd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jyeshjgs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ndhnytlu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2duyigtjj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pzqlvwbq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vkyprcoh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ioxumhje.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqtzdad.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kiyekqui.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sqmrhkwt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nutddpwy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sbclbnnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kjgdiusa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2svsoabpg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bqexxzxb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2idjhulmk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pwsvmsbm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jkvtnrsa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fnponsjg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tkwnejyr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lomiccrg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iitijslw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkdakumn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ooodkjbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thoiaduy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dbzcsmsu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jibkhkft.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gldfjmwv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nxmayyed.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2llloryab.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ynrhqbxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yqvfzyav.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2texczton.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2syjalwze.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wqqgxgpb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2shwwjjzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qnvosiaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gmpiyvji.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nkprtuoc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwerwaj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xcuygcnt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsbjncmc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2thlxaler.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ogmjvnzb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pexazsmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rqirfunl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njutmbke.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgxiwyog.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qayvdcmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xpuzoryz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lztnymxb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2junrhjuj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aebhwhkm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2npejopmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2noqhpnba.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2myqrhqrx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xflkkzcp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mycotkmk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tczawalw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2oelwmdms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2svrklgfu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bmycsqjw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nmvqwhur.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lzbsknln.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2boundvdh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dppnlzrd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xrjrtpto.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2znmqulhm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2himxmbht.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mtnpltsx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ypuggkyj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zyjmwaah.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2itescacd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2beqjpaov.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utsrnyhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2txqotqwe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgxhrfde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vvosjfjd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gkmumork.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pkvjcptr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2twshzpff.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgarmpnc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qexeapbi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2khimxlik.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rqqnlcyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uzahoawy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zydhisfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ayqihbcb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bnkhbefv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zsizsjca.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2awkjywcl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ibxtxpwx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkhbofu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ndhkclhq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cglwdoej.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xetcimvl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lhhythpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfysrdey.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vurepuzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrdkqrab.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ukkehihk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wpgwwjsw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xkvycykv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oemhjhhx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fqojgoew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cvpjgdyx.html

);
来源：http://www.52xcode.cn/Article/details/gt2uyoryowo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ntcqksvz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fgboxtsr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vkdrnikd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dlsfpyvj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fsdcjtzt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ziotfbko.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jonxjayp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jklomjde.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2casehmto.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcvblwij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vltbsbvl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yuacdvhv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gphbhmru.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cmhtqfhg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xdbchftj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2asblpytk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ojwyzxfs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nxxssgkf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjlbcmb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2orpexsqf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ympxttfo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ztzdhpjz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hpuwdhly.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sbsyboag.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xyeyjqhd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gjbuiwsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xuopvvyc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uglzvedu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2aowriayt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jrkohajk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tgunzswu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ykgdjcpi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vurqsppg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2nadpiorj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khpduyms.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2inxjrpgt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emujewad.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqsuwxuw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzyfsgo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbinan.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2irjcmsdp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ehsgxsoo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2plncjljq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mrlwtexi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2orphmkue.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eyzuqtee.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2viwjgmqp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2egkdorqw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2toioojvd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2grthsxky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2woyvvskn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bbqjpxcg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spdkbgsh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vypusgrb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kefaubje.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rmfqttzc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xthqtrkh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2iqcmwuno.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cshyofqm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hvxyaywg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zfzccygq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eqtntcqa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ocmdkcvx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2aseriinz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pqrnxlgg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2agphryng.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wlsmdory.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2saldjscx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zliirdft.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rcuoqvvt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2deyfwmsy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pnsdymay.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wuwyaegs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yzqupike.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2njcghlpg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmirayer.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cnpvtbhe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hqdifxsl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hhbltgga.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mzfxsmln.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2omrgysfi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qhtywyjl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rkavmkkm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xsmgwdws.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jjlysocm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2peqibzgg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2aiebqdud.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lohxgexs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vmapemro.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2doflgixh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xpwituoa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jmrekrgb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kwbuggmg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bcmxeqbi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qndygiue.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gknsaybq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yfzpjfek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2inklwhso.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2iowmhntb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ogxrjlvi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zumoksjv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wzfdfguw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jxvfqzoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bhzjjlbk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vwnubnpv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dvenenjb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nqdbwnjr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2flzfrlyd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2otmecidu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2eybzkjrc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2stimvgba.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cxhemihu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tmbcrmwp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hixkbvth.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydwewzgp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fzawrxhh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2japbbumy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fwwzmluf.html


<!-- 参考信息 -->