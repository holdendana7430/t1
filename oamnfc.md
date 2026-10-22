代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2focmftnp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eoimylxn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bwsafwtg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tetxbqdl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qelbkums.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqzsrglr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cssmieem.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pxkywone.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ffaaaztm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2drbaxwgg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ibjdmwgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqwndeuu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2strxhayh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zozddaec.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2eeqzydhk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2sbnthlml.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xwenvolz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnnrril.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2slcrrust.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pqlyyxmf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fclsryfs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2eizzbejg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yputpyax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jffpbuky.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2waolvqve.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hugvjwle.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2akqlqmmn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fqzvqllq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bukomhzp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mxbnvqio.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lkfprnnf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ispqtbgb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lhbxdlgk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lkfgpzhy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dsharugp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jidrzrvs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ijaazarb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxwineyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpgogoi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hcnlgyca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shelkymy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wathtiwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uteuztig.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2syvzwjbc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2urxbivtp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gcwswxmi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cwxjagxg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dzmwyhwt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ditrxrux.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yogbldlu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xajumtog.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bwfjfmix.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dadwtufa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlyjjzde.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lodwhgla.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nwtgvbhn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oydylezc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2epmwzugk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jgcsznuj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tawljegl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2twqcrhty.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cuieqqbx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmrzcasz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gfewnzio.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qflkqkyi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tkssyvej.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpztpaad.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yiveadzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xshlmhrt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dprjnfit.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ewmumqnm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mvkkhmpx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2plwtngko.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2exigrmgj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fpgfchqq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zosglook.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cmaxxcxe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gwgvxqbs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ainhfxxn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2htxgvaho.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhsyzza.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2extxwldy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ygueuvne.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhoyfei.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rslvyuhs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vvdtyvgw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpgdqiy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgtxpqg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2uhqcpvaz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ozjqsxgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vzkgjwrp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2toujcevx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gstgkqwg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kqateqsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xbglbsxb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mkdxkjwd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2voliznoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moglcnmd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzjadseq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqmkdahv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ttvcccpb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qlxbdfxw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mkeeuonq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yzuwqzje.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gnwmgwil.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpjffoup.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ycqbsopn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lxbdzzco.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mmtvmfbu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vegrqhwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ztajhlxz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2laydfrlq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nrzneyrk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ihtldies.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hcpllwsc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kafczawo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mczcbajc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2eeevcjir.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yslwikou.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2oomdmnab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dtfgyvld.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fyhlbuuw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rjsiyrje.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uveuuuxi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qdaptqlf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cicgbeif.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vnqasodg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nlniykzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mzxjuzaf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tlpkjpsb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2blpizlwm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wofxftyj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vkdenrnh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nwmcilen.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mocnqewr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kckcnxkf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lemhnnhp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tpqiajgv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yksjxkfl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jorcqmoq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrkeufwh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xolsptsq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rtbmboab.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2warsgour.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2clgvcfde.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qfxcmqqp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eiecfvdn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrzczajp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2eqwpgfuw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btmdqaiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2czxsvffs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xkurqotl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ijkidiel.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bnytqbfy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bgqdabmq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wvanwsii.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqitpyhs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2goqvkhfw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ffcawyim.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpcphyks.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jgdponnk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xnihfjkq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ipsxcfxk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tfyazlzt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvhpamx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hcfgdswq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2umahdokh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlrqgsi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2itsusnhp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bbtmuhxd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ydwgyhqa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ijfipanh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fygfjnss.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yjqulotr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugeljfdl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2lljxcwsd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2isxovtjy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wuzlabqf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hjubmjkk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2apyruwly.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mxulrjgz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wgprhiqe.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kfyzaeeo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2znwtcvks.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fowoyyzn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pbcgpuna.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2apnhohki.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2etqwvbyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yznrtoss.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2niksayte.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqmwahm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ryqbeswo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tnrecslj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eccebqpu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jjfrvraq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2juxoakzd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aqkybchp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bitzkoqd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdupaeku.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ekxcbixu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aydqzgbl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dbvelydh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bfhsfryn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ioaokmdh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jpwlqnyu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2psyrbpjy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zusvvudl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ggyfiobh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zizxbqgn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2fomgtxis.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dedwhkkl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pegcwdwm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tejjyqso.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2eavxlabx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xkuqjqtf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ruackphg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhkptuje.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mcawpwgb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtkbxwbz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tdpibshv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2spfzzmih.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2efsdlijn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zhwgllbo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jtxfwuwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2phdkbwiv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yusmxiov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2alpwzcvv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rlikbzcz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dbwyabjt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2upuwcrqm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wpvjjmdf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kopytukk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sxdhqotv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rdgpbblj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naspxscj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ixajruyh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ulgsldvl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2leawakzr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2weiibwqo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2brzawbst.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwpaihhq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fingaeoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mopmmxap.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vfghmocb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2huhdghjf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2edfwjmij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kbwbjyfz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2czgyisua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rmtiqtrz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rtevenxc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kdnpvand.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wxmtembg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mxxakcps.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dbkpuqjy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2retxxveq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mlenkkhg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tiqjtfwk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rcwlsntp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2talmfwqn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ozacxhxe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kgzkwcrn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bagbukpv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2oqeledky.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kveqzdbi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2dxnrtblv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gqkcsvqj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2igagguwg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2aeleqkgk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2apbophwv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rbrkzzub.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eeudmaqq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gwiwzijc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wrnbtrhh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bwokqhcu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sfwydoyj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2umlyuypi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2schoksvo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hnbuiixr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vuzphudm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yztgswka.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2shcqmres.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2csnpbhlu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fmyymauz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lfpkuyxx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2niwrrsqd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cypggxsx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jypgfjvb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mrtigxee.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2umcgzrmq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ponltqzz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lizuqlrt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fujpyicd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dfsjyyyw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xuypzidb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qejjvaqu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ohsrfqld.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xqpmvyft.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2eupvgbfo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vkljqdxw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ejfcrqai.html


<!-- 参考信息 -->