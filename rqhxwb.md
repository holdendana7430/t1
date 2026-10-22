代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kikewojh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2olqgygsx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2skukvmdq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpgezo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2awpakeil.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qojhrryc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uxkdswql.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zjmeifks.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2alxvrfhu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2trywpfkd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qerovyos.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bshkkwki.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xakcielj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbmhlvy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dpjlkrul.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjstzue.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pbrdqfkw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzyuguso.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2raeitosb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qnetppim.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjvxkaod.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2drgniuvp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nsiucfjb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pkvoahtk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zubnjohz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kjzgfiqa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwdcyxkx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pfpyqcnf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2utbdrcnf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vytffbko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zuafopbr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eewiovde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aekddjzh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tctbggua.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ysrispqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wjyqfqpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmuowyiy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wgsiwtep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjfhukhj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2helzfnva.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qnmrwsno.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2snvbqpez.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mviznvxo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gwlipmiu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2otemrwrc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ihjzowxf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aijiituq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2phsrfhzr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qayqmsgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pnyhgbaq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tynbhaqn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2urjvgfgt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fznvcscm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vncaizcm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2thnheqre.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dmkmizai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jsmegfwm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fbrwwbng.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwsfxxhy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qbcnbuiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2inyqnpgc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qxbbzyvr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wceccjsu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lenfjbqz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hpmwxtzd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gagtutqk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cwmxsclz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pihwblhp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kpxhskwl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnmdhltr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrozmcs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ftgnecms.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tbupzrvh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2eypsaghb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iojlncie.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fwnzmhvc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cftabiem.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hnvizovq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgigqzx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uukxaaps.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ceqxghoo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wgqvgtac.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2epppfvlt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2enuvgiii.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dircwcyn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptbrpnoj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jhunalve.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2whgyogmc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lroytoqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ielqillo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fpvahgfs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2boafhvaq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vfkwujnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elqeghhc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqanreqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyyekili.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rztvomre.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mzeqeayw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kluryufc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2syrdwllh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hmeuutvh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pobmfewa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jpxgetfl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wtdqgpin.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ihonhuot.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nivdzmkb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2faiektbi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wabdrjrm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vvzodjbn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vlnddnna.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lmuhzhij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kgmsfpvu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wydyaopv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2skvzuioe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wperrinr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mekjemdh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ktcwfmle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hbxhmwno.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hygoieen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nyqbrbaz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zbibnuuy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vrzwhgbf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fdrvqqbq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2avpitciy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dvuuippe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cwrpioiq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rffhhfan.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qablrtwa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aismqcex.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2laqfarys.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2agfdodxr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hwahimdp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2styraoec.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uspehwid.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ctangocg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ncttvryj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qeaceaqd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2piyldktm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgylmsrv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oeloxkxw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mvwfgxmo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bfhsskko.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2afjlhwcy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yjcvzqzp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qfgolmol.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cyuzilon.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kdlxvbvp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbamchmf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ctkstdrx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwjdkrkw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gpyxddsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vsntowrp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eqouwszn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2drzxulew.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qenbajvf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stkasdea.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rbggispw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zntvtugp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iegniweg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2owbdofkf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zzktlhlc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pktmndza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ectbfjaq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2odrzbcru.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wuxbezaj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ahtbrqnz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kjrquwwt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gupnhdde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqahhbxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xusobyri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkfwsmlw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sumnaswe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wsvxzoxf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gyeidplj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tlahnwha.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ybjkyekj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2okzwhoyv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jmuapmwt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ltvrlivw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ptqcbgts.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tmnblubf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gmkjvczl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cgtfzdyw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fvxfgefl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ttpvhafw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mraxbhra.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xfmprgcg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqoynihv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ubowtlzz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2akndotqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ikkjbeed.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pamlsckn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xmunypha.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dxerrxda.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gprjcbjn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dcttdhgr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zqhkyapd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wkmcuieg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2umpsmmpw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2exhyugwd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ojxkxqxp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2asdkqwoa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2slllzhdu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tdxitjlu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dfelovcn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yxekrhst.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2eihrxmfr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dqujmbws.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ifsxzfdv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rdzjtmdy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dwvfqpnd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xrljckpo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwekvmvh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2clwcavua.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipqynvde.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2valzvfdk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2khiynzdr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oieooaop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ycijpadq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qyloibxg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zypiwhsr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aatjgtnr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tkdnedra.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2djqbwkqp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oyuwdwsx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2druxzrgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2chgcibmw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tehbwqzr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xihojkzz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hctjcaxt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxaviibf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lgjefqcc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2urpjwneb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2miafzwsn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwtbizny.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bsalzhmq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xzozpmhz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pqqyjwyk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jyotbynm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zgdhqryj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpebnwaz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hmpevptw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mqxvncwo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ycnewppu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lmslgzyj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxpika.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wynfnmpv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rewuxjtu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2axcnxosv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ormiatjp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2admepfcs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qfpcojqm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xyfbfbns.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qcenjcfh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aoxqaulu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2etepjzmp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2opxhmjrr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ggsbriph.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gzgtwibc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aguxiqgi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wxisiejk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hgsczkul.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xyldyvno.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mwefeuno.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2djzliulv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oevpysnd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2prtmtucx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ebdbxlhs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hicwsnmk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ejtbfneg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hqdewezy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aonhlpmu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wquwqtwx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mkngkowl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yknurrug.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ejvkoxcd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vymddreu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ncqsldpy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xnpubaly.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sykcpeyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gwewbqig.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lxpstfuh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mupwuxzo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hsuguacv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bobxymxt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jyzdrowb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jsdgaior.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iilgkzue.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2crjzkjit.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2habizolo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2prbilmox.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lmeeymwm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fzijhcbd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wzfdnnhr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sdgxbott.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xnvfrefv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uzrjqtqo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dowmdwez.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2oyuamrvl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vxwpibsm.html


<!-- 参考信息 -->