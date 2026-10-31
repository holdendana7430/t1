代发 wailian999

TS:   process.platform;  process.version
来源：http://ad.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jg.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cm.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ht.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://er.szsharing.cn

================================================================================
来源：http://ul.wgjwhj.cn

N. 数据结构与算法
来源：http://tp.hahajie.cn

================================================================================
来源：http://qg.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://uu.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hp.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ks.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wh.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sn.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ve.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://il.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xw.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://km.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://vq.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://xb.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ok.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lq.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ir.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ry.colortex.cn

Go:   slices.Sort(arr)
来源：http://bz.hahajie.cn

Ruby: arr.sort
来源：http://bt.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eo.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://bf.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dc.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://oj.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wv.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yr.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gv.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ft.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pm.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cl.chemitech.net.cn

[N04] 斐波那契数列
来源：http://qm.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wo.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://er.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sk.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ov.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qk.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sm.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ct.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://le.panjiajie.cn

[N05] 最大公约数
来源：http://kq.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://kz.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jr.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hc.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dl.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uz.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wn.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://lg.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vd.shxzukj.cn

[N06] 判断回文字符串
来源：http://pv.huanxung.cn

Py:   s == s[::-1]
来源：http://pj.asd995.cn

PHP:  $s === strrev($s);
来源：http://al.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://sv.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://qq.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yg.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://ki.huixiangedu.cn

Ruby: s == s.reverse
来源：http://dj.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hi.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://ut.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qd.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cv.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gj.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://cj.jctech888.com.cn

Java: // 手写 HashMap
来源：http://rc.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://wp.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://mv.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yn.shtwfgs.cn

[N08] 生成全排列
来源：http://hj.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://kr.colortex.cn

PHP:  // 手写递归交换
来源：http://gx.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://ix.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ln.shxzukj.cn

Java: // 手写回溯递归
来源：http://if.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://tz.colortex.cn

Ruby: arr.permutation.to_a
来源：http://qs.asd995.cn

C#:   // 手写回溯递归
来源：http://si.haigaiapp.cn

[N09] 栈与队列
来源：http://lz.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gs.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qh.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yf.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xz.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cv.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mu.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tf.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hj.wgjwhj.cn

[N10] 链表节点定义
来源：http://zp.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qv.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vf.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xx.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gz.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://jf.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cr.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tk.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pg.huanxung.cn

[N11] 二叉树中序遍历
来源：http://yb.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dn.lnxyls.cn

PHP:  // 手写递归函数
来源：http://hu.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pu.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://to.nszjky.cn

Java: // 手写递归
来源：http://ea.shxzukj.cn

Go:   // 手写递归
来源：http://qo.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lt.hahajie.cn

C#:   // 手写递归
来源：http://ip.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jj.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gv.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jh.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ya.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cn.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bb.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nf.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nj.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fe.asd995.cn

================================================================================
来源：http://bw.chemitech.net.cn

O. 并发与异步
来源：http://rc.gzmigu.cn

================================================================================
来源：http://rl.jctech888.com.cn

[O01] 启动一个线程
来源：http://in.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qu.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zz.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jy.bjjhwx.cn

TS:   // 同 JS
来源：http://vu.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://om.shxzukj.cn

Go:   go f()
来源：http://po.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://fu.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://pw.szsharing.cn

[O02] 使用线程池
来源：http://nb.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iy.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rb.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://jg.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://ej.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://an.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lg.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xf.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xx.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://dz.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://ol.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://tk.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://na.nicolike.cn

TS:   // 同 JS
来源：http://vz.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://vt.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tk.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://af.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://lj.newstarts.cn

[O04] 定义异步函数并等待
来源：http://yg.521024.cn

Py:   async def f():⏎    await g()
来源：http://mm.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uw.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://gn.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ou.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fg.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ov.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yl.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://ek.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://vr.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://rc.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wz.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://uk.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://gp.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://el.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ez.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://li.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yd.newstarts.cn

