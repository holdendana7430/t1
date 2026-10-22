代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vytgaqkv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bvtcjqsi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jpkgixgn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uqcegjbx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tkfbrzix.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2asctadzh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mdaekqiq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jxygvfky.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjvlgdq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sojzjgoh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tiedrkep.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2krmdtlvu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhplniff.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2okvlwmko.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2emosptmu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pgfblfcs.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2exstvzod.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xekhqvyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecrxiajg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebqlkjdv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sufmqavp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgijuuhr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yqcfhhvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bienjvaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fimghpsi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pwtqkshn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2clnqcwqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2skqdfozp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtzhhwg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2omftjpwb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvzrwze.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2obfzmlub.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2sucmiuxy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhgodpwo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nubudoej.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xrfwsavp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bmxkqyrv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dutpnhfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jaqanfhm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqarmjyj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2umpnrcet.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zwgplpks.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bnundsby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mvonuitt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hifyeppv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yhtrdqkz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vhikqwdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fagxwojh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bdhnfope.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2thdrwydt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngfxuebh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bqvxpmod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdpordpv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2egofufse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejaskkbl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2clpetkej.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2azxfenyh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wsjreaxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jfhmmxvx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2icevdugd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zuikvtqn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xqrtwmgv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yitoloaa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hpfnjueb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2repvhbbg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hyrnbjdq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2clnfmaqb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2troiwuhh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nkqkjjbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jnltbsxq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ejzanowq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ucborcgg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hetpgeup.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sxcghtwb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2oakwdvul.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2evxwuapd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lnriqixj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yssecbar.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eevwxyzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yuulhucb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2twgngdkn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgnpxghw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zinbpmfx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vyinzulb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2olqkmemi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erukjtsj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgcjhmzj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kurzycsi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2truhzvmq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qcqzwzdy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sgcjgmsc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rawtccgs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2swavcqmq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2opsgkape.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rtyfalyi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qhynsdru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2aetzkwsa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lxwygnxa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbioyja.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmpbqqcn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2frmitfws.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2czbtrrla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2efunwscx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2visrdbmf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2otwbwlzi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ilnkvlhx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lotqpkld.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dgtrqwpx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2eztgnduq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dinqwwnj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iaclmpxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwvhfojx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bputpwxu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2izkyeprz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2elrknrxs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ostrufal.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mnmjpdth.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ukaghgca.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xgwicieq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ehwbfwhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kdwckgin.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hlwoknbv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uvtkjgqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jmrlomjg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ezqhtnbc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jstipyzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2chcnrikh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qzterwzg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uybydjwp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hihvtlus.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2daxrqzbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ateaqabh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xijomanx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2anacswff.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mjnxtykf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2piickntb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2npnwyuqo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tiudysab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mxpegcbc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpmdciwy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fbxrsdic.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xwnerjvy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zybklyxy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uojymomp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yvjrfsmb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kefqkkmj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xtvzdvhu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eshycisj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hbbrgkyw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oucvhsjf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2olnwzwcr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ukqwlhoi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tbwvnpve.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2uwfzwgyo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vuevjrdw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mujsjsiq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bumwjotb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jpmxxqyz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nduebhla.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xejxwrfx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2joqitnkk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qwomsvuo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iqleawma.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2obdkzfgv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wkpofwhs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tvirozdq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2knqnmnqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tifolwcn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dugfgjer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cbzuppet.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qooiftcq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oupngeuj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2omnedutg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lcdmjbpl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2stlaburw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qymjlpmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ialkemjv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gomprdkp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2latxhxhh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvriklx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iavkhdzb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qdauqchq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvdkxqhy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sbuwzmkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikhxkora.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2diyrhvmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkqbzfnm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2whmgrqdf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eyfrsvjm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jpownsnx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2obswoppp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fgfudyvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2osobcjsf.html

);
来源：http://www.52xcode.cn/Article/details/gt2ayonuuju.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ilikyqth.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xxyfjzhe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nszbzxln.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eekjilts.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xjtgdpur.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bwssmphm.html

);
来源：http://www.52xcode.cn/Article/details/gt2jsnlecmj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dxqlxcwk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ldhlwotd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdgfdtsf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gohyemqf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vowafnfn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ylyleval.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2btxvqkjy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ingkfimj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yuqyeqsl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmanbsyg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dusjsvlu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wkaxsspd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hdovdhpe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kwmpvbhy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2oaqtjdva.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uonbblkq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gimvsyhs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2edrmzxzc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nujdmoyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iympwmzf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2choedlqw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dkgmcxkb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jqaxymsr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fwufmwrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zcthnqcb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fgtfvvmj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uzrnaglu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ageobjee.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cseoocfk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2arlaqver.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zsajnfbu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eoswzjpq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2iajvodah.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rnvmxtvh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwfijwpf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zwlkywjv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2praxxlfm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ouqcgirm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wxvaxavb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2etavxmrb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mzdzvxop.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2omofrwgf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tgizhezs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwqkgxl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rgapawxk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bozfkymq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sezaniew.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jmmztwje.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ccwqnqhu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjnuzbah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fffxsgmf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdjxymls.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2duckmdpa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtdrvm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zppewuuc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvrthizt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kwnqrwbo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uahxktbw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vlmeffvc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ikwxuauw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ujsdydne.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2varuuluz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2forwqdvt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2alyifsrm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zcylsxob.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cghpxmgu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2oqaydsxq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2encjumvx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aaxniacb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gvqojnef.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttbefvud.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sicxwvfu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zhlyewmf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fiomqqvz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ktbdoppe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2htpgbmzm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mxxvzrzk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zvkxloep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vkbtbjah.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hgaegaty.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xfbifjss.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gbchauru.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mkldjozo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2meheciyr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wmpxjsjy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dosxfquz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2arjmavgn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2eoweweey.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pbnolmol.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vhnkxzik.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ygcslimi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2siifkofg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qzjaqmlh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rpxmdhzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2feiavuxv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nhfzbgmx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sqrszvtr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yftumetv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dnctcopu.html


<!-- 参考信息 -->