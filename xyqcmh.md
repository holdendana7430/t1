代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sydnufqv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lfdelrnt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2brbnirqn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ofbcgbte.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvzbbiac.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pcecnawt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iokoygaw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vfnxamjz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swfdhvuo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2esimmffh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qexfcmri.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bkqtskxz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ufyxeuam.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mumpvwpx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dkbwxrrx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ddjrfruq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cxtcuels.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jxxqreor.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vsmuenvi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vuokyblq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ozfwyzcy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nosejzjx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wpvtbabb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbncmzft.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2opvgpvnr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dfwwaefz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qrkwlqss.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wfprrxbm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtsgvaj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruelndma.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ifslgesx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zomovtut.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nzwscdcs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jcveigey.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lxlwpzvy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ihzratmq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2teqxgeyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tqfftkzm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bagrvibn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ophanlsc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ghvsubra.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pxgkrmwc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kidfxvck.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yvchbkqy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ftrfaxqv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uzcsngrt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zecacbzz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zrpxzjrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxxqxmij.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ofcaaekj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyhffuvp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ffavqtch.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ukeiasna.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mlmncijx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tvhwgiiq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hddbhzez.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hqwtvkxh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nevmiyhi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lqpfarom.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pgzxoqev.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gziuozax.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mxinpwpc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zuagsknb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cxttzaoj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lkojewpw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2emxntodx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wqpwfxuv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ppmnscku.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mffrcdet.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wmmajrvz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjtmgfpc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2idvzryrz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vtzzysis.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qmiipttx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hrbhlyif.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2osndteua.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bsobvyrv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qlnviqel.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gaopunji.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hnjmofph.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pmdlfdgk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amjjqtdk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cljmdnvs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cjkstyda.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nbcykfpa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xjlahsce.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zgbrhajp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ctnnnwaw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xawufine.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ritxuweb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pazspjyx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jqrmujlc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jglxkxvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ngbrabhd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zppjpwsb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ztipgkpf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ftewlaqw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jbvyrryh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mwxtavgw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ryqxoypy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yzppuklj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xssljsly.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ryoslcsi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2aczoqlor.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2bqtjwvox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppizikec.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnzrxyny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjdnddxx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ajzksanw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2whnelqfs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dalscrlj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ouwsllhv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2peajfukh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2meglviaj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2uwgzooiu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vhcuvcwo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xdfrktja.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kmpjcrua.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2oeggjpja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xuiivyrx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hcvgscfd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nobhmucx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwhzvgv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pkhnjgpz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2whvjxtzp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wqmgmszs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2plfuacvo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vgmwulqv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fcyhhldp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zxngnkll.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sacfqjhf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ymtygmuw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2teloakvh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjdlngk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bdvxqnra.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lotrcikd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2luusavss.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sybaorhn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fsdrwuhi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wegyzmwq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wwmxsnsm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ollbhtzo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fpycjwkb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vzaipstl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gzyipkhv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gejntpxr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lclqnyic.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2spdmxknc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnlhfbti.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2klrlbfmj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2taumtkas.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cxoeqpcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wovokqgk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zftxuuqu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2agiolrkc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ksmgsrkr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2womqocms.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2njselhnp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ytqcnzeu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlzybhfs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2sgleudfb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyqczren.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fntgeckf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2oprhhclb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ynaucwwf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rfzzonpf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mmgdqvdt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arkleyrt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gefhqpoj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hruvhfui.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2efmqyxrp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kqssfeoe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2alwfvmck.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fqpqiblc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bxoqrkfc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ubkzuncr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jeiuilqw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2iptdkodt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ilqizenx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ocwifvch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppenkfwz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zrnadvzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bobrmlvs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jamwdqbf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nrsrswxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mrgscvih.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dcjsmdsu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rbflnjsi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dpxyxjdd.html

);
来源：http://www.52xcode.cn/Article/details/gt2zykuzthi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zwzxcnmy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nrxspblw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rwcfdpqq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hdqzxuub.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vfixwycx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hbzvwxvc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hsjxbkkm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xpnwhaap.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rysfcrdw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fovynjpg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hrznljtp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bchtqptm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2btcdkawr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qxesudhc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bbiwgpry.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2clhyahif.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bqfptrkm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2figardrn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nmlpbfya.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2czytiqbw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2azrckumi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zupkybij.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jpdluows.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dvljobpf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cdjyhbfm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2drnvchrt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yobtfdyn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2knqjdqri.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qgiymjei.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zwasboxf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2folykrig.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hxestbhf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nraczxyb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2esbukhsp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqviejz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2daqvoyku.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvvfjauj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hkrwncll.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2trueonrk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sapjxkjp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ihxdpcyi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jvyjxrcy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bhiubula.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2thjgkgzh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jbndoche.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kjuqdeut.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yvwbrutx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2urwibsce.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zmadefwf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tuyxaxag.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dqtjttgi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dcojxxbu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbhocfrx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fqtmekus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxldlt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zkgsmadl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwuyrrcv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xemodqrv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2upchawns.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tqicsgbz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwwezunb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vseufadn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptyjbqum.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hpkfewhh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kfzrkkpq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2njdmytko.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2shhfauaj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fbqmbekx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pflokfbd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kvtrnbhr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mbognley.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2axfxlvah.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2tfnzbvnk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2skuforac.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tpnhnnfc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpjypjcq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cywqtkjg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kavidivq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rnyalboa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nahivhnx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tkycxnmu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwmigkwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kettxxje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ztbfewqh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cyizzasq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lzxaxtht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rjhjriys.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xdpqdppp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2olhmbqax.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ijlxszkj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2danvatse.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vkblzllr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2unzsglmx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ngvpclma.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2renxnjzp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ckdnqkof.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2obtdiodt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pqdbjagq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2izqgapba.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2djiasgcf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dncatizy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2opovmibe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gqclvvlj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hfvpbxiu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jvrjerco.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aiuzuoan.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cqlqgohq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ojxfmhgi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oknsvyeb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ofzhxuoa.html


<!-- 参考信息 -->