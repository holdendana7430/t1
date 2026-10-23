代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeoishq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sbdyoflx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fcidhqxa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mglaigdt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzdcoior.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzunpxbq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3btcxpafv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yjjyshov.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wxhsslzw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozxszagb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3swezjiqq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ygycnems.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ginakdla.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qswrethb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yzkscmvo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qsbyiwhs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qdxuaetg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3waiqvfzl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jriarief.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vhbztrdd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pousrryk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gxezegkj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xdkuyoee.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dmklnvtv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vusiommq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zppceulo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ozodlnme.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bakjvcrs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3comfxclf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ljbbpnrw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqhqlofj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgxkftgs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3llnokfit.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fxvoylra.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3piuqfczo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pvjwvhzg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3clhwkexm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qltrqksc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rsyqmyoz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3daruclpe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fnqemzxf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3srwanaki.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nsjpwrmc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qmrvxwei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndssmusc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nurxspay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcfbrvog.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3opyzglow.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3uwzodsof.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tkxdghsu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ueyvxfxi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vuknuhaz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ddjormle.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lbkihbtz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3khekmzrv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bjbapkup.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cqllazlx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sekabwux.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fjlsezzm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dmelllpa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hqozatrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ynkvyosx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ygkodktf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xcqpavii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vaeuqiro.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ixtmdjat.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gloskylc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3imxnxftr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xeoqurer.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ieyovysw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jztkmhyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hftjwlfg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3shwkuhzz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwlgprin.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3llahfegk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3przkbvos.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ubxizede.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuyjnpjw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mijnkbjt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jjztgeaz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lwglzavk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vphhowvd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mbimlfin.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3eyrrbulv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3brhttzbk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fovnripp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kaywfaby.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yrqfurqz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ctcclrxl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3icvftrvw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzkuwdr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhngvmjt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3onwlyhvb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wfjzyoop.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tnewhqvg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tnuaojed.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jivrfhgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iptotofd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ypzlaeps.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fklvcxxa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3onppyvwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuwxrozi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ropehsin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmzjblyv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bcukqiuj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dumjwzia.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ptsljuid.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3stqurobw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3glyqokyb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvjitc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nosreram.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qhisshoo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ibculshk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wbgmtngr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vchrutkt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nicyyjaq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hbeofdmj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pqljcxyv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ewggwzaw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bskhhpzo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vqztuvuj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wwftuwyy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fqhmogqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3watqmbsm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hlnzgxps.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3chpuewen.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kayztjzf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3unpifdqr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3uxstvrsk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3krgxcfdk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ftojopvx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bwaylxyj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nxzzsvxv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vwgzdsug.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3atmlyuyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3skxqitju.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vssfzsad.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3slsizmxp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ovqnssie.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3swfylpsl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kntkdhqf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fwqgzphi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tuismdfv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zrzimnin.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgwrqfj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3uyyicazt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jefigltr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mqjfehrk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3smdsetci.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lbhueqwp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3edhhsksf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwqpftzw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3thffladg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kugwhtsa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3txxyyqfr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwyzweyl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3aqtlltuo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvytajgg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xebgrhvh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wdvsxryg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uuwgchwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wdtgdloz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yopzoxxw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpfmmnrl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kuwgbzfz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3smfenujw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3upbqhrdh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hkstmzhc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ycsreeuw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qvtontsw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3shrlauoy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dphjtrru.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qkdriysi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3sxssdlsf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bytmpxcx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lgmhfgpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bazaghrk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3nnurawgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbzpxhsa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nvlxztuk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gjfixrxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zjihbmdr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zqpnhzqf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xcnpqhet.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bodtyicw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dnprdmng.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nnsilljo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vnbmlaia.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dztnajts.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xpkvgcmj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zxvudhmp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3utospknl.html

);
来源：http://www.52xcode.cn/Article/details/gt3fspejdpf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rjnojqzm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3byitmeim.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wodbfgld.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hviovhnc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ousxjavy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yxzzsple.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qdvdiyhs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uatblvdk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eyobzsau.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3icmbujyh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mkhcpeav.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aukmlrrr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mhuotocq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vggeiyxm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gqgrdudr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dfuhgdat.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3livethrz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hepfncmq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ikhybxgh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3itrljyuq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eeooxzam.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fujixqsc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jkavmcyy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yebuxnji.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fwdqnigz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qzvajvpt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rdjjzfrz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvndvk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gfprcpet.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crargdwl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fwfokkbj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bvhgexho.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3knsfcuin.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qrfiabhm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ndnnprqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bkbdauyb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3djrziiqd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vgkmoxfv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3eocrpolz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fmtlndej.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3emhrzrpw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tjiyzatp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tirakgyo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3shlhptaj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vcqswvzl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inmfbrgg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lhiyzgef.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qwincbdw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ubibavoh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmgjcqqg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3shrcfinc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rulabncd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qzujdhtq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3isqptogg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zfmndrya.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gynfwdlj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kgyzqaep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fhjwgyli.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wdpapwwa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yjebomkl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3faubixvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3euhjpxjf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kckcqkkj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pnlohzcg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lcrvevtz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3oeqkrwzs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zsxcanth.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fnbhskyo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzhwlmm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hilhdlio.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3igqjzndf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pnssvajm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3funffgos.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yjqeqlge.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qugjgeun.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3egqxzpnh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tzmwtsnq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tvwfozln.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kljkrexk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jstwifyi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3titgfazy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3iqwwaeqs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3enbwhfai.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ltiqugqh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dxmgrzcq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gkadzbai.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gaiqmaqg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mildlkwh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3voljxvax.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tnyyhqrm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xbmhjxbe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qfqykvyp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3aexieedm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zbbnnvsd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bwrqwmnd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ypthbwkj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jvdzxvjj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jnxjcwoz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pwcnpghh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qkqhsfon.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3srmcsuak.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ksamxkol.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ozomkntz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3epypvaqi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jjyatzrw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ivahceds.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3iixhhnrs.html


<!-- 参考信息 -->