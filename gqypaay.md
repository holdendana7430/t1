代发 wailian999

TS:   process.platform;  process.version
来源：http://iv.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://my.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yb.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jo.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://va.nicolike.cn

================================================================================
来源：http://fs.lnxyls.cn

N. 数据结构与算法
来源：http://ki.muxihuayi.cn

================================================================================
来源：http://mn.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://yf.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dl.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bn.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yi.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yr.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oc.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://pk.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://af.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qa.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zr.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ig.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gv.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mu.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tf.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dy.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://hj.hahajie.cn

Ruby: arr.sort
来源：http://zw.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jy.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://jr.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dh.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://qx.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kd.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gh.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bg.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yz.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nd.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uc.chemitech.net.cn

[N04] 斐波那契数列
来源：http://hr.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sd.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ap.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ya.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wl.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bi.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ym.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dy.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bb.asd995.cn

[N05] 最大公约数
来源：http://ut.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://nx.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gm.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qp.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aa.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ow.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://lk.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fk.huixiangedu.cn

[N06] 判断回文字符串
来源：http://kw.panjiajie.cn

Py:   s == s[::-1]
来源：http://pe.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://po.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://nd.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://xt.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wz.asd995.cn

Go:   // 双指针从两端比较
来源：http://mq.bjjhwx.cn

Ruby: s == s.reverse
来源：http://hf.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jm.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://rd.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cm.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jz.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xr.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://bs.gzmigu.cn

Java: // 手写 HashMap
来源：http://ny.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://vt.hnjuh.cn

Ruby: // 手写 Hash
来源：http://is.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vc.bookmarksfly.cn

[N08] 生成全排列
来源：http://wa.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://wx.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://xt.shxzukj.cn

JS:   // 手写回溯递归
来源：http://nk.hnjuh.cn

TS:   // 手写回溯递归
来源：http://bd.shtwfgs.cn

Java: // 手写回溯递归
来源：http://kf.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://fo.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ok.huanxung.cn

C#:   // 手写回溯递归
来源：http://ok.bjjhwx.cn

[N09] 栈与队列
来源：http://nz.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://df.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://es.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zq.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ux.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xg.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bu.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://je.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vz.shxzukj.cn

[N10] 链表节点定义
来源：http://uy.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dp.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cm.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://su.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ig.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://rn.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://md.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ed.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hx.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://we.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jk.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://nd.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zq.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://im.nszjky.cn

Java: // 手写递归
来源：http://gk.jianghongdianzi.cn

Go:   // 手写递归
来源：http://wp.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nt.yuntaijiaju.cn

C#:   // 手写递归
来源：http://hb.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dk.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sj.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kf.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sh.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qt.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ml.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cu.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qj.bookmarksfly.cn

================================================================================
来源：http://km.9csxet.cn

O. 并发与异步
来源：http://ne.bjjhwx.cn

================================================================================
来源：http://vj.bjjhwx.cn

[O01] 启动一个线程
来源：http://gm.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bx.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pu.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ff.shxzskj.cn

TS:   // 同 JS
来源：http://ln.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://yg.521024.cn

Go:   go f()
来源：http://fw.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://jl.nicolike.cn

C#:   Task.Run(() => F());
来源：http://gd.chemitech.net.cn

[O02] 使用线程池
来源：http://sl.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cj.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://df.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://de.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://pl.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qo.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eh.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tu.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cn.szsharing.cn

[O03] 加锁保护共享数据
来源：http://ys.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://ba.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://bv.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eq.asd995.cn

TS:   // 同 JS
来源：http://wt.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://rq.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gv.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ji.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://hz.nicolike.cn

[O04] 定义异步函数并等待
来源：http://ec.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://tx.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://re.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://zi.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uk.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aq.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wi.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qb.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://cx.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://zb.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://sj.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ru.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://wi.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://oi.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uo.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wr.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://nr.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gv.yuexingan06.cn

[O06] 使用进程池
来源：http://un.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oz.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://va.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://er.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://eh.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ep.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qv.muxihuayi.cn

Ruby: // fork 块
来源：http://ys.jctech888.com.cn

C#:   Parallel.For
来源：http://io.hahajie.cn

================================================================================
来源：http://ms.szsharing.cn

P. 常用工具函数
来源：http://ki.wgjwhj.cn

================================================================================
来源：http://lo.huanxung.cn

[P01] 生成 UUID
来源：http://bn.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://pu.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qf.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://nl.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://da.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://fa.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://al.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://cy.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://nv.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ou.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fv.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ir.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ls.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oj.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ig.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dh.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sn.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ax.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://wq.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hr.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wa.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bc.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://md.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qc.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gx.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ka.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ik.huanxung.cn

[P04] 求长度
来源：http://pb.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://va.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://os.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gs.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bj.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://gv.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://ey.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://ed.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ut.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://xn.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ug.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mi.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lz.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://od.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://if.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iq.jianghongdianzi.cn

Ruby: a == b
来源：http://eg.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ev.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rv.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fb.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://tt.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ym.chemitech.net.cn

TS:   if (x == null) {}
来源：http://az.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wp.chemitech.net.cn

Go:   if x == nil {}
来源：http://rk.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lr.jctech888.com.cn

C#:   if (x is null) {}
来源：http://oy.szxytkj.cn

[P07] 防抖与节流
来源：http://hv.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eb.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://zj.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ja.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vg.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wl.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dw.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://op.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bc.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://uy.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tm.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dj.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fe.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zy.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fz.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bk.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fs.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ac.muxihuayi.cn

================================================================================
来源：http://kj.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ze.nicolike.cn

================================================================================
来源：http://rh.jctech888.com.cn

[Q01] 创建表
来源：http://fv.wgjwhj.cn

CREATE TABLE users (
来源：http://wk.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mk.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://gz.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://au.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rq.nszjky.cn

);
来源：http://ip.hahajie.cn

[Q02] 创建带外键的表
来源：http://xe.nicolike.cn

CREATE TABLE orders (
来源：http://qd.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gh.newstarts.cn

user_id INT NOT NULL,
来源：http://fm.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://jc.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zx.jianghongdianzi.cn

);
来源：http://dc.huanxung.cn

[Q03] 增加列
来源：http://ow.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lo.panjiajie.cn

[Q04] 修改列类型
来源：http://pv.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ss.9csxet.cn

[Q05] 重命名列
来源：http://gl.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ei.szsharing.cn

[Q06] 删除列
来源：http://xn.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ng.jianghongdianzi.cn

[Q07] 删除表
来源：http://ym.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://st.yuexingan06.cn

[Q08] 创建普通索引
来源：http://th.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rw.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://qz.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zp.nszjky.cn

[Q10] 插入单行
来源：http://bs.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://so.jctech888.com.cn

[Q11] 一次插入多行
来源：http://ln.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://om.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://yx.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eu.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lt.hahajie.cn

[Q13] 忽略重复插入
来源：http://fl.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ba.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://lj.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cl.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yb.yuexingan06.cn

[Q15] 查询全部
来源：http://mb.szxytkj.cn

SELECT * FROM users;
来源：http://mi.bjjhwx.cn

[Q16] 查询指定列
来源：http://tm.huanxung.cn

SELECT id, name FROM users;
来源：http://ii.panjiajie.cn

[Q17] 条件查询
来源：http://pd.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://an.bjjhwx.cn

[Q18] 模糊匹配
来源：http://lc.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lt.jianghongdianzi.cn

[Q19] 范围查询
来源：http://rb.shxzukj.cn


<!-- 参考信息 -->