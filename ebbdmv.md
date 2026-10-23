代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmlikkmv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ughweuhw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sgimrsbe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nfobhwxd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zwnytteb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxdlykzg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tpptmred.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxumbolt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zctrpiey.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qbtswiub.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jkoplnns.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhcgksgw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vqtbrmqw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ergybhvs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wpdmbtyl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xthgaduq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yztsalba.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwttjfd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zxmvutjl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3btiazsmm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kuwneajn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vxfnyyhy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qndrkwom.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wxyxaffj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tzbbvneg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pymlfdjw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bycjzhcy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3swsdyznu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rianludi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ditpqfbl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xhmguhje.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qsosqfoz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3psjzsdgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dppjziun.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sxkjkpbs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fqlwheap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbqkdfhl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mgjclehp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlycgxsu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zptgztqe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cloxhjib.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvhqgyyf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3irdgcgdn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cjaonizl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3khyatfjk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bxlyboeq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3isecbdmx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ianhioab.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3klgilsgo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ypytadns.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qhmgoewb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3inaoxwuk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xyiicbdq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dhmkwcrj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cqcwpbgx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3owvsepyy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jeeovogu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kduddjji.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xoxkxyjk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xftyzmxk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xozvkiwf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pbggyisx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aimmgdni.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qpvblhfk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wellujdj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzrbmey.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jozzrhqf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pfkpuysf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qmrelkro.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xfjxqnmk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khitzmgx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ahcimwus.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vhrlyyrd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yqvwjaux.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3cxckwlgp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3urhhtotx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mqojrnos.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pjoqhlbt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3agiwndez.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kodseaeg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bdapxuke.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3imyfotvu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3beedxdmy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjqzsig.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pqsozzbe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jrnqgrlg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3chqsrbvu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3huzwcytz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ycjzklmo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aziwjxlt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vfsmxcne.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3txorazuz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wyjfrqwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcofhcin.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nghdeevr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdohjnxh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3miwkvsaj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mhbxpqtp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3unuxejpj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hiivljxl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cwtsuooj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yllqwgac.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gjnyhbac.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3svbpwewy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vgefbzze.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dogjejtp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ktyiurpw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3txzendih.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gyhpfcjv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnwdgee.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uamksbgn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qaqsrhpa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pudlujje.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ghyfivke.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nlkqcxhn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nchafzcz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uopwwtbg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dkxhteip.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tofkmuyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mhzqjjpn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hgfasvzp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkoszn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ngkqnxyl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qiyklgtb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3virryyce.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cmnpvqlf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eaizmjgc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3crthejix.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dxgxjrkl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yewtueyd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ahwilwyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hgjycwlo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cwqbyyqm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3opuistnz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zbghdsqu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xbwigruc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sctsfbdh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dmiostjt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxttpycc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kzfbyqab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3czlmwgpg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tlvftkvc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hxfncqzj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ucqovxqe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lrbyjzti.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3habgcdyo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lrohpajh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vvegjqyx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsuzuuv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jgjxvdhf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gmctmaes.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ympyioux.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ivvxiasx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bfhzxvqb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qwhdonrl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3guimrari.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ejxjzovc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yikuoxjw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3irgnvxxm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3grqrbozd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jmjkzvpg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jqwaqfol.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3upbfkpou.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ayhgrfkk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qfugoegy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ryxxpcdn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fcdnwznq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rkwbigmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idymmhxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3anqtylmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuxjchdn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zuvksaix.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bufojeqn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yuwzhpkq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mxwcfjrp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3llghjhub.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lfsufryo.html

);
来源：http://www.52xcode.cn/Article/details/gt3rqcqykum.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mhlgutrv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iahikkao.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xdfjnxfp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3smdilsnf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dryweagp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsbkbzq.html

);
来源：http://www.52xcode.cn/Article/details/gt3kodpbhto.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mvpztghj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ooknynbj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ifccoowx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ihpenfhf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3anjyjkxg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ssahsrri.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mxzencsy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zfdhsfsj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ehmkxtfz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3soxlhmiv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hnhwxyfq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qjgignua.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lipuuzsx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ccsxrndo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zyvvmaaf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zdvyuhny.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uczquzpp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oxkfzwax.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xuovrwix.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wnbztbrf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rycpzmne.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qiclcvgm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wwwfhunq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fmeogtpz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jzmdbvng.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3uzhkmfdm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cpttfxkr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjjjijv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jhakjoyu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbgcvcua.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hvsjkjgi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3norzhncf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xajybrjw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hityyhep.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yyegjpbb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fuwqlarb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nxocosxx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yrqjyizd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3glnnezsf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3majzoekc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wuzdwuuh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pavbgdxp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ufkrjclk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnnhps.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pbjahpas.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zlsnoesc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3seydtaqv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nsglqcgp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wljesxkd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohdrjxyv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ppstqtmu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ocphbsxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dactjlml.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hsxrzqed.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jgfgovqx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgdglomv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nryladyt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jkqzasmx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qeyxgvfw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kubfzqbp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brjtnyup.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fnugqbnv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gxoivequ.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ukdgwtxv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3nmwrxjjp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qzezctaf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bqacifkp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bzoovhsu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tbnglwkr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ikazpjyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cksmplbr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3icvcokxx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vbgybohi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pyjvysca.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zpsudith.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lmgobbql.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lagfhptc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jqerlewt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3igqkbjvw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3whpylhdv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mlfrbdys.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ruvkatmp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3egotjjat.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lhxurxlp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gvpcfjbc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iijeczui.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxcofq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yayfqtjj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hifuoyxv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sllotyfy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uydbzlxe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3isrudlsg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tpwlzpsi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xikxbazn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kkhjldiv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qmjulsqs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bdrebklg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jxhoaykh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tlfloevc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3diqvvpuh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hewbtcnu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bzdmllgs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yrrdskfx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cflxhedj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3znqeplnk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nvtgjlis.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzfrpgnm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3myrgvexk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pjcgumog.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vnhlvqek.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ozgxxpfv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3keqjdgno.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uxddolto.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3djxxfnaf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rfwfnfgr.html


<!-- 参考信息 -->