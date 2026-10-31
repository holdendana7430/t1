代发 wailian999

[M08] 获取系统与运行时信息
来源：http://rd.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ov.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://hy.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://yl.szsharing.cn

TS:   process.platform;  process.version
来源：http://ju.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ts.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eg.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gz.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eh.haigaiapp.cn

================================================================================
来源：http://yy.shxzskj.cn

N. 数据结构与算法
来源：http://hi.yuntaijiaju.cn

================================================================================
来源：http://gy.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://jv.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rp.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pw.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fo.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bm.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://qr.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hn.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ke.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://gu.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ip.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ks.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xe.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yj.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lf.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://pe.yuntaijiaju.cn

Ruby: arr.sort
来源：http://km.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yj.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://gz.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hs.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ev.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fd.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bm.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://el.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rm.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xl.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xc.asd995.cn

[N04] 斐波那契数列
来源：http://sy.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cf.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jt.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kg.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ln.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ln.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hn.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ij.asd995.cn

[N05] 最大公约数
来源：http://nc.9csxet.cn

Py:   math.gcd(a, b)
来源：http://dj.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ew.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oc.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://db.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://si.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uq.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://km.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mp.huixiangedu.cn

[N06] 判断回文字符串
来源：http://oi.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://vf.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://fb.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://qg.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://pl.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ui.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://dm.gzmigu.cn

Ruby: s == s.reverse
来源：http://tx.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://th.colortex.cn

[N07] 两数之和（返回下标）
来源：http://ns.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://he.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gu.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cn.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://ta.lnxyls.cn

Java: // 手写 HashMap
来源：http://wx.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://hv.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://or.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rv.bookmarksfly.cn

[N08] 生成全排列
来源：http://kz.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://bc.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://qx.nszjky.cn

JS:   // 手写回溯递归
来源：http://dg.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://lg.bjjhwx.cn

Java: // 手写回溯递归
来源：http://ml.hahajie.cn

Go:   // 手写回溯递归
来源：http://yf.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://xe.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://yq.colortex.cn

[N09] 栈与队列
来源：http://fw.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fg.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ys.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gu.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vw.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://to.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://if.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mf.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xp.panjiajie.cn

[N10] 链表节点定义
来源：http://te.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qn.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tb.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vw.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uw.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://rn.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aa.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jg.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fq.nszjky.cn

[N11] 二叉树中序遍历
来源：http://qe.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yj.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://tg.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cp.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://es.wgjwhj.cn

Java: // 手写递归
来源：http://jt.nicolike.cn

Go:   // 手写递归
来源：http://kx.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ym.9csxet.cn

C#:   // 手写递归
来源：http://es.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ou.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://or.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ok.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qd.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uz.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jc.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tv.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hd.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sm.panjiajie.cn

================================================================================
来源：http://af.yuexingan06.cn

O. 并发与异步
来源：http://th.yuexingan06.cn

================================================================================
来源：http://bn.shtwfgs.cn

[O01] 启动一个线程
来源：http://tj.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xz.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pk.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lo.yuexingan06.cn

TS:   // 同 JS
来源：http://ex.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://xw.jctech888.com.cn

Go:   go f()
来源：http://ho.asd995.cn

Ruby: Thread.new { f }
来源：http://wk.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://zl.jctech888.com.cn

[O02] 使用线程池
来源：http://wx.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dm.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zd.huanxung.cn

JS:   // worker_threads 线程池
来源：http://qe.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://qd.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://og.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bq.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gb.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pn.hahajie.cn

[O03] 加锁保护共享数据
来源：http://as.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://rp.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://ch.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rl.chemitech.net.cn

TS:   // 同 JS
来源：http://np.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://rz.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://at.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fb.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://hj.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://fu.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://el.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pi.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://la.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ra.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mh.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://en.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jn.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://te.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://pp.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://nf.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wj.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://dy.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://ar.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bz.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cs.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://xc.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fb.nszjky.cn

[O06] 使用进程池
来源：http://dc.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bb.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fl.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://js.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://of.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bp.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://py.nicolike.cn

Ruby: // fork 块
来源：http://oj.chemitech.net.cn

C#:   Parallel.For
来源：http://km.muxihuayi.cn

================================================================================
来源：http://zx.521024.cn

P. 常用工具函数
来源：http://vy.shxzukj.cn

================================================================================
来源：http://tz.panjiajie.cn

[P01] 生成 UUID
来源：http://fz.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://kj.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bu.9csxet.cn

JS:   crypto.randomUUID()
来源：http://sx.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://iu.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://pn.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://wo.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://qo.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://sz.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://vw.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vt.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xv.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://px.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://df.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gx.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rs.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gb.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iq.szxytkj.cn

[P03] 生成短随机字符串
来源：http://dd.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lp.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cc.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kr.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://en.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jz.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hl.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bz.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dj.hnjuh.cn

[P04] 求长度
来源：http://oy.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nv.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tj.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zd.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ly.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://fc.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://hz.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://pi.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bs.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://hx.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ds.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qf.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jm.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kk.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://az.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mi.hnjuh.cn

Ruby: a == b
来源：http://gj.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eg.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bd.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qx.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://hp.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://is.panjiajie.cn

TS:   if (x == null) {}
来源：http://zi.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sm.yuexingan06.cn

Go:   if x == nil {}
来源：http://pb.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://me.bjjhwx.cn

C#:   if (x is null) {}
来源：http://tp.yuexingan06.cn

[P07] 防抖与节流
来源：http://wd.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qm.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://vr.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jh.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://om.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://he.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pn.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kh.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lq.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://gs.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ue.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ca.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pp.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://er.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pc.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ty.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ps.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wa.huixiangedu.cn

================================================================================
来源：http://ua.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uh.hahajie.cn

================================================================================
来源：http://ca.yuexingan06.cn

[Q01] 创建表
来源：http://xk.asd995.cn

CREATE TABLE users (
来源：http://gn.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zi.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://zk.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://yd.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ik.yuexingan06.cn

);
来源：http://mm.nicolike.cn

[Q02] 创建带外键的表
来源：http://lx.huixiangedu.cn

CREATE TABLE orders (
来源：http://ia.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://en.panjiajie.cn

user_id INT NOT NULL,
来源：http://kc.521024.cn

amount DECIMAL(10, 2),
来源：http://yy.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ko.colortex.cn

);
来源：http://jj.szsharing.cn

[Q03] 增加列
来源：http://jg.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rc.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://yt.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ap.huixinmuqiang.cn

[Q05] 重命名列
来源：http://us.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ck.bjjhwx.cn

[Q06] 删除列
来源：http://hz.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://db.asd995.cn

[Q07] 删除表
来源：http://kp.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://bi.newstarts.cn

[Q08] 创建普通索引
来源：http://lk.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ap.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://wu.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://es.huixiangedu.cn

[Q10] 插入单行
来源：http://vd.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lc.jctech888.com.cn

[Q11] 一次插入多行
来源：http://bx.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bv.colortex.cn

[Q12] 插入后取自增 ID
来源：http://cf.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://no.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kb.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://wy.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pv.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://kb.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sm.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zh.nszjky.cn

[Q15] 查询全部
来源：http://wq.asd995.cn

SELECT * FROM users;
来源：http://iu.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://tn.szsharing.cn

SELECT id, name FROM users;
来源：http://tx.haigaiapp.cn

[Q17] 条件查询
来源：http://vo.gzmigu.cn


<!-- 参考信息 -->