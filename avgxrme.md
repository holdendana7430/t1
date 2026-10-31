代发 wailian999

[M08] 获取系统与运行时信息
来源：http://oe.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://en.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://qp.colortex.cn

JS:   process.platform;  process.version
来源：http://sz.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://gs.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uf.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fk.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sm.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ze.huixiangedu.cn

================================================================================
来源：http://cn.shtwfgs.cn

N. 数据结构与算法
来源：http://bx.newstarts.cn

================================================================================
来源：http://mh.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://kx.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ce.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yb.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rm.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zp.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://tf.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bq.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gl.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://st.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qk.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ni.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dw.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mc.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://an.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://dv.jianghongdianzi.cn

Ruby: arr.sort
来源：http://jv.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zi.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ot.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ah.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://tf.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mg.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ne.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ug.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mm.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hs.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ct.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://cf.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://da.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ja.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://th.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gf.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ay.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pu.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fo.huanxung.cn

[N05] 最大公约数
来源：http://tg.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://dm.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gs.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gx.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wc.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://li.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ts.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://cb.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vd.haigaiapp.cn

[N06] 判断回文字符串
来源：http://xc.huixiangedu.cn

Py:   s == s[::-1]
来源：http://ru.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://ee.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ej.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://kx.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qv.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://xf.haigaiapp.cn

Ruby: s == s.reverse
来源：http://oa.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://se.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://qe.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gg.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nz.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lq.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://wt.szsharing.cn

Java: // 手写 HashMap
来源：http://fd.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://xl.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://kd.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lh.9csxet.cn

[N08] 生成全排列
来源：http://qu.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://cc.521024.cn

PHP:  // 手写递归交换
来源：http://bx.shxzukj.cn

JS:   // 手写回溯递归
来源：http://bz.szxytkj.cn

TS:   // 手写回溯递归
来源：http://tx.9csxet.cn

Java: // 手写回溯递归
来源：http://ms.panjiajie.cn

Go:   // 手写回溯递归
来源：http://yk.521024.cn

Ruby: arr.permutation.to_a
来源：http://uq.9csxet.cn

C#:   // 手写回溯递归
来源：http://kg.huixinmuqiang.cn

[N09] 栈与队列
来源：http://wq.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jt.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fo.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zr.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fc.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qu.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bs.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vt.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qk.wgjwhj.cn

[N10] 链表节点定义
来源：http://vn.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ku.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zy.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hs.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://er.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://pv.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fh.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zm.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hh.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://ad.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bc.panjiajie.cn

PHP:  // 手写递归函数
来源：http://ex.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://em.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xn.gzmigu.cn

Java: // 手写递归
来源：http://di.bjjhwx.cn

Go:   // 手写递归
来源：http://gk.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dy.jianghongdianzi.cn

C#:   // 手写递归
来源：http://jq.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://et.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mu.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nu.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://di.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://df.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lw.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ox.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ca.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ul.shxzukj.cn

================================================================================
来源：http://gn.wgjwhj.cn

O. 并发与异步
来源：http://ea.panjiajie.cn

================================================================================
来源：http://do.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://vs.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mv.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lk.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cy.wgjwhj.cn

TS:   // 同 JS
来源：http://dl.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://bb.hahajie.cn

Go:   go f()
来源：http://zf.hnjuh.cn

Ruby: Thread.new { f }
来源：http://gi.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://jm.chemitech.net.cn

[O02] 使用线程池
来源：http://mm.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://em.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vd.huanxung.cn

JS:   // worker_threads 线程池
来源：http://km.9csxet.cn

TS:   // worker_threads 线程池
来源：http://ul.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bu.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://va.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://al.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dm.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://wa.lnxyls.cn

Py:   with lock: shared += 1
来源：http://gm.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ff.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fy.haigaiapp.cn

TS:   // 同 JS
来源：http://du.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://ex.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nu.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cr.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://ib.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://uo.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://kg.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rh.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://lz.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kr.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://va.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jw.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zx.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://ey.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://dk.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://lb.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://et.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://ca.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://yi.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yp.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ub.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://su.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ca.yuntaijiaju.cn

[O06] 使用进程池
来源：http://qp.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wq.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pw.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://gk.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://fy.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ae.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ya.bjjhwx.cn

Ruby: // fork 块
来源：http://ku.shxzskj.cn

C#:   Parallel.For
来源：http://ky.gzmigu.cn

================================================================================
来源：http://mx.huixiangedu.cn

P. 常用工具函数
来源：http://wb.huixiangedu.cn

================================================================================
来源：http://ic.bjjhwx.cn

[P01] 生成 UUID
来源：http://uv.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://qm.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dj.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://fk.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://im.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://hj.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://ww.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://oc.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://jm.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://go.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ys.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://to.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uh.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://af.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://su.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ur.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fl.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tj.newstarts.cn

[P03] 生成短随机字符串
来源：http://ve.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tx.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kl.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hx.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hs.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://td.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cr.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rt.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ng.haigaiapp.cn

[P04] 求长度
来源：http://dt.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nx.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://te.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ht.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ih.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://rs.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://ni.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ms.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sw.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://zn.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cg.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fq.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ch.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zt.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xw.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ll.nszjky.cn

Ruby: a == b
来源：http://ek.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fv.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eb.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rk.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://wt.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oq.jctech888.com.cn

TS:   if (x == null) {}
来源：http://wu.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lj.newstarts.cn

Go:   if x == nil {}
来源：http://jj.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ny.huanxung.cn

C#:   if (x is null) {}
来源：http://oj.gzmigu.cn

[P07] 防抖与节流
来源：http://nr.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mp.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://hz.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pp.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sq.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nj.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://au.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vh.9csxet.cn

[P08] 处理浮点精度问题
来源：http://es.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mh.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qg.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ol.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://of.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wo.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wd.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yn.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kt.nicolike.cn

================================================================================
来源：http://fj.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lt.shxzukj.cn

================================================================================
来源：http://my.colortex.cn

[Q01] 创建表
来源：http://tl.nicolike.cn

CREATE TABLE users (
来源：http://bz.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ez.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://df.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://mp.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jn.521024.cn

);
来源：http://gu.asd995.cn

[Q02] 创建带外键的表
来源：http://ut.9csxet.cn

CREATE TABLE orders (
来源：http://ea.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kn.bjjhwx.cn

user_id INT NOT NULL,
来源：http://eu.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://dj.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gp.huixinmuqiang.cn

);
来源：http://zj.huanxung.cn

[Q03] 增加列
来源：http://lx.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rx.9csxet.cn

[Q04] 修改列类型
来源：http://xw.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rz.chemitech.net.cn

[Q05] 重命名列
来源：http://sn.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fj.9csxet.cn

[Q06] 删除列
来源：http://ms.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vt.hahajie.cn

[Q07] 删除表
来源：http://md.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://jn.szxytkj.cn

[Q08] 创建普通索引
来源：http://jg.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dp.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://jq.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cq.shxzskj.cn

[Q10] 插入单行
来源：http://zr.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://st.9csxet.cn

[Q11] 一次插入多行
来源：http://av.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kv.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://fu.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ro.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jt.gzmigu.cn

[Q13] 忽略重复插入
来源：http://vd.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zw.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://ti.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ar.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vj.szxytkj.cn

[Q15] 查询全部
来源：http://ze.chemitech.net.cn

SELECT * FROM users;
来源：http://vf.colortex.cn

[Q16] 查询指定列
来源：http://jv.bjjhwx.cn

SELECT id, name FROM users;
来源：http://xj.hnjuh.cn

[Q17] 条件查询
来源：http://jd.colortex.cn


<!-- 参考信息 -->