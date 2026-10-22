代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xchzgbwg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2iulckutt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2errjfcpc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mptpolel.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tvsusefi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rprwazqg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2acdzfyyu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gujtowqr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzulqu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qvamxubl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttvvtfhv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2imajsukl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qxamaoin.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ljsbdupa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wldiyoob.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnxveygi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rkyrkldh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vcimbgmg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tjytjbcg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihwqyczo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2txhzxqpz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2igjttxpb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidgylbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2prblxhbc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vdfblwqa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rswprarw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ulcpgpca.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ntrezrpd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uavhlvig.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yvegsegt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2olzbrorl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2moriokyu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dethedsi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bplxnemz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrmgpfeh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2joliizpa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zmutaxyi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2roriduou.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jztmyzvo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uwjrjihw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2odzlahmu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2izqicprz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdffyvd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gbsrcmkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxtdhwvf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wxysvtkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwpyovwo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gcegsbrx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qdkblxvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nhooppgf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ocfgsudn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ktxmnfkb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mlbnwyof.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2amxrkkhq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ubzxrqfk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jsfutwup.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fkyxicmx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pydvftcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nwgniniy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rrztxdcs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rixsbduo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdtcxuo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yvkjauvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lvpnxmce.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2humkfrmc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2iqetolrz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zhxfpxgr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wohxgvie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2aenbcsoo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mzxbxdzr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zemzmaih.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nrhylvgn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bfyzyaga.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2koivrypl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jnvypobw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fkscouwh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2akrcpyey.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ahdldfcs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfgbpvt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2creueplg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ukybossl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kawbhhff.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kjaydgwk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kddispou.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwgxvji.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pxjgnliw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dxvkwbqd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2irmtwkrt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pitxuuzf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fcdwwbmv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tirsqvqk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mynovqha.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mxnwxqjd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dxceugtt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mppstark.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rvhnmwux.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zxgllzbh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tudtaiha.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ycsuxtoz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iekvygkh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jwnlxcfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwvodwzh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbvqdvdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxsbnaqf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ivoslomx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2phoxakyu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gnqgpgzj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rilehqnk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jlbvtfnf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2thtohspi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wseqhprh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gmtmgfkr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2raawvdzt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hzvryrwj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2weacsowi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xijvbzkn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2obswrxmi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sksxmbfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esfiaqcm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ujwrkzdm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dhyivqcs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qbrnrmuk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jvhorrku.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2errsjmvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2npmpklor.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ntviokym.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rpperhhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2akcimzor.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bxwczcfh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2abpfxvcb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mrabdogp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wshzitti.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vtwsilhs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2csduzata.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mtmdsbtw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ksexsevc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dvfvtrnb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqfpnip.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mvivwcgb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dntdlakh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2divzagqq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fnwngtyk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vprdtvvg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eajacocd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyecclu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pmptwlik.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqvqnoi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lqtssqrz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pjpftpyu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lewihqjd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qvufoicz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kupwsafp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zmbtglmc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdnhyltz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fahixjad.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ljyuzolx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2oeaompbu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qsfittdr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pmzuhbzq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iqgxlmhg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2sjrwavqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xmhtreij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vpqcfaje.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jdanqapn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2adbjbmih.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2eiygorjl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nhkhmzmh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jctbmgyn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vrionaan.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lycrqtce.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xjihkhoo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfzypbh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tdkdrqhk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hsihycoj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gwkusfhy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2juoxikhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xigoveud.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2aqteknhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jccufilv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2scjegxbi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nvenbjxq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zyjdltps.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gewskzwc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2smgewdlq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ojcwvddx.html

);
来源：http://www.52xcode.cn/Article/details/gt2cmnizido.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ckxtucho.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zrbrixmi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lkfqcwnh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yzqmrxnf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mnlfdvvt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qudkbskw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oggjxcud.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rghkhjrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dxlzqkbu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2iuiepveb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2recrkzvx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pzdvljnz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cgqdkvbh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pxlvclnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dlhjmlgi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2esymjigj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sduwiwuh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xrjyonbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ikdjuavy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tovvckit.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2luuehwsk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xtowzvzq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uwjbjjpj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bjweiyen.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pvzykmgl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jolohyuh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fnzadgvv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ypwtebqj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xvhaxcfv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vchiiiaz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wfaprlnr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lciivndi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pmxoodcj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vlfivoyd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zueprqtz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2envevuag.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsveleir.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zsrhbcpe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rmphnvbp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kvtdmlrv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qupttpmn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ygaaddsg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nnjziour.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2umnxmrex.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqnxbqno.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kabvzjqq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lxkyoggd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bxvanwdu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2easwdouv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hhzgyphs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xmwjfuen.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dgxtcpqx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nxjkqloz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2owxygqwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kmsqzcbd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fisnjaug.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmyjaqo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kwdeaoza.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arivailr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tesqudme.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tmgtprhy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rnmlaaka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkdrkolv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ctwpgjsj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zmqkvwli.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tznexzeh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qudqdlwb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qgbdymid.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ribynbaf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kmymaamn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wlzeebji.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ivwkkjxg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hectyqfb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zxkxeycl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2plhiqhtx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2azhfvuua.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2blqsqewr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xwcmaabe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xfkiuvan.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2exbytkyp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2lnlpzhcr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2posbivij.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jktsqtwc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qipfmjlp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zeitbncm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cygantqu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bdwjnbqp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2docsvrml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bswkndps.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kjfekmce.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vgfdluig.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qfkznhey.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wghnrltg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ftqcmobk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lmufpoxl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ywoloirv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2updvrfdk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ahypkhwx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbcgkgqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kxtxvfra.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dfwrofuq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvaaljp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mwhutdhc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wnvdcvxs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aluizycl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hqffwhak.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2stiiqlft.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsophxt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mjyirntb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xsvmcokm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ujzwximy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2psgolmji.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2icdmchqs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjovoklh.html


<!-- 参考信息 -->