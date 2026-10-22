代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vdkosaek.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ncdggmix.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kfjplwyk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2izgxkize.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2daagjgkq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lfpzbwed.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lhmjncbw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iydermaa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cxkxwjfa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zknuhmsl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2bjxnuamt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2htuwefwk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rfuufnet.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gjiyeuns.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xzopjhli.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqwpiccp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zhhqahvb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ilgoxcdf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aswpzmak.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ibasyzag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhkpzio.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wbpdizdi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fpbryiyb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ilkedqyx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2oehstmor.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lplgelmr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2umfyfbkv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2reregewa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlnbny.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xvlcivrn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vkwlzouy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fzzzjuzr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sjakjfnt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vqzctyio.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cfgrxdfj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2osvciaia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ameuazxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2boznzaxe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kvziqtnc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fhxihfxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lonbsqzu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zgmghdoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgojpwye.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ecyyoqea.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ynmorutc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tdcjlvzs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2guiidkld.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dbsvsevr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vvrvkrvy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dvstkppl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2djkasatb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bhgktioe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wcpelwpa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bpjdqyie.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2geanopvm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2emruqhti.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cxfzdlog.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hovbzyad.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kjxzeebx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wrmnleaa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vnlzpcyx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nnnuhnab.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cdtyxwhu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2czwkyegl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2izzcewwn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gxzinscm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxcsiz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bthlnuzx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2svpidqup.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hinkdrjm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rdmkyhdy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nivosqey.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pjraooqm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2resonvxf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xjqpmdng.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dlduatci.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cvzeggcv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xutmlutc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdjipkh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kqijstps.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ooleruax.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xqajsbvr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2smzwgbjv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdkpnot.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hbccwmlw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hhjlnfxj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hxohtyyh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ucdjmsij.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fjmfkhvd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2usvxzniq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2evrfajrf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fnrjpzty.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vztwbxbo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iysudvhb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nstxhsxh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2amudncbn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uaanpkfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etdzzcnx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lovvnvhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfzwgnme.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qsamemyh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2szywbedc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hpvbfdhk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jklorroz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fogtyxcw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ezhorwsx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2anflbmpv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vzexjxqq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rzezzbiy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2quocpvtn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tigqxztn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hffmyvff.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rourhryy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kubddqgj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vhjqxyte.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yxwgewcx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2eovqokns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ajvmzqua.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwabxluu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fdkmqxip.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vpzkcmkb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2enupadrg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bfsaeqzq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zroccrbo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjjfer.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2azyeaapd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ogpylxrp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lurhsnqi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ldjkeenl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bfilcrha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xnopiiom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lczrozzi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oqlsaewm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zozznlyh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pgjyphlh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qyodstyf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vvrpppnr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2geoxyqsg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xlngragl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2eoshsnnq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfaiytix.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mwyufhff.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rvddbkwo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gkavlyus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2honnjvgb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vwigndwa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bgyoplqh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnojltyv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qhbzurzl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbpbrtgd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2osexjrsq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwhrsuod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hsaauwun.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rqzpjimq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bjfmhjmx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zpgdlzpt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2iqiuyeix.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ovnrtlxq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xcjizzop.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zsqckcav.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mrdcarlh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xxurwiji.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2dlfcklwn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2eowubbwc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iqqhwffc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjdmiix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vmceayxj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2swqlmdsb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jewovkln.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wndjazqx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mydnxjtv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2oyypyyba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfdcljgk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rhcuwxbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxqpoije.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mlnxdtea.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kjxvzyxe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2itwcdgdu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hlrzkdko.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hloliweg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ehlypzrr.html

);
来源：http://www.52xcode.cn/Article/details/gt2rkvhjovk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xgqgzrfb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ysjhhquy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nocrksqd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aejykrhn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vbifmwtn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fnmdyvol.html

);
来源：http://www.52xcode.cn/Article/details/gt2tekppfsk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qbdjpzjs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2apwuekxi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vucrtkis.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dtvzhvlk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vlsoytjk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpdlibfp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kvqhozga.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2frnwksid.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bzyqtcjf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mmbeioxf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2miomfqrd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hsgynpch.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2uyjbzbgi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eqocxhue.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2urdsgvab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qkewtzxr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lkobccgt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hvjdypfo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2akurwagf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gswakser.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dkjukjtx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fomgbzmn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pnkxkwqr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mfgewlkc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2akzrvlby.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yrcvgkhp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xbecqxnn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnhchrhu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2oppvlhla.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vdclqrvo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ypegizqr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2marykold.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jyhaulqo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2znxxrqfm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2awupkcsi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bzfdjwyo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zzfsmwnw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2izemozsx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uyrmlvvj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2soyhzhoc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nzyfiflb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pkinzqsh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tgfnrecs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fbrvvzca.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gvpsxbeo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkzxlhnc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rasfjnfo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yhkknsnn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dipqcwbq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfttvtfx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wcimpqox.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xwvrhrai.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2avsnkpda.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rsjwdeqx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tsvibiax.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxezwddq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bwiinwpa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wnywxoon.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ssjofjgs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2izqbvgej.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xzwmobrs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ywtcxpsd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wfbpwcjg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hiefgpnf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2arwtjtzg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mmnfanql.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vmeeznjw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zeatredo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bqkzgpnp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2oklqonxn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mpgqovlh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tmmdzzzv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2synamtwd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2guixlgeo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jiqdrzrm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ctjfeiph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdfxhnc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xqvcvuyj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hzvarrjc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ltoddjme.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2grlppzbb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jhdpihhy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oxruaosv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hogipbdh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxfylt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sfbmumqr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qzkkttcg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bgzbputp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bdlsucuj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rfbhmfew.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2iisybskr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dvppwcdb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lwugbvdw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ozuefukl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2loopbzrf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uoxrjiwz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nryydeth.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rxwaqklj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vdheyfqg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2iqsbevmd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2aafcltva.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wzdclhcb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xhmoyjxm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ryhqcihu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2inwvkojt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2igspzlhi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2oedptsmk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnwpfgie.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2owcvxedh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gytymlwy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yvgimqxx.html


<!-- 参考信息 -->