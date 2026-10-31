代发 wailian999

TS:   process.platform;  process.version
来源：http://ii.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jg.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mx.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://az.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bl.huixinmuqiang.cn

================================================================================
来源：http://bq.yuexingan06.cn

N. 数据结构与算法
来源：http://ln.newstarts.cn

================================================================================
来源：http://ex.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://zt.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gv.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gz.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wt.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ve.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fw.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://uo.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lf.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mm.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ry.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qa.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vc.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jw.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gx.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mi.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ev.jianghongdianzi.cn

Ruby: arr.sort
来源：http://sq.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://be.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://jd.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jr.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://mg.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hq.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xv.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gc.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pv.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://py.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mr.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://jx.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tu.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qp.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vl.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mb.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ps.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zn.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eq.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sc.shtwfgs.cn

[N05] 最大公约数
来源：http://mi.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://se.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zp.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://np.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hw.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tn.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ux.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://xu.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nw.yuexingan06.cn

[N06] 判断回文字符串
来源：http://wg.huanxung.cn

Py:   s == s[::-1]
来源：http://ja.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://qp.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://jd.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://mp.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gp.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://mc.jctech888.com.cn

Ruby: s == s.reverse
来源：http://zw.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qa.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://fx.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hc.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://do.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wn.521024.cn

TS:   // 手写 Map<string, number>
来源：http://bx.muxihuayi.cn

Java: // 手写 HashMap
来源：http://hc.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://im.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://yb.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ff.bjjhwx.cn

[N08] 生成全排列
来源：http://wn.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://xh.shxzukj.cn

PHP:  // 手写递归交换
来源：http://rd.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://kd.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://qq.szsharing.cn

Java: // 手写回溯递归
来源：http://bx.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://ul.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://sm.521024.cn

C#:   // 手写回溯递归
来源：http://kx.chemitech.net.cn

[N09] 栈与队列
来源：http://og.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hx.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fd.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://av.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jg.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fu.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yw.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vp.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bj.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://zn.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gz.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pb.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ym.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dy.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://aq.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vc.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bc.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qs.szsharing.cn

[N11] 二叉树中序遍历
来源：http://cl.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mu.panjiajie.cn

PHP:  // 手写递归函数
来源：http://oc.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ct.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ci.bookmarksfly.cn

Java: // 手写递归
来源：http://af.nicolike.cn

Go:   // 手写递归
来源：http://wf.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zw.huanxung.cn

C#:   // 手写递归
来源：http://li.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uy.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qo.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://it.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://un.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jc.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hq.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zy.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rw.hahajie.cn

================================================================================
来源：http://xc.haigaiapp.cn

O. 并发与异步
来源：http://xu.nszjky.cn

================================================================================
来源：http://kd.huanxung.cn

[O01] 启动一个线程
来源：http://ee.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gk.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ct.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://be.nszjky.cn

TS:   // 同 JS
来源：http://hn.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://ap.gzmigu.cn

Go:   go f()
来源：http://bo.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://mm.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://nt.haigaiapp.cn

[O02] 使用线程池
来源：http://dq.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ni.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mk.nszjky.cn

JS:   // worker_threads 线程池
来源：http://xb.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ed.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yk.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xb.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yt.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ph.521024.cn

[O03] 加锁保护共享数据
来源：http://hv.shxzskj.cn

Py:   with lock: shared += 1
来源：http://yh.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://jv.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kw.muxihuayi.cn

TS:   // 同 JS
来源：http://wp.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://xu.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fa.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mf.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://dh.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://wi.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://og.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tl.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://rg.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qz.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nc.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ra.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cr.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nv.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://oo.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://gj.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ag.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ym.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://bn.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mg.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://er.hahajie.cn

Ruby: threads.map(&:join)
来源：http://xw.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xh.nszjky.cn

[O06] 使用进程池
来源：http://mp.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hp.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://on.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://vd.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://ta.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ud.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wr.yuntaijiaju.cn

Ruby: // fork 块
来源：http://us.jianghongdianzi.cn

C#:   Parallel.For
来源：http://lf.huanxung.cn

================================================================================
来源：http://qm.muxihuayi.cn

P. 常用工具函数
来源：http://ql.9csxet.cn

================================================================================
来源：http://bu.jctech888.com.cn

[P01] 生成 UUID
来源：http://gl.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://qe.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dt.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://sb.nicolike.cn

TS:   crypto.randomUUID()
来源：http://zn.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://jo.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://nt.521024.cn

Ruby: SecureRandom.uuid
来源：http://ds.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://hz.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://nl.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ss.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ra.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tb.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ot.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aj.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zh.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ym.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bm.asd995.cn

[P03] 生成短随机字符串
来源：http://sq.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fe.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ch.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gy.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ir.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ur.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://um.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jw.hahajie.cn

[P04] 求长度
来源：http://eb.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aj.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oi.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mc.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ne.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://is.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://ew.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://tw.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lm.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://yh.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cn.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://go.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nx.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qr.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dp.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bw.chemitech.net.cn

Ruby: a == b
来源：http://dp.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sl.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vi.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xb.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://eg.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pa.nicolike.cn

TS:   if (x == null) {}
来源：http://vq.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://av.szsharing.cn

Go:   if x == nil {}
来源：http://iw.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://er.hahajie.cn

C#:   if (x is null) {}
来源：http://us.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ng.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qy.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://pc.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aw.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sz.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nb.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fc.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vw.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://po.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://da.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vp.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ou.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yp.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ia.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://er.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fl.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ux.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gj.bjjhwx.cn

================================================================================
来源：http://ul.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yu.jianghongdianzi.cn

================================================================================
来源：http://er.huixinmuqiang.cn

[Q01] 创建表
来源：http://zc.szsharing.cn

CREATE TABLE users (
来源：http://ss.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mm.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://gy.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://od.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gu.9csxet.cn

);
来源：http://pq.521024.cn

[Q02] 创建带外键的表
来源：http://om.szsharing.cn

CREATE TABLE orders (
来源：http://nv.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fz.haigaiapp.cn

user_id INT NOT NULL,
来源：http://ln.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://pb.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yf.lnxyls.cn

);
来源：http://vs.asd995.cn

[Q03] 增加列
来源：http://nm.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ua.bjjhwx.cn

[Q04] 修改列类型
来源：http://cx.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ol.huixiangedu.cn

[Q05] 重命名列
来源：http://xv.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://js.szsharing.cn

[Q06] 删除列
来源：http://he.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ji.szsharing.cn

[Q07] 删除表
来源：http://bj.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://zn.asd995.cn

[Q08] 创建普通索引
来源：http://re.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://la.nszjky.cn

[Q09] 创建唯一索引
来源：http://xt.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sb.bjjhwx.cn

[Q10] 插入单行
来源：http://mk.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vj.lnxyls.cn

[Q11] 一次插入多行
来源：http://cq.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pz.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://bd.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rr.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ge.shxzukj.cn

[Q13] 忽略重复插入
来源：http://nr.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ey.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://zi.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fy.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pe.colortex.cn

[Q15] 查询全部
来源：http://fk.haigaiapp.cn

SELECT * FROM users;
来源：http://uz.nszjky.cn

[Q16] 查询指定列
来源：http://mr.nszjky.cn

SELECT id, name FROM users;
来源：http://nu.haigaiapp.cn

[Q17] 条件查询
来源：http://qr.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://as.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://ee.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eb.hnjuh.cn

[Q19] 范围查询
来源：http://kk.jctech888.com.cn


<!-- 参考信息 -->