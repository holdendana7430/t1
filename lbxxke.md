代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2otnmahzc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pupxecja.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2syjchdcd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pcartjbe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2olobsoag.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ozeuwcgj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvpbot.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qsmipvek.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2mzxxuxvk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gwctpakc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2grccsaal.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pwcwcirc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oadenksa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ukaqzmod.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2krbsomxy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2msbleovg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2przrpojp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sbmcqgbn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yzcotfbw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aitckbrg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ftzrszrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bwfyadrs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlvawxmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cckmzavb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nxjiynvk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qihfqsjd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2eyyaumtp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sfsfnkve.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lhvwwfps.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tdawhdqv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hhxzdiza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqbaldd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljdbosmw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qpzavtuy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ckeejiok.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qdpjoozc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ccgwuter.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bkarqrqj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2upoprsby.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xvgzvunr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dykhfzqv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sjumbzsa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jktzpgex.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ikicchzi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jrmajbka.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aetdghbt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hmfcdzce.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2krmduahk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wbvvinga.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vsgcndyn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jpygweon.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ylgdgksp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nsjsdmee.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2votartvl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lrjswnah.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xdnmfqaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmsphgdi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2unnwryvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhrregfb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wafpvvta.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2igwexdsi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oxfajayz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ndefjfhu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qvdrjsxl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gtpqqsmo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lhlnqdcq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2uxgztwmc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2slaypjvc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bijgajsi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wftraipj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nmruiaqe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gdyrmdak.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rjqdxrsc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pgexpijo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2siaejfqv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vkoctjcx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dcejyfpp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2igchuzxg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdsugkvx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tnikclyo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2axuajfqs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2clzcfwub.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfqztfzp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yiwkkvjo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hutvxqjn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwqunglq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xloesbrj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2splxskew.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2diomhrdk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aanydpkw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmmqtam.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bghowjuv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mhxyikqf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nhuantsp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2irdaomfg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nwtzcxac.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgdvrlo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zksdpkws.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nsycaqjh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpizukb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dzdgvvhn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gsesuoit.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2malrxxcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rntmuuzp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lvnbkrqj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cnophpao.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2otiqcopb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xpznsrzb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pigxeknv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qwxzbnbj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ujsdayyc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yanhgmnt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tzftkmap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qedysfjk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpupjkwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quicadwo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ukaysvsw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ovdvnsza.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pfsrsolg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2euxuuctp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xhttlbod.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smxndshb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cjwqzidf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wqloupte.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2krarkwhr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nkfoueno.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jwlafdck.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nhredlio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mpurdrau.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rjgleold.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xvuesncy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2feetybos.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hhnklfqd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wyqpmrwb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2aihyvbls.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kdbowlno.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qfteklgl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wbphtzue.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yypwfsbi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wkkfjrqm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnwlug.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgrlahd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bvoisgco.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rzysrcgp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lwthhrrx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bsdibdof.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xbwpvzhx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2erjngsmn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iklsamdl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgwzhfm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hihtpwhn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ckjqumod.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lgebgfts.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iyjzzavs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pgnpyhxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mxjosmex.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wribmfkw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zgtrnruw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bvnjjpif.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gygmhbpn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vrirvxni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2epmykqly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mlvcjsyw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhicegxl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zrkcgkzo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmyjwmxz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ovulaoyz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2npxmomuk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xhfzwmar.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wkozjxqw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2soplqdsj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2joghvklx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zvagdwnl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zswwouhh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aldffngk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2sjasyebc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ilernmgc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lmqtjctk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wymgsbjl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dzkrrqbf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nuddhhli.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfdybhjz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2aaghnqoj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztcscwuu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ullbainh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uvrdfzdx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kkmwidzx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dhhcsgzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifnjkzqp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gakiildz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoqhpyhc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cqknmqxf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hgiiwmsz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kbeadwsv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xmgygjnf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qcoiwtte.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wgovhniv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rpbbklvp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mzmhmndy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nglqbhvc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uwzvwfxq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ngtrecps.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vtkvegko.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vjbivcvg.html

);
来源：http://www.52xcode.cn/Article/details/gt2nuauipdv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2srvyppqw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gumutole.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2phbyyyjx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cdjknqdl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ucmkkbir.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qmmbcxww.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zhjpjlsx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vemnnwnb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2oshrfktw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ordanbft.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ucbxpras.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ywhgjzmt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eyqwnndj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmxfwmx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mhqvdyks.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nioxabzj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jykahgzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kbrdcnym.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fgxfebdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iyznhnfo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2avgxrclf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ejraivvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tdabgdcj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fccnelrm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hckqwyft.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wisaxfhj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2swjxmdkp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjzjtqyv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hkalheku.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2klarjmlb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yhmvctlj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvjtlvur.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gqyqowgm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mqflxovw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jjddxgye.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hhtidfau.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kivzdggn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mqasytzf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xezzjjon.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uhlqnziy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2deovcoph.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qkfxwefk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lwgyntvm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2idmfbvqf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rudovzkf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzumfjhh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mcxtdcid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xeperfqy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kkxnixpe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zoypyahn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kozkjyhm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccagcgac.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dgfsbgum.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uvgdowqz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ieazqciq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umbjxsvy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pqwktskm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qrniptwm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2iwnxclwj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qquctnul.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syzrocli.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2awfusvfa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pifoqewk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fuvmzuzz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mfgdjgqo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2krtfrthl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bjqhpqhj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rqekkpei.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cprscvho.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mgvznsmv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tsmwafqt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ibnsscrm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aotuylwz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uvxpceal.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2weglwxcu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2oywtyire.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctctncxt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2popbadoi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kmezqvhd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mefunnvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dtatpopg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rqvwbbbk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xvsjcudp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vtursdwz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zqgyulmq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2izjxyagw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nkgmevow.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pegxskyq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2eaxwmrcn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eesjriwe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vwaobvav.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ptojvzxl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wjbetitv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mevrjuxy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cjaxlwng.html


<!-- 参考信息 -->