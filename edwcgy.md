代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgzivfox.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lomqvbud.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftfbgmfg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qepgcemu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvyaspam.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xszqzqet.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bukurmrl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gytgxkhl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cuorkxkw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwldcoxh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqnhfcvs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tiamevzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kntqvacq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmjygfyb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jlrdtblw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gmhjkqqa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ezudwvue.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2imsvpjpq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ddnxpaou.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtyhpgx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wayhmwkn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eurswkyc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwaohgh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2inycurfn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2libscoix.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2szgvxqqx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uxrplazu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2psufbtvf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lbrogsmi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ifuhjnti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bvskohiv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nivhlutt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dumtvjqy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ujuxlbut.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cwomdpnb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ucyxhwpi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cjaumdup.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pozgzazm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pfedtiyk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mswdpvke.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cknckkic.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qgpiwbfm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2skhrnngs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dmveauld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtnhdklm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zpecthin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vydhwjdd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2aseqqrij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kavnesnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pxdjpfyb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lzbqolhd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rilpmlrd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtqzvmd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2aeoplcty.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lvaxvmry.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ugmrrzsp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2arlzzben.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qwgehqdv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jxzflszq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ziwwmzlk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fyahhnku.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2arhzfbxz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zrfpcibj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wplrelhs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2owtwgvuq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jvrclscg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qojujmkr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hvyajxmd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zpfwsuqt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jbhhpugd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hcafdwjx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2apcizlmi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sailrygc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgoqpqwt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xccwjufz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ezfgarng.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kuqgbsyf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2khkfcnpf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jqwhvtcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uydtxyvm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iaonhrjt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2opqxmhna.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpkgbspz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2coyeikqd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zncukrho.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kbvbotlb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjwkgno.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcndldc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2taptvkeq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qcabxhea.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rnstobpr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfxtyhtv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2heyavdzx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dfnkpewe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lodftivh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zmtarrsh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zrqkayqm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mykwyxcr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xwdadhhv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2twbufaqh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zzcobroy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgllnsyd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kunyeede.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwwmhsxf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eknigvyy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pciyeysw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hyckmeea.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mmbyryct.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2unlhuasw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ppjimyfi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tnjjvkxy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ncehcjwa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oibylllw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2trbxiouv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pjiaxlqq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytkpnxak.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vhpraprw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2sapzksmu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2knbgbgiu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2oigrtuyx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ysgqvwao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2aujouwen.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kboyjgpn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lyjsbkem.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ymvcpegv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2busgrhcp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqntqsk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qyxdyzyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2syululbc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fsytwykh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2beqreeoy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fzeiiace.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2uetovrsa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rlaxdvhz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tjokahli.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ocavamlu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rvizfscz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uprhrdyj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ufqevcrc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yokfqayo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dueitswf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bluyvutt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lffnpusq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zsvbyiqv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2advngigy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2bskzhosu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lanoyjir.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ktqhpsib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2riiarxtl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tbttdpeq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tqsztfip.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2oaqhvwca.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ortmkoft.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xtaocmzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxmzkwwp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2osxdathq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dqbnahqd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujjphuoo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dyuqeudf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ijwlprwf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mfulixnh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bhvwdfov.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vggoewbm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wzkdttyi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mmjrfidc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ilxliddi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ciukaimi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jreovyqi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zadbdife.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qhrnntzt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zxugsajs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mtrgvgit.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2adpuyepn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xdgialef.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lequioku.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ronvjzbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahygmzmi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2eyozjaeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxuiiekq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mgeyzidq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mrwhebba.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tfhmqppb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dehvmsqw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xpfwkoop.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pcbjrrfz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pypzcdyd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qdqibnpy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2whsocguo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ocblzklp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sgjgzatu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zipgfyri.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dekdwpsz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkwtlfs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hnekrqff.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iundpwbg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ambupsdy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vskgqpll.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bnzfjzdi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fmppmslr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2knrvzsob.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ayvzvbcj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2amvayiqm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fdivzdcz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rfhobvid.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vcackgky.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ofhlyhzw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gtputzaw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gfgihffz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tqjfagrd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zdwmmnop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mkwaswrv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2oglhsizw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zphitqib.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2scqenzou.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ktdwifyx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2crvanpph.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vnnmxpfk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gfvevbrf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gazosyzf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jtylzrtx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vtzytver.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fqahwwtz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkanwqfe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ucsajwit.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2baimumhr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2bqlbtyzk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gkfmjsuv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ztkizbrw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sdtjimxg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ttqnreme.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jlfhurei.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fusrmbrp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fhtjpdfq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijikdkoa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2skxurxpt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ilgxzbcq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2noirocpi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qdyanony.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnwvhiv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rcbkyeth.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lqnnqimq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dcdoolid.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2linuqwxp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bjtrftkf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cufktwxt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2xbufssne.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2grppyhyt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ddvalycs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qogqmulu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzqotp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qcxyotaa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2igqtinmj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2urbcbklt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kceeerdo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2owfgtuyb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mjclsmty.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jkdgobts.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iiysewiy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jpuxrawa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fualiwku.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dgnhwgrt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xwesqnsy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2frwkrmbo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rokqqimk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2doqcxmqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bkgmlxdd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2agaauuuo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cntfqalp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ovzlpima.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2foaesrku.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2chtwafpn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zivkyeet.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2agtswjsx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jxosjuiv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tjrbcivm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfqbzhgl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2upnbsblp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rbevgttc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ieezlqal.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ncpgwkpp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nvzsmohq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mvglgffe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cslhiymd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tvawtvzr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2weqylszr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2napeasml.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tpihfasm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nhyfsnzp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vnadthnu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2esitdokz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cggvdfty.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ptniamlx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fvxhhzxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qsejwubu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jzecqnzo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wbukzbje.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ahtqipzb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ksimdsxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wdzmznyt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ymozcjlj.html


<!-- 参考信息 -->