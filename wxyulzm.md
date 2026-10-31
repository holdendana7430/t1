代发 wailian999

Java: public static void main(String[] args)
来源：http://jq.jianghongdianzi.cn

Go:   func main()
来源：http://rt.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wv.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://tw.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://ut.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://rk.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://rj.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ky.asd995.cn

TS:   process.platform;  process.version
来源：http://dl.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://us.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cu.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ey.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tc.muxihuayi.cn

================================================================================
来源：http://wp.wgjwhj.cn

N. 数据结构与算法
来源：http://wy.szxytkj.cn

================================================================================
来源：http://ig.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://tv.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://td.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fq.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wu.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dc.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jx.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://hp.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xh.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://no.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://dn.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jm.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xq.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dp.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qn.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rj.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://dz.nicolike.cn

Ruby: arr.sort
来源：http://xj.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gd.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://pz.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hl.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://uv.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nr.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ys.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qn.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nb.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pe.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tb.szxytkj.cn

[N04] 斐波那契数列
来源：http://ww.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lr.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zv.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qj.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eq.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ul.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xz.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nh.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hn.9csxet.cn

[N05] 最大公约数
来源：http://ma.asd995.cn

Py:   math.gcd(a, b)
来源：http://se.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ja.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rr.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oa.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xk.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ja.nicolike.cn

Ruby: a.gcd(b)
来源：http://cj.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://io.chemitech.net.cn

[N06] 判断回文字符串
来源：http://jy.shtwfgs.cn

Py:   s == s[::-1]
来源：http://fy.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://tl.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://ze.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://jb.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mc.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://he.szxytkj.cn

Ruby: s == s.reverse
来源：http://pr.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ga.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://je.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uw.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ah.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dg.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://xh.panjiajie.cn

Java: // 手写 HashMap
来源：http://nt.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://st.newstarts.cn

Ruby: // 手写 Hash
来源：http://yn.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uv.jctech888.com.cn

[N08] 生成全排列
来源：http://al.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://lo.gzmigu.cn

PHP:  // 手写递归交换
来源：http://ra.hnjuh.cn

JS:   // 手写回溯递归
来源：http://tk.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://xe.nicolike.cn

Java: // 手写回溯递归
来源：http://de.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://xq.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://ui.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://pi.jctech888.com.cn

[N09] 栈与队列
来源：http://ax.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vn.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sc.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dc.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ue.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ew.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ho.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fq.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nn.huixiangedu.cn

[N10] 链表节点定义
来源：http://hx.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ue.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lc.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sz.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://at.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://hm.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lh.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pj.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rf.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://jy.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://om.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://so.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fz.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://by.lnxyls.cn

Java: // 手写递归
来源：http://it.wgjwhj.cn

Go:   // 手写递归
来源：http://xj.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nx.hnjuh.cn

C#:   // 手写递归
来源：http://rj.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wd.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mx.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wn.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sd.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tg.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mo.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zj.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pb.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pt.shtwfgs.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

O. 并发与异步
来源：http://rm.shxzukj.cn

================================================================================
来源：http://ir.gzmigu.cn

[O01] 启动一个线程
来源：http://gl.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mb.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ky.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ip.hahajie.cn

TS:   // 同 JS
来源：http://kk.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://mz.haigaiapp.cn

Go:   go f()
来源：http://fo.panjiajie.cn

Ruby: Thread.new { f }
来源：http://hy.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://nh.huixiangedu.cn

[O02] 使用线程池
来源：http://ze.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mv.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gb.nszjky.cn

JS:   // worker_threads 线程池
来源：http://it.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://ky.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cp.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dn.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lm.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://en.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://mu.asd995.cn

Py:   with lock: shared += 1
来源：http://ls.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://cs.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kz.szsharing.cn

TS:   // 同 JS
来源：http://bq.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://ou.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://st.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qw.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://av.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://ky.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://wi.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yl.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://ce.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mk.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kl.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rc.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lu.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://ix.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://hk.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://ac.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ae.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://vr.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://jp.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://im.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wg.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://mj.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dw.muxihuayi.cn

[O06] 使用进程池
来源：http://jb.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yz.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vv.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://zw.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://yf.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vc.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xo.szsharing.cn

Ruby: // fork 块
来源：http://wr.shxzukj.cn

C#:   Parallel.For
来源：http://ky.yuexingan06.cn

================================================================================
来源：http://yh.huanxung.cn

P. 常用工具函数
来源：http://pc.wgjwhj.cn

================================================================================
来源：http://cd.panjiajie.cn

[P01] 生成 UUID
来源：http://ju.colortex.cn

Py:   str(uuid.uuid4())
来源：http://nc.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ig.huanxung.cn

JS:   crypto.randomUUID()
来源：http://rf.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://ss.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://zl.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://jv.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://kr.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://fn.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://oq.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ut.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gc.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fl.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bo.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ni.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://le.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ps.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bg.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ag.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kc.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ko.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tm.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kx.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gt.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://un.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ek.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sq.shxzskj.cn

[P04] 求长度
来源：http://oq.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://um.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mb.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://se.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bi.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://hw.asd995.cn

Go:   len(arr);  len(m)
来源：http://dc.newstarts.cn

Ruby: x.length;  x.size
来源：http://zo.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uc.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://yj.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pe.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fm.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ai.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vg.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wy.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vw.chemitech.net.cn

Ruby: a == b
来源：http://mt.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dw.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fg.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gc.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://yl.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tg.hnjuh.cn

TS:   if (x == null) {}
来源：http://wz.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://so.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://xw.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vb.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://vl.muxihuayi.cn

[P07] 防抖与节流
来源：http://tn.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yt.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://jo.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oo.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nw.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jy.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bp.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nr.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ff.szsharing.cn

[P08] 处理浮点精度问题
来源：http://lw.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fc.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hs.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://to.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mf.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jw.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ad.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gh.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xi.chemitech.net.cn

================================================================================
来源：http://er.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qj.haigaiapp.cn

================================================================================
来源：http://tp.haigaiapp.cn

[Q01] 创建表
来源：http://bi.szxytkj.cn

CREATE TABLE users (
来源：http://xm.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vx.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://zz.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://hb.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rk.9csxet.cn

);
来源：http://qx.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://wh.panjiajie.cn

CREATE TABLE orders (
来源：http://qc.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ew.9csxet.cn

user_id INT NOT NULL,
来源：http://cg.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://kr.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ap.lnxyls.cn

);
来源：http://pn.9csxet.cn

[Q03] 增加列
来源：http://li.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yt.muxihuayi.cn

[Q04] 修改列类型
来源：http://ct.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pg.panjiajie.cn

[Q05] 重命名列
来源：http://ow.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ra.wgjwhj.cn

[Q06] 删除列
来源：http://jz.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://um.colortex.cn

[Q07] 删除表
来源：http://bo.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://mw.shxzukj.cn

[Q08] 创建普通索引
来源：http://ty.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://es.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://ao.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xc.haigaiapp.cn

[Q10] 插入单行
来源：http://mr.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fv.huanxung.cn

[Q11] 一次插入多行
来源：http://yl.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ei.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://ud.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rn.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gm.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://dc.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ih.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://ot.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yo.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vj.shtwfgs.cn

[Q15] 查询全部
来源：http://im.jianghongdianzi.cn


<!-- 参考信息 -->