代发 wailian999

[M08] 获取系统与运行时信息
来源：http://mn.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://tl.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ch.szsharing.cn

JS:   process.platform;  process.version
来源：http://wm.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://lq.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tv.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mh.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uz.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ao.521024.cn

================================================================================
来源：http://na.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ng.yuexingan06.cn

================================================================================
来源：http://ys.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://mn.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kd.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://px.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mb.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kv.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xk.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://lr.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fr.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nc.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gn.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://mr.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ir.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dc.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ux.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yo.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://up.asd995.cn

Ruby: arr.sort
来源：http://ox.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pa.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://rr.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bt.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://iv.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vj.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hv.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gd.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://si.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yp.bjjhwx.cn

[N04] 斐波那契数列
来源：http://vm.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vp.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dj.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vi.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://du.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cl.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://au.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ew.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vc.bjjhwx.cn

[N05] 最大公约数
来源：http://yb.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://rs.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hk.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://te.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kv.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bl.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lo.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://lo.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://is.asd995.cn

[N06] 判断回文字符串
来源：http://od.gzmigu.cn

Py:   s == s[::-1]
来源：http://gl.hahajie.cn

PHP:  $s === strrev($s);
来源：http://fv.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://rr.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ij.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nf.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://tc.haigaiapp.cn

Ruby: s == s.reverse
来源：http://cq.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zn.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://dl.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qj.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jd.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sv.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://dv.lnxyls.cn

Java: // 手写 HashMap
来源：http://et.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ap.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://uv.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xq.szsharing.cn

[N08] 生成全排列
来源：http://xi.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://dj.521024.cn

PHP:  // 手写递归交换
来源：http://an.521024.cn

JS:   // 手写回溯递归
来源：http://kn.panjiajie.cn

TS:   // 手写回溯递归
来源：http://td.muxihuayi.cn

Java: // 手写回溯递归
来源：http://gt.newstarts.cn

Go:   // 手写回溯递归
来源：http://fz.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://ve.9csxet.cn

C#:   // 手写回溯递归
来源：http://uq.hnjuh.cn

[N09] 栈与队列
来源：http://jv.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xz.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bz.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fk.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dw.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rw.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xo.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vq.bookmarksfly.cn

[N10] 链表节点定义
来源：http://zj.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cr.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://au.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ym.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://se.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://rf.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://np.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hg.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lz.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://iz.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ns.shxzukj.cn

PHP:  // 手写递归函数
来源：http://sn.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tw.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mw.huanxung.cn

Java: // 手写递归
来源：http://qi.yuexingan06.cn

Go:   // 手写递归
来源：http://xc.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vr.lnxyls.cn

C#:   // 手写递归
来源：http://ty.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sa.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fd.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nf.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gf.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xi.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mx.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zr.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dc.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://go.asd995.cn

================================================================================
来源：http://ss.jianghongdianzi.cn

O. 并发与异步
来源：http://sa.muxihuayi.cn

================================================================================
来源：http://ik.hahajie.cn

[O01] 启动一个线程
来源：http://oe.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sk.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yc.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://et.hahajie.cn

TS:   // 同 JS
来源：http://nn.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://fv.shxzukj.cn

Go:   go f()
来源：http://es.lnxyls.cn

Ruby: Thread.new { f }
来源：http://li.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://xd.nszjky.cn

[O02] 使用线程池
来源：http://la.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fo.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gd.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ws.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://lw.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rf.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://im.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gi.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ae.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://sq.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://or.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://rn.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ar.colortex.cn

TS:   // 同 JS
来源：http://jy.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://wy.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wn.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wu.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://xq.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://xg.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://ij.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zq.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://wo.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yt.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ym.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nk.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://os.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://we.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://xl.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://gn.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mp.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://bt.asd995.cn

TS:   await Promise.all(tasks)
来源：http://dz.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hw.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rt.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://kv.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qs.yuexingan06.cn

[O06] 使用进程池
来源：http://lp.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oi.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sk.asd995.cn

JS:   // child_process / cluster 模块
来源：http://sl.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://tn.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://by.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dz.shtwfgs.cn

Ruby: // fork 块
来源：http://zc.szxytkj.cn

C#:   Parallel.For
来源：http://fc.muxihuayi.cn

================================================================================
来源：http://by.panjiajie.cn

P. 常用工具函数
来源：http://st.wgjwhj.cn

================================================================================
来源：http://tg.lnxyls.cn

[P01] 生成 UUID
来源：http://bq.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://qc.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://in.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://up.hahajie.cn

TS:   crypto.randomUUID()
来源：http://uv.521024.cn

Java: UUID.randomUUID().toString()
来源：http://cx.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://so.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://jd.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://tv.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ds.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yz.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jd.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ub.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kg.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lx.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rd.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ot.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ol.szsharing.cn

[P03] 生成短随机字符串
来源：http://dm.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qk.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xw.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ah.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lq.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bc.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ae.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://no.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ii.nicolike.cn

[P04] 求长度
来源：http://bn.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wl.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fh.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zi.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://ms.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://om.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://gi.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kd.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://yl.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nv.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ry.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sj.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pf.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tm.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xq.lnxyls.cn

Ruby: a == b
来源：http://xp.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://du.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://in.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fi.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://me.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fw.nicolike.cn

TS:   if (x == null) {}
来源：http://io.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zn.colortex.cn

Go:   if x == nil {}
来源：http://tg.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dp.shxzukj.cn

C#:   if (x is null) {}
来源：http://tv.huanxung.cn

[P07] 防抖与节流
来源：http://tf.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tr.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ru.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tb.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pn.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bu.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oj.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vt.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://td.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://da.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iq.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yp.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zr.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hy.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nw.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pp.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ju.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ab.jctech888.com.cn

================================================================================
来源：http://ce.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pk.asd995.cn

================================================================================
来源：http://kz.nszjky.cn

[Q01] 创建表
来源：http://ie.jctech888.com.cn

CREATE TABLE users (
来源：http://ta.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ut.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://iq.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://pp.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yn.yuntaijiaju.cn

);
来源：http://wc.colortex.cn

[Q02] 创建带外键的表
来源：http://tg.huanxung.cn

CREATE TABLE orders (
来源：http://gt.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vl.huanxung.cn

user_id INT NOT NULL,
来源：http://sh.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://sv.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://au.shxzskj.cn

);
来源：http://zm.chemitech.net.cn

[Q03] 增加列
来源：http://im.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ro.521024.cn

[Q04] 修改列类型
来源：http://yr.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lk.gzmigu.cn

[Q05] 重命名列
来源：http://gz.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gl.521024.cn

[Q06] 删除列
来源：http://hu.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xi.hahajie.cn

[Q07] 删除表
来源：http://bk.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://iw.shxzukj.cn

[Q08] 创建普通索引
来源：http://ja.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wv.shxzskj.cn

[Q09] 创建唯一索引
来源：http://gi.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lv.hnjuh.cn

[Q10] 插入单行
来源：http://za.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ib.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://wm.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://np.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://zl.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oy.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gk.huanxung.cn

[Q13] 忽略重复插入
来源：http://ft.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wj.521024.cn

[Q14] 存在则更新（upsert）
来源：http://jf.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://df.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://px.yuntaijiaju.cn

[Q15] 查询全部
来源：http://ts.hnjuh.cn

SELECT * FROM users;
来源：http://xh.lnxyls.cn

[Q16] 查询指定列
来源：http://zs.yuexingan06.cn

SELECT id, name FROM users;
来源：http://mu.huixiangedu.cn

[Q17] 条件查询
来源：http://at.hnjuh.cn


<!-- 参考信息 -->