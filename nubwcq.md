代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kvnokntr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bgfilciw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mzistqnl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2quwhnqgy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hiacdmsm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vlgchhyq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cfztciln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ixlqplon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mthgebux.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zucznyjr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2iyzvjjtf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2morkcswl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zrczrnxz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bixyofvx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rmfsekgu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qchgqkxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2goduqkty.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2temcvjeb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfpwglcd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2quzstmqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rkmaqcyq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjvuhclz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cyyeladh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zkfzepun.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2twvlcpur.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cfyqulak.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tqyjwvog.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugihuiuh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qrosnyeg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2opnbrfxx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gkjznpig.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vwvhuald.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xdjygqzc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ojzcqwpj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kjnudcuy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ftxcmanx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mvcysmol.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lbsudlvg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2svwwkenw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2diwamrof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hapnynhw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2aenlopho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aybejegu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mgwmdagy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cdlllndh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jyxdvpjw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sdromtnl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xthethdv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sykzyxej.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qrzdkykf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2grgxkbhk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wruzadpd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hobffsre.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2doixktyn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nrwjtemv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ucqupxbc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xefragse.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ticovepu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kbqpdnig.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gazsrxyu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vfqckawu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2srjbfbyz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrtackrg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nnpdjijr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qaqxaqsg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tbiiqpdm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgwlys.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2axyclnac.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wrtqtqtz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zttrdvtp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2azjyhguz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2bzczktaq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jlrlqqpd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqehswrj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2egppbyyd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2otiibkca.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2btxpjozz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jofhquam.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2eltzzlzu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ocbqftla.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yrahqkju.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eyymaamd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2labavfmi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsrefuh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2tstuvtei.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2atkuaasc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wpujyduj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2waekibhj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hqvtwjsv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2asuwnejx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2khinuavc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rwadzcwc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ouqiyfok.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uanakzvk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zkdcbzpt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dcbnoqfr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2bshtvueo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqoflwdm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2svughznc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mphmbiul.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2oltdxrxv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wzslbkbt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vyphzhal.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bszcpzlp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ojuzyqsa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gduwmrrr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jedzuqxi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ymddyagq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wgmfnife.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2srcgzvle.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zoajzbkf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhodousb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nhalmuyn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gsqgxxmi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kqbmnilf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hjazgbix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ioghogpm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2sqdzqsdd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dgnriynk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nopjxitu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2toudpwpu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aviksmvu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2scnyzlbe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2geuyxvym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tuojjxlb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2echdhxej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pbquetge.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rfmwlzzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hnihkpon.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2utdhizgc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ksajhuoy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zffsgloa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gurscege.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2idvbeope.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qtbrkdwq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zmsamixz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qbtifeho.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cyfjkwvt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wnfvftag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cxctlbkx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yhqpuzcm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2krsatyft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yxnhohhl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mchhvkwa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mztzjbsp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wgtkpngt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zqqplwms.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fnnvopvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jjqendmx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fttyuifv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ubuykaro.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aawndirr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mmlolffz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skhnusbs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xqjemcma.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qzoiwjpd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ouyjpnyb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2klljywis.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ijijnpyp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vwiftnqj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xvozsovx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mpfdhthj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ksievhsv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fofkbdkq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nrkorqlr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oazludne.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bwyrbyzl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yduyvwho.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2aptkrwym.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cqijyssr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bzetydqu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2liktcmqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzaijuml.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hlokcwha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozwgmrsp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lrddsblu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bgkujbjl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qtqoljsm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rvyxdilv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jnceljuc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mrqoazdy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jqdodyxy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ibcedthg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2khbbktnz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hekjofpq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2srlzxska.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2spgwyyrx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mudxwfru.html

);
来源：http://www.52xcode.cn/Article/details/gt2sawxxecs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wcksdgxq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jdzwfatm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2idfivhqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kwzipulj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fjtcwcvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2iipcdysn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rdygkldp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aevvpaxo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qyfxniux.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2huytzxfo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gwkfoych.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ndrdngmg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrtltjbr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ohaekfhm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ctmpcfdj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2igjoahkq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nhrqklyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hcypeimx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cvkgaeqs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qqrhrtcq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vujtkloz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mdlwhhgv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2demakkwy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2calrfqjn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jxrbjnxw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2urfchnje.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2oepcqaob.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igbbqiqi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2szmplyfe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtzzpddj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ltkljxgl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzsoyudl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gdurazmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vtizinly.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tgxtadgy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2urgdiclx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zrighgdq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2urhaxkks.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dvysjwvg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gcxadgby.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2silzwzof.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fgemoopm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kabgvuqg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mmftcuoo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fhqdnnav.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urkhphiq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vkvuvonv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fdpdhmvv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vfdoeooo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqfziucq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qvfkbtyk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsjmqdva.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cbzpwuow.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vfnrquvh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sygzqgob.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxfvilua.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ihdqqaoh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hiicdwfd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qqmsaabn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ijasmmrp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gngfvsrk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lwgmfnpa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nsiinwhr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gqdcxdbz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2islsrfew.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nctifwzl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mbditfkl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ajkqvbac.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mopfivfd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2amyvhpxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qkqbcsvf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oczgkyqd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xultpymo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zxzprdyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gahmfxbo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tleqhlkt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fvitkqja.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qtencoes.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2znfgraod.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wddgjpmn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nzwopnlv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rmlshqyn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gdnzkkjj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cvecuuot.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tfhcrmfq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dxgdctmr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uqwsewfg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bgxsfggw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2proktihq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cveoikca.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wucwbqyw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2agslkxdd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pvxdgmcq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2aoaovash.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ulupnrjr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vxizlwtn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rfbvjumt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pbwcqblv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sgmsxrwx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2usveltkk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dfefpxuj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2boulidsc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2asbstfbk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jyenowvg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vxgovoqc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qzoaurqy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jjjdcoyt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqyjziyi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zpybhkrp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uukpsjyu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hfupxuun.html


<!-- 参考信息 -->