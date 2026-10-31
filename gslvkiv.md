代发 wailian999

[M08] 获取系统与运行时信息
来源：http://dm.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ss.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://ui.panjiajie.cn

JS:   process.platform;  process.version
来源：http://sa.colortex.cn

TS:   process.platform;  process.version
来源：http://hf.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qj.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ex.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lz.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pp.shxzskj.cn

================================================================================
来源：http://wi.9csxet.cn

N. 数据结构与算法
来源：http://dg.wgjwhj.cn

================================================================================
来源：http://em.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://cp.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ad.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://po.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://el.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ge.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hp.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://yu.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://le.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uy.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://vz.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ok.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ks.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aq.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iw.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jz.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://vw.huixiangedu.cn

Ruby: arr.sort
来源：http://hh.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pa.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://wp.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yq.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://lb.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pe.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bj.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dw.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uu.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ib.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://un.szsharing.cn

[N04] 斐波那契数列
来源：http://zy.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ep.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sz.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ao.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vu.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tt.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yo.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qc.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kx.lnxyls.cn

[N05] 最大公约数
来源：http://dr.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ju.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://us.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yg.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ho.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ll.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://yu.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vc.szsharing.cn

[N06] 判断回文字符串
来源：http://kj.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ef.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://ce.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://nu.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://ta.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ig.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://rw.wgjwhj.cn

Ruby: s == s.reverse
来源：http://vy.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qc.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://nx.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mi.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pc.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hr.521024.cn

TS:   // 手写 Map<string, number>
来源：http://hs.muxihuayi.cn

Java: // 手写 HashMap
来源：http://sv.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://di.521024.cn

Ruby: // 手写 Hash
来源：http://ij.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zr.shxzskj.cn

[N08] 生成全排列
来源：http://zt.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://qk.shxzskj.cn

PHP:  // 手写递归交换
来源：http://cl.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ur.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://th.shxzskj.cn

Java: // 手写回溯递归
来源：http://qf.newstarts.cn

Go:   // 手写回溯递归
来源：http://yy.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://er.shxzukj.cn

C#:   // 手写回溯递归
来源：http://aw.hnjuh.cn

[N09] 栈与队列
来源：http://yf.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://du.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ey.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://af.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yl.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ja.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eo.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pv.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rl.gzmigu.cn

[N10] 链表节点定义
来源：http://qa.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sa.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://da.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xw.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mk.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://ud.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vz.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ps.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://by.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://rc.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qt.nicolike.cn

PHP:  // 手写递归函数
来源：http://in.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fy.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wj.wgjwhj.cn

Java: // 手写递归
来源：http://kh.521024.cn

Go:   // 手写递归
来源：http://dz.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dr.gzmigu.cn

C#:   // 手写递归
来源：http://ia.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xi.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ym.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dc.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://na.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ko.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ka.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sa.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oo.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dc.hahajie.cn

================================================================================
来源：http://oe.nszjky.cn

O. 并发与异步
来源：http://ry.hnjuh.cn

================================================================================
来源：http://iw.gzmigu.cn

[O01] 启动一个线程
来源：http://ty.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ax.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rn.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fc.shtwfgs.cn

TS:   // 同 JS
来源：http://ns.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ev.muxihuayi.cn

Go:   go f()
来源：http://wz.gzmigu.cn

Ruby: Thread.new { f }
来源：http://ya.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://eh.yuntaijiaju.cn

[O02] 使用线程池
来源：http://os.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qy.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ez.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://mf.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://ng.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lu.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lg.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ox.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cm.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://ts.hnjuh.cn

Py:   with lock: shared += 1
来源：http://vg.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://xm.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yy.hnjuh.cn

TS:   // 同 JS
来源：http://ci.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://vj.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dh.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gu.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://zd.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://dm.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://kn.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xy.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://rf.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yi.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://om.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://je.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ec.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://ln.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://vf.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ov.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gk.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://px.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://oj.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rx.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cp.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://ol.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lk.chemitech.net.cn

[O06] 使用进程池
来源：http://nm.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xh.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://we.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://sw.asd995.cn

TS:   // child_process / cluster 模块
来源：http://bq.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ez.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xl.shxzskj.cn

Ruby: // fork 块
来源：http://ue.nszjky.cn

C#:   Parallel.For
来源：http://pg.9csxet.cn

================================================================================
来源：http://rs.jianghongdianzi.cn

P. 常用工具函数
来源：http://yq.asd995.cn

================================================================================
来源：http://ov.jctech888.com.cn

[P01] 生成 UUID
来源：http://pk.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://pw.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dv.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ms.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ul.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://lq.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://gw.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://yr.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://hc.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ut.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qv.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://er.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gy.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gn.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qh.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gx.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hn.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wz.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://vw.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ms.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qe.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vr.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qv.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://py.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xp.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ub.yuexingan06.cn

[P04] 求长度
来源：http://vl.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://co.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jk.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eq.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ay.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://rz.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://nn.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ot.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fh.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ao.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qd.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lq.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lg.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oz.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://se.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xk.szxytkj.cn

Ruby: a == b
来源：http://xk.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yv.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vw.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kg.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://nr.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://az.wgjwhj.cn

TS:   if (x == null) {}
来源：http://vx.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ss.wgjwhj.cn

Go:   if x == nil {}
来源：http://oj.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bd.haigaiapp.cn

C#:   if (x is null) {}
来源：http://zg.colortex.cn

[P07] 防抖与节流
来源：http://vz.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oc.521024.cn

PHP:  // 手写时间戳比较
来源：http://bj.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fg.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bv.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fk.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qj.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://en.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://em.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://mi.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cg.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://et.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uc.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wb.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jc.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yg.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://en.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://li.shxzskj.cn

================================================================================
来源：http://al.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bt.lnxyls.cn

================================================================================
来源：http://id.lnxyls.cn

[Q01] 创建表
来源：http://jy.szsharing.cn

CREATE TABLE users (
来源：http://hx.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zp.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://wq.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://on.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ce.jianghongdianzi.cn

);
来源：http://fl.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://ax.nszjky.cn

CREATE TABLE orders (
来源：http://je.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kc.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://el.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://tp.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cq.lnxyls.cn

);
来源：http://lw.huixinmuqiang.cn

[Q03] 增加列
来源：http://qo.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fy.shxzukj.cn

[Q04] 修改列类型
来源：http://vs.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qq.asd995.cn

[Q05] 重命名列
来源：http://aq.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mm.yuntaijiaju.cn

[Q06] 删除列
来源：http://st.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://af.shxzskj.cn

[Q07] 删除表
来源：http://hd.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://nm.szxytkj.cn

[Q08] 创建普通索引
来源：http://tu.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qy.asd995.cn

[Q09] 创建唯一索引
来源：http://bd.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mj.chemitech.net.cn

[Q10] 插入单行
来源：http://si.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wo.muxihuayi.cn

[Q11] 一次插入多行
来源：http://bp.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vn.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://bu.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ww.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xm.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://ud.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ds.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://qv.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ft.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gj.shxzukj.cn

[Q15] 查询全部
来源：http://xu.muxihuayi.cn

SELECT * FROM users;
来源：http://ao.gzmigu.cn

[Q16] 查询指定列
来源：http://ro.newstarts.cn

SELECT id, name FROM users;
来源：http://ns.521024.cn

[Q17] 条件查询
来源：http://ig.jianghongdianzi.cn


<!-- 参考信息 -->