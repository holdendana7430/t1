代发 wailian999

[M08] 获取系统与运行时信息
来源：http://yd.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://sm.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ch.nicolike.cn

JS:   process.platform;  process.version
来源：http://eq.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://sf.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vo.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qr.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dn.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ml.bookmarksfly.cn

================================================================================
来源：http://ai.asd995.cn

N. 数据结构与算法
来源：http://fg.asd995.cn

================================================================================
来源：http://lh.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ma.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bu.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bg.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hk.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ig.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://la.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://du.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dc.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sq.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://sz.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://bq.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rt.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vr.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gi.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qm.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://pl.huixinmuqiang.cn

Ruby: arr.sort
来源：http://wi.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qr.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://pa.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pt.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://yf.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gb.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jx.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://do.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kz.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tl.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ed.hnjuh.cn

[N04] 斐波那契数列
来源：http://lv.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://si.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ee.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://du.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nw.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ap.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ns.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lc.muxihuayi.cn

[N05] 最大公约数
来源：http://sf.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://pg.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xu.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://og.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eq.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ad.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nm.szxytkj.cn

Ruby: a.gcd(b)
来源：http://iw.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zk.haigaiapp.cn

[N06] 判断回文字符串
来源：http://op.haigaiapp.cn

Py:   s == s[::-1]
来源：http://bu.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://jn.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://pw.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://bd.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jc.colortex.cn

Go:   // 双指针从两端比较
来源：http://wd.jctech888.com.cn

Ruby: s == s.reverse
来源：http://cd.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zs.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://ef.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jt.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ky.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ls.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://rq.asd995.cn

Java: // 手写 HashMap
来源：http://wb.nicolike.cn

Go:   // 手写 map[int]int
来源：http://iq.nszjky.cn

Ruby: // 手写 Hash
来源：http://ae.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lq.colortex.cn

[N08] 生成全排列
来源：http://vx.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://fu.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://nq.521024.cn

JS:   // 手写回溯递归
来源：http://ar.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://zz.shtwfgs.cn

Java: // 手写回溯递归
来源：http://wy.newstarts.cn

Go:   // 手写回溯递归
来源：http://uc.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://zu.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://uu.huixiangedu.cn

[N09] 栈与队列
来源：http://vc.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xm.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://is.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kh.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gc.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zk.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jk.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rs.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vh.shxzskj.cn

[N10] 链表节点定义
来源：http://fz.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oa.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ci.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kh.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wj.asd995.cn

Java: class Node { int v; Node next; }
来源：http://oq.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rs.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fq.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://za.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ug.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jo.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://ga.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qa.haigaiapp.cn

Java: // 手写递归
来源：http://sd.huixiangedu.cn

Go:   // 手写递归
来源：http://oy.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ai.9csxet.cn

C#:   // 手写递归
来源：http://jr.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zj.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://la.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wm.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eb.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vl.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hc.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xo.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ns.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.chemitech.net.cn

================================================================================
来源：http://wq.521024.cn

O. 并发与异步
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://nj.nicolike.cn

[O01] 启动一个线程
来源：http://mk.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wm.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nw.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yo.nszjky.cn

TS:   // 同 JS
来源：http://jl.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://hp.nicolike.cn

Go:   go f()
来源：http://dd.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://xs.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://hr.9csxet.cn

[O02] 使用线程池
来源：http://pd.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sm.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rf.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://kx.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ym.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rm.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kj.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lu.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bl.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ja.hahajie.cn

Py:   with lock: shared += 1
来源：http://fg.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://nz.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eb.bookmarksfly.cn

TS:   // 同 JS
来源：http://rm.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://xr.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tc.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ff.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ym.szsharing.cn

[O04] 定义异步函数并等待
来源：http://bh.521024.cn

Py:   async def f():⏎    await g()
来源：http://cj.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xc.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://sk.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vb.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://du.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vp.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hg.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ir.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://ef.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://tz.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ck.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://hc.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://jt.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ns.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kl.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://px.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yv.nszjky.cn

[O06] 使用进程池
来源：http://je.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ia.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pf.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://fo.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://xx.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kk.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ps.bookmarksfly.cn

Ruby: // fork 块
来源：http://ic.panjiajie.cn

C#:   Parallel.For
来源：http://zf.colortex.cn

================================================================================
来源：http://xo.huanxung.cn

P. 常用工具函数
来源：http://io.lnxyls.cn

================================================================================
来源：http://av.nicolike.cn

[P01] 生成 UUID
来源：http://ug.521024.cn

Py:   str(uuid.uuid4())
来源：http://ar.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://px.nszjky.cn

JS:   crypto.randomUUID()
来源：http://xm.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://fu.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://rl.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://ay.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://ww.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://st.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ni.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tj.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hp.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qv.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gp.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nm.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://is.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://my.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://di.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://jz.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ci.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ya.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sh.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://og.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ix.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kf.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cu.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qw.newstarts.cn

[P04] 求长度
来源：http://xb.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ww.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xp.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bf.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://kd.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://yj.szsharing.cn

Ruby: x.length;  x.size
来源：http://ci.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cw.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://xi.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ef.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yt.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ya.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zc.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iq.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ih.haigaiapp.cn

Ruby: a == b
来源：http://bk.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://an.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rs.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wa.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://ll.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oj.huanxung.cn

TS:   if (x == null) {}
来源：http://ax.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://up.shxzskj.cn

Go:   if x == nil {}
来源：http://vq.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gr.colortex.cn

C#:   if (x is null) {}
来源：http://rc.shxzukj.cn

[P07] 防抖与节流
来源：http://qf.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zr.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://ly.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wd.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xs.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dj.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gk.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ro.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://al.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://or.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sg.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://te.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dt.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xe.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xs.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nf.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://no.hahajie.cn

================================================================================
来源：http://ts.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ll.haigaiapp.cn

================================================================================
来源：http://ys.asd995.cn

[Q01] 创建表
来源：http://bp.bjjhwx.cn

CREATE TABLE users (
来源：http://fe.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gr.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://qs.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://dj.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ds.nicolike.cn

);
来源：http://at.hnjuh.cn

[Q02] 创建带外键的表
来源：http://gj.jctech888.com.cn

CREATE TABLE orders (
来源：http://pz.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://np.nicolike.cn

user_id INT NOT NULL,
来源：http://qf.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://br.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sm.chemitech.net.cn

);
来源：http://cg.nicolike.cn

[Q03] 增加列
来源：http://pb.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eu.chemitech.net.cn

[Q04] 修改列类型
来源：http://vk.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ys.asd995.cn

[Q05] 重命名列
来源：http://mc.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iq.wgjwhj.cn

[Q06] 删除列
来源：http://zv.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zm.newstarts.cn

[Q07] 删除表
来源：http://gk.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://yb.gzmigu.cn

[Q08] 创建普通索引
来源：http://qj.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gm.nicolike.cn

[Q09] 创建唯一索引
来源：http://xu.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dz.bookmarksfly.cn

[Q10] 插入单行
来源：http://bn.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uq.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://lm.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fe.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://sy.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lf.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vv.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://wq.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bd.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://ve.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ak.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ax.huixinmuqiang.cn

[Q15] 查询全部
来源：http://aa.shtwfgs.cn

SELECT * FROM users;
来源：http://sv.colortex.cn

[Q16] 查询指定列
来源：http://gr.colortex.cn

SELECT id, name FROM users;
来源：http://ln.panjiajie.cn

[Q17] 条件查询
来源：http://ru.asd995.cn


<!-- 参考信息 -->