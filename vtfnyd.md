代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wlgfvsea.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2esxusers.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sfexzwof.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xjglimqh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfoldyij.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fwqeerau.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kmptkigb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xnpgghza.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kxubrgug.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cwaghhmq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2czdnorww.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zoaliixk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ksrybrll.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bqvdoevz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fjbkgspc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gacwwulg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ehphphkf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eerxuzah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fcauojzi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2utmvfjpa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nypvzmqq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kpjtrwpq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vvmegldz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2huctmgjw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vbhovisv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lsehlpiq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cjojuomv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kydikotj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pfebcvrn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2egfkeiqi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2eetxkwoi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2voinqeai.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqymrsea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ulpdnqry.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dsovvcus.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nfvoskwn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lwezivho.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nbdopwoa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnvkwgjk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2imttrlhb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2czswxdtt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vxfgxdby.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gqncwxqz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zapxansg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eqkbfcik.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dwollhsp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lxlrearl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pnauwqef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uezjodrd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zbnkvttc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gowtfezj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tpipqdun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gyivftap.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qeibvisa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kgozxzgr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rtpsbyya.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2onakjlsk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2onjcixjm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2uarxotpa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bzcgzvea.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ulxhigtu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtpjahfh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2raruprxf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpmcic.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dnxpfqav.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iisaqfkv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uefpclao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gzxuipir.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2utrpypsa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vhhdqwfr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2iqkkjxzx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hajdilni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ozzcfall.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ydsxkfoi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hqzqpqdi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tmbvtvro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2runzqbcf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbgeccna.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lvnleard.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qzywcduh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2egyiasfq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dnwovgio.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ljiljzio.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fphnvwiv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ypybobsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mqzpvybb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ucmfzlos.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cmioqltz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2elduqjdf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2thkvznvw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lnoqvxzh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2clpiaebr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ijuapzqv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kmulunlc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wclkrget.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2eorwsjzv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nlublwfp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gjkkzbma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nbnnqhui.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yzrjkopp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2udfucztv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2accquczd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xwofgpbu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fnsmrbdk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pyltmfgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulkijous.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dctmlbjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rixjbgvf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jiunjlcw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mdugcgiz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qpkowciy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fzvopqsi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ensqluzg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kcmxnthm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lbcdpwkg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xtyauscy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jggsqljt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cainilzo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hkfnpups.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2cwhsfkht.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cdohcxgg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tdskdgvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kowewvvd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxnbev.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kkqhneqb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xbgfhutx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2teikmpew.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2weozfvxn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mgflleon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xwunuqxr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnnyqrrd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nzrqbkuo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bcofksdy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2taxhtugr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2loxhgvkv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gemktnui.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hholvcwk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vfdgoygo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ycdnrqgo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2numsniwi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fjqhcnjp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vgkcvhqg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ggzzxret.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kzkuuqfb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uavprdly.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dvowkhcm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tmqvkipt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ygvwohnw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2prqzxzao.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sprimkfr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rbazhodl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bumlvzhh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ijjysiax.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hopzvbet.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2witncjtg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2krcofthn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2njfaigrg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvyotfxf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gyfubafa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucxiedox.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvhnsma.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqxrhecp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dfunesrr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ivhpghyw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tndwblac.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ecxngwyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rkrqgbxt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djotcuhn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ibibmofk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pucpaaks.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xbyoiyqd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vkmwpgmj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjptedm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bygjrxlg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zckazpws.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2skrgbpsy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jvxisbyh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bcnpmcmi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cukgzufi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bkvimxpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igvanezy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kxlrqctt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsaoimtd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ghvugkwe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qxjglqfl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qbtjqnzw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zvbyactl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jyemrgec.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2funcwxsf.html

);
来源：http://www.52xcode.cn/Article/details/gt2adlladgh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2afmqhdlw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fqizucso.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ffcglmpg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tezwrija.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mscibwcx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2eedjpprn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wdvqssna.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2swqlilcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zcgxbrca.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wylthxos.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kbetrltl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vwmhnnsh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rphzbefw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dhqdmxvd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tlrdfuiv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ztuztwzy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fxoqsihn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uiwpocof.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yzcgzgdh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zlkmlccy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jkeprwdr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kzzwhuut.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wrqitakl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wkfllkun.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fkoiikbq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jebfwcrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jmsflllw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uvareokh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kiijlmye.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2phhrzkgk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2eypxvmac.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kvooucoq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fmmhrupy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uqnkyqtm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sainwzsi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wqcdfqjf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rynhnhmn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hfomlrep.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tsummsuu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ciibtlcv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zijedubi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2khtyirxi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qrwnfzca.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hafvyonv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tkdumgfx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xrzabozh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2itccgjts.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fhojfaee.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zgzvjbts.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2cuolhvcw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2lcdpqknm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2otleimes.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dpvyfvxp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ujrlbrbo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2buiqpxxs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jannlbsj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dlkjmqti.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rjatfcyn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oeexzqsz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dtrghzbv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yigsckzu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jpjqeewx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxhfttii.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ekizirhb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vfwnxtry.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qcroeuez.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rsmfsarh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wvemypev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cwmzaljs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rdhcjikl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qqjphepy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jjrpeldf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cubfnpfk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2awcokbkd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hyztwfud.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xqyqfagl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2prwwioma.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qnqybity.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ogivhhpa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dlhbstyp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kxzgzyjj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vqcpceal.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bvfielwq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhavnlie.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hbdaggot.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2guqzzvbb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2spxuvooa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sgcwbvgc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fjgeenvw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zydvuktr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2efeinsdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iscrttyc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2revcatgl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oblurhpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pscnkqwk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nrbylssh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zbgwthwa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ixeqfpfa.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vdrodbij.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2caduosjf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kzgmdvim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sjkdeyvr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2akhycxry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uktmzabo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xnamfpyo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwrarq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yspdriir.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxbbswa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2omoblfna.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ibizvsda.html


<!-- 参考信息 -->