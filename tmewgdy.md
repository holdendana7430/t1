代发 wailian999

Java: public static void main(String[] args)
来源：http://rh.lnxyls.cn

Go:   func main()
来源：http://zt.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rb.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://iu.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://ae.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://qd.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://bj.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://kw.9csxet.cn

TS:   process.platform;  process.version
来源：http://av.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://um.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mb.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wk.shxzskj.cn

================================================================================
来源：http://dl.bookmarksfly.cn

N. 数据结构与算法
来源：http://in.shxzukj.cn

================================================================================
来源：http://da.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://gt.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fs.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yv.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gu.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qe.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sv.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://rk.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fd.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fu.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://xi.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://xd.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://za.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gg.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ex.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oh.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://ez.muxihuayi.cn

Ruby: arr.sort
来源：http://rk.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pa.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://we.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gv.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://ec.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mj.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vg.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iy.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ve.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iz.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ms.haigaiapp.cn

[N04] 斐波那契数列
来源：http://vx.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dp.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ao.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ys.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gk.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hs.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sg.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://un.newstarts.cn

[N05] 最大公约数
来源：http://lr.521024.cn

Py:   math.gcd(a, b)
来源：http://vv.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://am.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jw.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hi.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nm.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bt.colortex.cn

Ruby: a.gcd(b)
来源：http://cz.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pu.hnjuh.cn

[N06] 判断回文字符串
来源：http://xx.nszjky.cn

Py:   s == s[::-1]
来源：http://wv.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://mq.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://cw.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://tv.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pg.szsharing.cn

Go:   // 双指针从两端比较
来源：http://cm.521024.cn

Ruby: s == s.reverse
来源：http://me.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tk.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://xl.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kl.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hp.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ra.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://sk.shtwfgs.cn

Java: // 手写 HashMap
来源：http://ka.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ns.shxzskj.cn

Ruby: // 手写 Hash
来源：http://dd.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sw.newstarts.cn

[N08] 生成全排列
来源：http://va.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://zi.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://qo.hahajie.cn

JS:   // 手写回溯递归
来源：http://by.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ii.yuexingan06.cn

Java: // 手写回溯递归
来源：http://tx.nicolike.cn

Go:   // 手写回溯递归
来源：http://ql.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://fi.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://nr.9csxet.cn

[N09] 栈与队列
来源：http://zq.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rd.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vn.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eu.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aq.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zq.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ov.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zs.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ql.shxzskj.cn

[N10] 链表节点定义
来源：http://hm.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jp.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://se.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ae.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://er.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://ed.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jz.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sr.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ji.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://lg.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kl.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://zt.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xc.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qh.asd995.cn

Java: // 手写递归
来源：http://fv.nszjky.cn

Go:   // 手写递归
来源：http://ut.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fe.szxytkj.cn

C#:   // 手写递归
来源：http://fu.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kj.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cr.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://km.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yr.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tl.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kv.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tx.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ok.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://us.asd995.cn

================================================================================
来源：http://ud.9csxet.cn

O. 并发与异步
来源：http://fa.hnjuh.cn

================================================================================
来源：http://zx.colortex.cn

[O01] 启动一个线程
来源：http://os.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ze.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zb.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nd.nicolike.cn

TS:   // 同 JS
来源：http://ol.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://hk.newstarts.cn

Go:   go f()
来源：http://ko.shxzukj.cn

Ruby: Thread.new { f }
来源：http://tc.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://dh.hahajie.cn

[O02] 使用线程池
来源：http://ya.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://or.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rb.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://aa.colortex.cn

TS:   // worker_threads 线程池
来源：http://ih.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fy.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eg.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jv.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sm.colortex.cn

[O03] 加锁保护共享数据
来源：http://ul.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://zc.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://pt.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jk.chemitech.net.cn

TS:   // 同 JS
来源：http://db.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://pl.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ys.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kn.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://ni.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://ba.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://nq.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nu.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://xx.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jw.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wy.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zl.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yb.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://tn.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://mk.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://xc.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://da.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ce.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://su.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hi.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hk.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://me.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ll.9csxet.cn

[O06] 使用进程池
来源：http://wg.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pn.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kw.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://ph.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ph.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dj.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ls.chemitech.net.cn

Ruby: // fork 块
来源：http://jr.szxytkj.cn

C#:   Parallel.For
来源：http://uz.yuexingan06.cn

================================================================================
来源：http://kh.colortex.cn

P. 常用工具函数
来源：http://zw.521024.cn

================================================================================
来源：http://qb.huanxung.cn

[P01] 生成 UUID
来源：http://zo.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://lq.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vw.521024.cn

JS:   crypto.randomUUID()
来源：http://md.asd995.cn

TS:   crypto.randomUUID()
来源：http://lz.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://al.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://ml.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://sa.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://sc.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://gz.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kz.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ah.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bx.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ce.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mg.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mc.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jl.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uv.hnjuh.cn

[P03] 生成短随机字符串
来源：http://gp.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lm.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nq.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mq.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sm.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yi.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yh.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rs.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gx.nicolike.cn

[P04] 求长度
来源：http://bq.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ti.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kg.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://se.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lv.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://wd.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://jm.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://vy.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ey.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://nw.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ld.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rd.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sg.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jq.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jg.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xz.nszjky.cn

Ruby: a == b
来源：http://yg.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qn.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qk.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hv.colortex.cn

PHP:  if (empty($x)) {}
来源：http://oq.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://np.wgjwhj.cn

TS:   if (x == null) {}
来源：http://vg.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hp.haigaiapp.cn

Go:   if x == nil {}
来源：http://xf.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sz.szxytkj.cn

C#:   if (x is null) {}
来源：http://wa.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://nt.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ii.521024.cn

PHP:  // 手写时间戳比较
来源：http://kq.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://it.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eb.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fq.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://np.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mb.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qy.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://hg.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ht.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kz.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://et.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://py.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bt.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://de.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tw.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tm.bookmarksfly.cn

================================================================================
来源：http://ct.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wm.yuntaijiaju.cn

================================================================================
来源：http://yn.szxytkj.cn

[Q01] 创建表
来源：http://sy.wgjwhj.cn

CREATE TABLE users (
来源：http://rp.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mp.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://px.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://df.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ld.521024.cn

);
来源：http://ul.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://vc.muxihuayi.cn

CREATE TABLE orders (
来源：http://dx.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cg.yuexingan06.cn

user_id INT NOT NULL,
来源：http://ok.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://vs.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xp.szsharing.cn

);
来源：http://fs.szxytkj.cn

[Q03] 增加列
来源：http://to.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://io.hnjuh.cn

[Q04] 修改列类型
来源：http://qu.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fe.521024.cn

[Q05] 重命名列
来源：http://jm.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://si.chemitech.net.cn

[Q06] 删除列
来源：http://gp.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tn.wgjwhj.cn

[Q07] 删除表
来源：http://xe.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://sd.newstarts.cn

[Q08] 创建普通索引
来源：http://gc.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://ot.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qg.lnxyls.cn

[Q10] 插入单行
来源：http://zq.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ce.asd995.cn

[Q11] 一次插入多行
来源：http://uh.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://es.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://ke.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wm.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mj.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://hc.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rh.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://hr.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ye.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nq.huixinmuqiang.cn

[Q15] 查询全部
来源：http://xm.jctech888.com.cn


<!-- 参考信息 -->