代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ou.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://eh.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ag.hahajie.cn

JS:   process.platform;  process.version
来源：http://yu.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://cp.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rl.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ng.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nl.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rd.muxihuayi.cn

================================================================================
来源：http://jq.szsharing.cn

N. 数据结构与算法
来源：http://pt.panjiajie.cn

================================================================================
来源：http://ef.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://pz.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sv.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nr.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pb.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pt.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://ft.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hi.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gc.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://dx.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mu.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ip.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bd.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yv.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ey.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://zi.szsharing.cn

Ruby: arr.sort
来源：http://ou.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fr.colortex.cn

[N03] 快速排序（分治示例）
来源：http://jb.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qy.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://uk.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mo.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://if.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tk.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dm.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oj.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cs.szxytkj.cn

[N04] 斐波那契数列
来源：http://jj.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kt.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://en.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tx.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oz.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mg.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rk.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gw.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yi.bookmarksfly.cn

[N05] 最大公约数
来源：http://cm.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://xp.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://za.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bk.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rd.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lr.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jn.nszjky.cn

Ruby: a.gcd(b)
来源：http://qw.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ja.colortex.cn

[N06] 判断回文字符串
来源：http://ux.colortex.cn

Py:   s == s[::-1]
来源：http://sq.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://fp.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://tq.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://vd.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jd.colortex.cn

Go:   // 双指针从两端比较
来源：http://ol.shtwfgs.cn

Ruby: s == s.reverse
来源：http://nx.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xg.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://dv.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xv.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://re.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kz.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ms.szxytkj.cn

Java: // 手写 HashMap
来源：http://pn.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://sp.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ks.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bo.hahajie.cn

[N08] 生成全排列
来源：http://ev.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://rl.nicolike.cn

PHP:  // 手写递归交换
来源：http://ij.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://fb.shxzskj.cn

TS:   // 手写回溯递归
来源：http://dq.muxihuayi.cn

Java: // 手写回溯递归
来源：http://iw.colortex.cn

Go:   // 手写回溯递归
来源：http://dq.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://qp.colortex.cn

C#:   // 手写回溯递归
来源：http://il.szsharing.cn

[N09] 栈与队列
来源：http://lm.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mf.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zh.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://un.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uq.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nr.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hr.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wx.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ul.9csxet.cn

[N10] 链表节点定义
来源：http://xj.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ow.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ai.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://am.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hd.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://wd.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ud.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pc.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://be.colortex.cn

[N11] 二叉树中序遍历
来源：http://jg.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://md.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://et.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kc.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eu.hnjuh.cn

Java: // 手写递归
来源：http://xx.shtwfgs.cn

Go:   // 手写递归
来源：http://db.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ba.bjjhwx.cn

C#:   // 手写递归
来源：http://qh.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hy.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kn.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wv.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rg.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://il.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gx.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bh.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ej.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rn.panjiajie.cn

================================================================================
来源：http://ww.chemitech.net.cn

O. 并发与异步
来源：http://zz.gzmigu.cn

================================================================================
来源：http://xb.9csxet.cn

[O01] 启动一个线程
来源：http://yh.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rw.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mc.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://un.huixinmuqiang.cn

TS:   // 同 JS
来源：http://hl.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://lu.hnjuh.cn

Go:   go f()
来源：http://em.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://qs.9csxet.cn

C#:   Task.Run(() => F());
来源：http://jp.jianghongdianzi.cn

[O02] 使用线程池
来源：http://pj.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wf.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bi.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://oi.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://wt.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jp.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ik.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ob.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vc.nszjky.cn

[O03] 加锁保护共享数据
来源：http://lc.shxzukj.cn

Py:   with lock: shared += 1
来源：http://bx.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://aj.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yq.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ij.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://fq.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xy.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rf.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://gt.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://tc.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://ri.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://of.asd995.cn

JS:   async function f() { await g(); }
来源：http://ba.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zl.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jq.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mr.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zr.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://ij.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://kk.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://oc.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wf.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://mx.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://wn.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lp.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tw.colortex.cn

Ruby: threads.map(&:join)
来源：http://cs.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qg.muxihuayi.cn

[O06] 使用进程池
来源：http://ur.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ed.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ug.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://lk.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://nd.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fb.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fh.huixiangedu.cn

Ruby: // fork 块
来源：http://tf.asd995.cn

C#:   Parallel.For
来源：http://ct.asd995.cn

================================================================================
来源：http://bl.panjiajie.cn

P. 常用工具函数
来源：http://zn.huixiangedu.cn

================================================================================
来源：http://gn.nszjky.cn

[P01] 生成 UUID
来源：http://co.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://fm.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sv.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://mu.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://su.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://ux.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://yi.521024.cn

Ruby: SecureRandom.uuid
来源：http://ta.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://nk.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://eh.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eu.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rq.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fd.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nv.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uj.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jh.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yf.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mm.szxytkj.cn

[P03] 生成短随机字符串
来源：http://co.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dt.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qu.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qu.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cu.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nf.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yx.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mp.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://di.newstarts.cn

[P04] 求长度
来源：http://ti.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jg.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wa.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rb.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://we.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://tz.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://jl.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://cl.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zt.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://wf.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iv.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nc.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dm.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://la.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ax.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tb.hnjuh.cn

Ruby: a == b
来源：http://xf.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vb.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ja.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zu.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ss.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bw.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://gy.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ba.9csxet.cn

Go:   if x == nil {}
来源：http://wo.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ca.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://xj.nszjky.cn

[P07] 防抖与节流
来源：http://cm.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nj.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ba.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yu.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ak.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bo.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kh.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jn.asd995.cn

[P08] 处理浮点精度问题
来源：http://oy.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pe.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ri.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pg.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pe.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bf.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://we.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fk.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iz.panjiajie.cn

================================================================================
来源：http://re.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.szsharing.cn

================================================================================
来源：http://mj.haigaiapp.cn

[Q01] 创建表
来源：http://nq.bjjhwx.cn

CREATE TABLE users (
来源：http://pl.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jw.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://cv.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://ie.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cx.wgjwhj.cn

);
来源：http://nh.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://it.haigaiapp.cn

CREATE TABLE orders (
来源：http://iz.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kz.hahajie.cn

user_id INT NOT NULL,
来源：http://gl.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://qq.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yx.szsharing.cn

);
来源：http://xp.asd995.cn

[Q03] 增加列
来源：http://pw.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kx.asd995.cn

[Q04] 修改列类型
来源：http://tc.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fu.jianghongdianzi.cn

[Q05] 重命名列
来源：http://nn.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rn.chemitech.net.cn

[Q06] 删除列
来源：http://px.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pb.panjiajie.cn

[Q07] 删除表
来源：http://pt.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://nn.hnjuh.cn

[Q08] 创建普通索引
来源：http://jp.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bp.hnjuh.cn

[Q09] 创建唯一索引
来源：http://rg.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iy.521024.cn

[Q10] 插入单行
来源：http://dm.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://us.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://cm.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xl.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://ea.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://je.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oj.hnjuh.cn

[Q13] 忽略重复插入
来源：http://ft.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eb.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://dp.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ak.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pf.haigaiapp.cn

[Q15] 查询全部
来源：http://bp.gzmigu.cn

SELECT * FROM users;
来源：http://le.muxihuayi.cn

[Q16] 查询指定列
来源：http://li.jctech888.com.cn

SELECT id, name FROM users;
来源：http://mj.shxzukj.cn

[Q17] 条件查询
来源：http://im.jctech888.com.cn


<!-- 参考信息 -->