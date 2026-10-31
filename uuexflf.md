代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ph.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://tr.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://nq.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://dn.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ga.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://za.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://db.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ib.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lg.szxytkj.cn

================================================================================
来源：http://ff.nicolike.cn

N. 数据结构与算法
来源：http://aj.521024.cn

================================================================================
来源：http://at.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://cn.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://up.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qb.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jc.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ec.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ah.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hs.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ek.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://pl.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://dd.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pc.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://no.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bo.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eg.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://gy.colortex.cn

Ruby: arr.sort
来源：http://it.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ny.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://dq.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qo.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://ya.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vk.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bc.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tc.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tk.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yn.jctech888.com.cn

[N04] 斐波那契数列
来源：http://dv.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hd.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vn.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yb.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ih.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kv.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fg.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nr.huixiangedu.cn

[N05] 最大公约数
来源：http://ac.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://kr.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kk.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ei.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wj.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ct.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ay.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ra.hnjuh.cn

[N06] 判断回文字符串
来源：http://vd.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://np.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://kk.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://og.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://xu.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dn.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://bh.shxzskj.cn

Ruby: s == s.reverse
来源：http://se.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vu.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://jr.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vx.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ne.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ln.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://lq.nszjky.cn

Java: // 手写 HashMap
来源：http://ok.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://mc.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://cz.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yt.shtwfgs.cn

[N08] 生成全排列
来源：http://hz.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://rm.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://tl.nicolike.cn

JS:   // 手写回溯递归
来源：http://nu.shxzukj.cn

TS:   // 手写回溯递归
来源：http://xl.gzmigu.cn

Java: // 手写回溯递归
来源：http://jn.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://nm.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://qx.9csxet.cn

C#:   // 手写回溯递归
来源：http://wv.szsharing.cn

[N09] 栈与队列
来源：http://oz.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lg.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dk.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ww.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bz.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ey.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vi.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jn.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vi.hnjuh.cn

[N10] 链表节点定义
来源：http://rz.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gj.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ky.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oq.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mo.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://ps.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ck.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dr.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wb.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://ln.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ts.szxytkj.cn

PHP:  // 手写递归函数
来源：http://ul.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ut.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yd.bookmarksfly.cn

Java: // 手写递归
来源：http://tk.shtwfgs.cn

Go:   // 手写递归
来源：http://io.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zy.gzmigu.cn

C#:   // 手写递归
来源：http://ok.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vd.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bt.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://la.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cy.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ek.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vc.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xd.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nt.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tg.shtwfgs.cn

================================================================================
来源：http://fv.shtwfgs.cn

O. 并发与异步
来源：http://sv.haigaiapp.cn

================================================================================
来源：http://pz.9csxet.cn

[O01] 启动一个线程
来源：http://he.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ms.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rh.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nl.yuntaijiaju.cn

TS:   // 同 JS
来源：http://nv.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://gi.gzmigu.cn

Go:   go f()
来源：http://ob.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://rv.huanxung.cn

C#:   Task.Run(() => F());
来源：http://pn.nszjky.cn

[O02] 使用线程池
来源：http://pl.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gd.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kv.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ba.szsharing.cn

TS:   // worker_threads 线程池
来源：http://fi.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vy.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://to.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dr.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://us.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://sm.9csxet.cn

Py:   with lock: shared += 1
来源：http://mb.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://io.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nk.yuexingan06.cn

TS:   // 同 JS
来源：http://ry.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://yk.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vt.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lt.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://jx.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://mu.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://uu.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pw.521024.cn

JS:   async function f() { await g(); }
来源：http://uv.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ow.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tq.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kr.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dq.colortex.cn

C#:   async Task F() { await G(); }
来源：http://xh.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://wq.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://tc.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ld.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://tf.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://wk.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aj.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tz.hahajie.cn

Ruby: threads.map(&:join)
来源：http://py.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yd.huixinmuqiang.cn

[O06] 使用进程池
来源：http://nn.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gl.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ip.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://zd.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://tq.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://op.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fd.newstarts.cn

Ruby: // fork 块
来源：http://kq.shxzskj.cn

C#:   Parallel.For
来源：http://vh.lnxyls.cn

================================================================================
来源：http://tm.asd995.cn

P. 常用工具函数
来源：http://kz.newstarts.cn

================================================================================
来源：http://jk.panjiajie.cn

[P01] 生成 UUID
来源：http://tz.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://et.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ac.nicolike.cn

JS:   crypto.randomUUID()
来源：http://bf.9csxet.cn

TS:   crypto.randomUUID()
来源：http://we.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://fd.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://rg.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://kn.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://cx.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://hc.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://md.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tw.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oq.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ha.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zy.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hc.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://og.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lm.panjiajie.cn

[P03] 生成短随机字符串
来源：http://nt.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vl.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zs.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yx.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ov.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xb.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mb.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mq.shxzukj.cn

[P04] 求长度
来源：http://fo.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nv.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uz.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wn.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ae.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://wy.hahajie.cn

Go:   len(arr);  len(m)
来源：http://xw.asd995.cn

Ruby: x.length;  x.size
来源：http://rt.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://od.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://vq.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://le.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dt.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fj.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vb.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vi.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fi.muxihuayi.cn

Ruby: a == b
来源：http://pk.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rk.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pw.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zv.521024.cn

PHP:  if (empty($x)) {}
来源：http://yt.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xz.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://ng.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ea.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://jz.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ug.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ou.newstarts.cn

[P07] 防抖与节流
来源：http://uz.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yo.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://pz.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fo.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pi.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gq.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sl.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://xw.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mm.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://on.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tz.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pv.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mo.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xb.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hl.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hl.yuexingan06.cn

================================================================================
来源：http://ws.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ml.szsharing.cn

================================================================================
来源：http://cm.521024.cn

[Q01] 创建表
来源：http://tc.panjiajie.cn

CREATE TABLE users (
来源：http://gx.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jp.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://bs.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ta.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vf.jctech888.com.cn

);
来源：http://ia.gzmigu.cn

[Q02] 创建带外键的表
来源：http://wz.colortex.cn

CREATE TABLE orders (
来源：http://bh.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fc.chemitech.net.cn

user_id INT NOT NULL,
来源：http://vm.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://wg.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kl.szsharing.cn

);
来源：http://qd.newstarts.cn

[Q03] 增加列
来源：http://lf.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://la.bookmarksfly.cn

[Q04] 修改列类型
来源：http://aq.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rn.bjjhwx.cn

[Q05] 重命名列
来源：http://bl.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://da.yuexingan06.cn

[Q06] 删除列
来源：http://pq.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fr.szxytkj.cn

[Q07] 删除表
来源：http://ls.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://bh.hahajie.cn

[Q08] 创建普通索引
来源：http://ec.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oe.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://rs.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vg.gzmigu.cn

[Q10] 插入单行
来源：http://kc.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ak.nszjky.cn

[Q11] 一次插入多行
来源：http://sn.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yw.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ey.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pk.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sn.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://rl.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ui.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ci.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ah.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://po.hnjuh.cn

[Q15] 查询全部
来源：http://ju.hnjuh.cn

SELECT * FROM users;
来源：http://ag.newstarts.cn

[Q16] 查询指定列
来源：http://rm.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://wz.huanxung.cn

[Q17] 条件查询
来源：http://ml.shxzukj.cn


<!-- 参考信息 -->