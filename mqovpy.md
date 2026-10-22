代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nvjlwsos.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qghayqoe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vqkkphft.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ftsrqzdv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrzhgve.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2upniuubr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmejlqod.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2skbijjap.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dhdultge.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yoeabugi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xrpfbabc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctmmgjcb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kqorxldp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vcghapez.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bqbrfjyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsqjomji.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zwazkmza.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vssndvxr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ulxctkyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2htqbwqzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bpoobdhj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2noulerbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2plyugitm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zavepoal.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgzyhhqk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mmwccndo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2utriqyuo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wcactcla.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2plqcsfdb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wjtfyfrg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alabqmar.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lxnkqhwr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2okzerarx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rzqqgzgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2byfrowkh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jcuxtnpo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jerwdvir.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pnkbcpkf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nkhxatya.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2eesgrcef.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zaftxunf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xzhmmvps.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cuaxxnuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yrlfikhf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cilipzsi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uhayfhge.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gmkelnpu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jazsgnmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbwefb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2axsqjcnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cozobgcf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2eefuyhsh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yeytorux.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hwepunfc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2otoefdpf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vdfwaihq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vnjrxctr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nhzdeprk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2eniymrqw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pgaxtxmx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bqwfsqck.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2sfuuilyq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mbofuzsm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yorladgz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ginbuwsq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cwhbdbob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lmlmpccm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cmvavtdv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2htardohy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jvgrztxf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wqnjysxz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zteullrt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cktsmjex.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2npjirhax.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sdpqktyt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2htqpxcvq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2anlkuwnl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmftvawx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rnlrkznr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jjkfxwfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qfvicyuj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svbwwrww.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwvfhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2baaavorz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tdxkjxkd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dxkgegek.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ihukeske.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ylrlbeln.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2omjvngmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2uxmvqfej.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xsmtawcn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcrulbp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pvsotooi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vgpdsvom.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nqgbbgjs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqxdqqg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gigzslyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xhbmhcwg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kyjwhxnc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2azspgbcm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xwwuaxla.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jmqwbhgr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qsydeuyf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbxmpx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hxqvnunm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vigytrag.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmqktdmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhmaaqjz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2akxyuzhv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2izlbwicu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fgavqaex.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rzvcrqxh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2esmpxssy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uelnkzgy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ttxftrvb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2euujvcbj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wcviuilr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hqitnncx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nkerktbf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjhbhybm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pnqveyex.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dynvtkwv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eklmkkax.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nuzivcby.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uvavyhwb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2eqkkaqea.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nanjkyxa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qizrjerk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fngnvfjc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qnchjiqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bfzgjnfr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xnihgkup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xtzewrvz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jkignjmu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nkihpuck.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2thbftcwq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xgyfhxcn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kzscmupf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cskkvvua.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fooxmbrc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qkejkopk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iflertrb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lxwmmzcr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2obkxzhcr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qgpryber.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dtbrmrss.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zlcfigzc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iwyvnzvl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oprfyzan.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mwcwdejn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lqrhulgd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2srnwigbn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qlwdchpk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hquhmfqq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ifcocwfg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deilvbjw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2thiogkrf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwoykxkf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltzjemnq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbmbiuku.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wabzdvjc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2canhzzkk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2maozrqmu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ecaepnfn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dvhdvaky.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tepbgtdy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fhtkauzh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2duisgfnr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vdovkwje.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yfbyxuwm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xtrszjad.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pqhtppaq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eyzblrjm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvecewlb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uqdcmizw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmcthaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2numarkdt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2udeokhep.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dlebslam.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2swumdohb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtozalpl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lswwdwnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eosamilg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2etzlugwg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kqfhdngb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2velwmxtd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lxfnjalo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mvtjtxwp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qusmktxa.html

);
来源：http://www.52xcode.cn/Article/details/gt2lzojgzkc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lyiodtgf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ajtdnkbn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jdaikaul.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uqhsomju.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eqyetxyg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rcjymhhv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oxyibpjl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mbykucur.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xlcjrybh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2decpgtrf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2flyhetqs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jeknfzih.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dillfgav.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2zdulpjgi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rkzdhxde.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2seccxpph.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2afehhgen.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fqdksftf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2owvsjzof.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2riocsqwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hpzsbvgy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tbgjastk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mdvsnrfd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2onopzqvh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yjqlbmkm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gtihebww.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pklyytta.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nqthruvn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rtgbecjr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ttlyvsiz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2shtwxegw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ddepptna.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hyipkokt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xurtylyl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epfqijvw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yhvonrak.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnqzwubv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ipjwilhz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ioayhgcq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qjnjitlo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zamkazna.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qwdzubag.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yqjfpmip.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2iqtatlkk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dcwhlwcy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kgpmxpbc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ipujtssr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wpkjawrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2plkobhlj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ouqgodls.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rfssuvgc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ygrkuvxn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfiivyup.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kkqxxaud.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bvwautto.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xsxacctv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aaqdmmmu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mwmxjayr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2daultilq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mgewvzrd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hklevncp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cjyurpds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xajjszjz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fbswupsr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qphefxii.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dplgxgsw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wwntreug.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izhznscc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aaqfqurd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yyyejkxm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2guxmiusn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tfosoxau.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mnandvvg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ebsogory.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qoxlzyst.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ndanmmhd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fbcyzuna.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pvwcxnbh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kmdybgru.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hisgednz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qmkbjxgs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2doqkwuqa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rcdjvgbm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyotavgh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qnilvrxt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zyyklgzr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cgephxjj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jyvhwokb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xbpguxns.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2amxbuxgl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hznsxvln.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2inlsnygv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hifdqqha.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hcruwlke.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xbftrzpi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ftctrwyy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2thfgbhwc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jpyfffhs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sgcfehsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cjoxhwur.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eenhlxlx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dtzcscwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rxhmwiau.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tujcqsnt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rfgeteoq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ihxfwcro.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ocuemsjr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xrtizuar.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nrmvauxg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wcxsisbk.html


<!-- 参考信息 -->