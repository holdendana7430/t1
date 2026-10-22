代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2awkoizez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ierqoljl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2giyiwxhx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cruaomwr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2auqsxjpg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yosyrsjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mjzyvmsk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kisvqyqv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iphqnpkl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hwvijozb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2spgbkopc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xhfxdlpr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iwfrkbyd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rfjbaple.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wvvgwpqr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfpgmukl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2leduskcn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mneltegr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfxbyqwd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xzjuigtj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tyfcwpfc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hthmklgt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eafytqnm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yyqcakpd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dzvwkhly.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eynsjtev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lwqfrncf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2svjvcred.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jpwuwnyi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eznycjfk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nztikgfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2izdedegz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2astrflkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tgmrajqb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2knoapbmt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ajwmuipx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iyjnccsm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tizffcjt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qofxqqhq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tbhofjly.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddvyqcmn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fwdodjrm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2saadfoqf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mrplyvol.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iqujnrwd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2amvfnyhl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2egtinrat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2expzhgyr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sgnnixsg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vcpjmcih.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnppokp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2huibbrkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qiolblji.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yakuqvvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spcaxiao.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bomcjrnr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bxfaisej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2szvfwmgx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tmyhmshq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dwcgdcah.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ycdcmppm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2uxblpnwb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cjarrmpb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2plgmbvyz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2frhocuny.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bdbrecih.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sgwymdko.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qbxlmpve.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gazrbund.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbpnpqf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bxueoucn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gavaqaou.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zxdkleme.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ppcaiwgs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2emhsyynr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2exzzdjed.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tvkcfhtc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ttdaagiu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzlbvila.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pwgcruej.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wakzrdnt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ltqdttwj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2avypyumq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uatjlgvq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2htkpfspx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrucswd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imffzemu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uinwlnvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kpqeavvq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yjdvcvkq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfvrxouk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xifpgzsa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vknhgfup.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wzqfpzfj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qprrupub.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2irskhbwm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sanjsyab.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dhjetmbe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hnufalma.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkauccbp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zvkouyfg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lfaioavd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ohrjgnsu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lhfaoqtw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2chkgsjob.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zxgkyixw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sekmcojg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2figewmjq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fbrsromc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsiueuts.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggdgveoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwzbregx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eucdffxa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rpgkwbhq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2uhvnwtyr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ultyhksp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cwcwbyzq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zkqfvkgy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2izdcenet.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wxshbscz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hqdkvagw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fmijcmgr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2curhxkdb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2oayybtfi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bhfqqrec.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ebsgzpar.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2irlzmgjn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nixdmtrf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjftevl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pcrtjjee.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rookdjqt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wiwerqem.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wdkkfcdo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oizjwwzt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kywqoofc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2gfsbprfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2twacylku.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cjfdblzw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wicrocga.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2owazessi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yapcbaqi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2znamtupp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2foamgbot.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2euypklrg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aylfdrcx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdbohat.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bcuwowbn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dvfsekvg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xickscup.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2trxwfkte.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ngbkkdxx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jklmdksz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tifwpglp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nnjgomjr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ktwdteyj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xaxvavvh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ujmdzxmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dqlddzwc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zjvvogqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdeocpjg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xocxicwn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cupzfaml.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2owodvigp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvrjtjkx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2laokoogs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rjuhgmyy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cpbcdyqc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qenemioi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ljviewyt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wpidvyhk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hdjgkilg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yomaoarc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oquhvcep.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kpoondog.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bgsimxaf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ndxdqkxs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2htgaxtip.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvcahn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2usdxxpxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsymagiq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jywpjtsg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qwvutbov.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jnngwvha.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wnqqtlij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekjkpabl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bbemsdog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shafxlpp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2inmslyoh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2axfzlnkq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hzmsejby.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vvtqbfqs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mpibfrnd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mtpouxps.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nqxsgcwy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2pfnkhqlq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uqsmzscf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lokoppsz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fsryycrf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2exburfwj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hflzninl.html

);
来源：http://www.52xcode.cn/Article/details/gt2edmmeyii.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zxekqoqy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lpedirnd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2myqzoypm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jkisiqtx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rkubhhqf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wzmzewlb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qssecfjj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uyikxnjk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qyoimdsd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fzilnbbp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ergepbze.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dqblcaaa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nqdtznzi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lbpzosom.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2htmltedm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cifmyayh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2cillavlj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dxjdblxl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kqxzfhmt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ycpexiig.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hivitdar.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ozvgidje.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zszefkbn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yuishyiu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zbjkonai.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wgmbalrd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nnhizxjf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbezpdw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fauihaqu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcbmtoeq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2sljywqis.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2azehtbeg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2clsygwyc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nkhrcoqy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjzjzmib.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iflwmpew.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fqjuqekr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bbmceypo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bcgdpvdo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2enllmuaz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ipzwpacj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ucrxjfgx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vongjfiv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fyuhvthk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nsimuive.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iehmhggb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mowrpike.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ncqvbopy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2prhzrmsh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dnfckbjc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nkpjhtuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2helqgumg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dwzxthxa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmsdiqgl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fdlpheqw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkeqzwas.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gfncpkzm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pdgjpjff.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jljagduw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hjguqlww.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjeutuzo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xfuyyvie.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gfrggzaj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2aukadovo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kmgyxqmw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2avuwrzbo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2igdgctxp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ngxtnfgw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxvnzqdo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sosdrtau.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iiqfoncv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gpfdefia.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lkwunstm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pzfhfiqv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2psaoddkf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wqjowwuy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xowrowkw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pusfwflv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mcnrdpro.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tqzftigu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pblqcfqf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mfnlxyye.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2slliugft.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fekcgngx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lsybmeaq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kjwvjini.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wvokzskn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sheegerr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ialhhgzx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qedgmuey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2chlbxspi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rcegnhyf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mvpbvwnr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ginzywrw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2frybepyn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kwhqfbjq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gqequvfv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2owjdavgo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2njrpiosr.html


<!-- 参考信息 -->