[O06] 使用进程池
来源：http://rt.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qx.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sa.colortex.cn

JS:   // child_process / cluster 模块
来源：http://vf.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://xh.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xa.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xl.wgjwhj.cn

Ruby: // fork 块
来源：http://mc.colortex.cn

C#:   Parallel.For
来源：http://mh.yuexingan06.cn

================================================================================
来源：http://uw.haigaiapp.cn

P. 常用工具函数
来源：http://ca.colortex.cn

================================================================================
来源：http://hq.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://ye.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://in.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://di.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://gf.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://gf.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://ks.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://id.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://wv.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://wr.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://fr.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zo.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://px.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pd.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lz.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zv.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ue.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lm.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vv.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ci.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wo.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hh.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gn.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gf.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pp.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dl.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://og.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wf.nicolike.cn

[P04] 求长度
来源：http://lg.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pj.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rw.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qw.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vs.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://hl.asd995.cn

Go:   len(arr);  len(m)
来源：http://sv.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://hy.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ms.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://hg.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://id.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ih.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nz.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bs.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ci.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bg.szsharing.cn

Ruby: a == b
来源：http://ef.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uq.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oe.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zy.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://kk.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xs.nicolike.cn

TS:   if (x == null) {}
来源：http://zw.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wg.hnjuh.cn

Go:   if x == nil {}
来源：http://na.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pb.jctech888.com.cn

C#:   if (x is null) {}
来源：http://vy.chemitech.net.cn

[P07] 防抖与节流
来源：http://uj.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ep.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://yi.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ja.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hy.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jo.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jp.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qg.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xv.nszjky.cn

[P08] 处理浮点精度问题
来源：http://wo.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://he.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kg.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://om.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zh.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gv.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://de.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yg.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fp.shxzukj.cn

================================================================================
来源：http://sv.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ad.colortex.cn

================================================================================
来源：http://yy.panjiajie.cn

[Q01] 创建表
来源：http://sh.asd995.cn

CREATE TABLE users (
来源：http://ab.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mm.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://wr.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://vc.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ip.yuexingan06.cn

);
来源：http://ij.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://mb.wgjwhj.cn

CREATE TABLE orders (
来源：http://qp.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dc.newstarts.cn

user_id INT NOT NULL,
来源：http://ey.nicolike.cn

amount DECIMAL(10, 2),
来源：http://on.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yf.chemitech.net.cn

);
来源：http://gm.lnxyls.cn

[Q03] 增加列
来源：http://pq.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ck.yuexingan06.cn

[Q04] 修改列类型
来源：http://di.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sa.yuntaijiaju.cn

[Q05] 重命名列
来源：http://sv.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lf.shtwfgs.cn

[Q06] 删除列
来源：http://nx.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jj.lnxyls.cn

[Q07] 删除表
来源：http://rx.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://of.szsharing.cn

[Q08] 创建普通索引
来源：http://xr.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sx.521024.cn

[Q09] 创建唯一索引
来源：http://pi.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://da.muxihuayi.cn

[Q10] 插入单行
来源：http://td.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zb.jctech888.com.cn

[Q11] 一次插入多行
来源：http://qm.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gp.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://ol.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://su.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dp.szxytkj.cn

[Q13] 忽略重复插入
来源：http://rg.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vr.521024.cn

[Q14] 存在则更新（upsert）
来源：http://oc.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sv.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jx.jctech888.com.cn

[Q15] 查询全部
来源：http://pi.hahajie.cn

SELECT * FROM users;
来源：http://jp.jctech888.com.cn

[Q16] 查询指定列
来源：http://zn.521024.cn

SELECT id, name FROM users;
来源：http://wc.nicolike.cn

[Q17] 条件查询
来源：http://ex.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ii.szxytkj.cn

[Q18] 模糊匹配
来源：http://ju.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oi.nicolike.cn

[Q19] 范围查询
来源：http://hh.9csxet.cn


<!-- 参考信息 -->