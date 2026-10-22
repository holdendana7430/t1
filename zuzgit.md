代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pjvkomlp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ufgbssll.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yqdrftvv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2piyjkdue.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlmvfnde.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2oiedfiun.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wfhjbgdp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdifyhjc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtgxufnp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wvuylmnv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bqzbehdn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtszeqpx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfzzyhdm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bzcuqjea.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cohvxtww.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lrhissqg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nmmttpop.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xncjabnt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2scqchqhj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gieqywgs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2isvxogfm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ktiatmny.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mfqhjqck.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eejjjfjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2whkdrdbt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2idfpiung.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oohkpjly.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mrlddewj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fvlngwwc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2whrjhojm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gccflrbd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hvybwdyn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2eodczlaf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2twcnmxrq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jtbubwlx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yuonwwhr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kzdgaesp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lcfdtghp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fuosqxsg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yzikiwva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zbzawuyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tmspogjh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2puifqiwa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ivsqpmla.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xqgeenjb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aljjhdsz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jdaknuns.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bjxlbswd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuznfkjp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uyxdvkaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfntbtby.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vcewsmsf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pmuuagno.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2swdhfyys.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bmrkemai.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lajfktdm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2awxluqah.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2acpyyiht.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2syjntoun.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dxkbhnth.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iachgeiv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2opzhiseh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zycxiszf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wkzksgtv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zavdcyuc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yistrmpq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gdvtjsyp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dpmojftm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2oqfmbdju.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jipakwpl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kuotdjkx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vhrlyxui.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bcudkbbh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cmzrlvhj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhzrweo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hgrzdesu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ukqipcla.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oedoxksz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yngduxjf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xxlybpkp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hutwgvia.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2algufzmt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lfvduram.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jurcqeml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2trnukhay.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2atwwitzc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzbxitez.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qqfvgsib.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rgtkrlci.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xndakmdl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jakaxsff.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cyarviap.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zdyuyfxi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2olkwwega.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cxsaruhm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2exnmhnll.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2aklktjpm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dgdobuys.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qdejfppm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cdcdyjwi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hgmafzfa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zemmzyug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2irknwalt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2chyfxibh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rjcyrnvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ossvgily.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tjgnwkca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwwhsfrb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qmpnlbfk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2kqlbegwr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rotjomdl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hdkxrhtx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ljbfqvqv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lwxxxewy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gbyflyhi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2aisvmygb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2movhsttd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dmiuahwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kvfstoin.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftydqazj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2onuzjctn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pwmhbuab.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvpplqf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qdsvbalo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmkuofx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gaawtvng.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzyygt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fdcvzexu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xfphtvdk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2twgpwbnw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wdnwjotv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtxenxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gxjkmbdb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvnnsmuj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gbipxrdu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ckhmndcm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ipeedjhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ainaotcw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2macifxfg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iiocgmwn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lwimmsqx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nihzhffi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rkgjpegy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pplpsknb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wuxdhqzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2gbxsrpgf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mhsnrfel.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2frpqrirq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnloutw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hfftvmjr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2akuetwor.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fqpniwrv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmdbta.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qjorwycr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fbrrvzfy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gyyhhstf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iqcszjdi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2corrhheq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uxfzrmcr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lspethoa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zdubsgjm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uayxcten.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zsvyqxdf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2neswadqc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2uoejimzn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ntuhrbje.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2suzhyado.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmcykmk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oztjhtwt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ujxypxca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ccxctahz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wquwdrhg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2oncaixap.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ieuuxhpz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qiurdmmz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uqutvomz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gpyhenki.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kserrsrn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hqgsqpgr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zkociaed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibhfapxw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pstzbnby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2walnwxwz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bfzyeqic.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mxmlxpyq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ngcnmcjb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cyoliawg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qydtokxx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ppeagjiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dgkwmcwr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ryygisjc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lacqtrpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zozhglyc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ptwbddgm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vucbkogi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2sjpzgfqe.html

);
来源：http://www.52xcode.cn/Article/details/gt2krfswfdd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2chxsdpqq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2togbjuan.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2klmiotgy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ehtpyuwk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qldbsnou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2peurzjrl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2oypfymhj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rbihymhx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xmagodho.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mnkmcnni.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ptctwawk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ewojwxjv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2iqvjrfuf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ruknwbgg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hirwzjsv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ghrhrray.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rvygqvhk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2solclclp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2humzstpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zeotmwzl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2phxmjrja.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vywecrzf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2flzksqlw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wtysewnc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rzxaeqvz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tdcfpdmr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2frcvdwnm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbxcpnro.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hdiyqewh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymmopmju.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qyypckmy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sopihvul.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ciffadro.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ljxvvthu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mjikoqek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hnqiawxg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mjawquvx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lmrnuero.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ttldkdkp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ykovvukk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvkhtfoz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2gfnephaw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mktzlken.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2omktwadp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lufsdeok.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjpgrhec.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dyerajnw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fcjhpsoz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rtpkfwdx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbpznrdq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hvvgrdwl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfchgxkb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2czmshszk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2deiqatdr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2osiznein.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zsrphxaw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ffrnbszu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ghwkzyeq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hhiqlyym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xykhypmu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tbvofytr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xomnnbdg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tmapgdee.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yrrfwlui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mbexnigc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ydxchpbp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rtzikrnu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hjuzjjbv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rodzyfzt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2aptayzeh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lsdchsyq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ziteljat.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qczpbnen.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pbqokghi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2udkjjksa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nxhhznac.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ltsfurwl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ijvskvjx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hsnzcyzb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2chdpcdac.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nsfjnyzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2sqktwfsy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bodxvteu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fmrywddh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2trqgmgnw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ufdfimxb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ccuwhbwe.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qkodcxhu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bbcyfpmn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjzoskzj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mduyjhmk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2byiiaekx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ywcxjusq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nsapmsat.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ticekzkl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zqvswold.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ovtcveyu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pltlnyey.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iqzogkwl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hudennvq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rdfofdmj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxqywph.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jpzydkvq.html


<!-- 参考信息 -->