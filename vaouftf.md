代发 wailian999

Java: public static void main(String[] args)
来源：http://xl.shtwfgs.cn

Go:   func main()
来源：http://lg.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vw.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://lo.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://hp.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://zd.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://dd.lnxyls.cn

JS:   process.platform;  process.version
来源：http://ui.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://bh.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hf.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gd.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rj.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vs.chemitech.net.cn

================================================================================
来源：http://ad.521024.cn

N. 数据结构与算法
来源：http://du.shxzukj.cn

================================================================================
来源：http://yt.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://vk.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ab.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xi.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ru.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wy.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yr.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://tl.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ac.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zv.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ud.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ip.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bv.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ja.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wn.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tw.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://nm.shxzukj.cn

Ruby: arr.sort
来源：http://ja.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lz.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://dy.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vu.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://by.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://en.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ri.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qv.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hv.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ze.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vx.hnjuh.cn

[N04] 斐波那契数列
来源：http://ke.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bu.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jw.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rd.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uz.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://js.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bs.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oo.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hq.jctech888.com.cn

[N05] 最大公约数
来源：http://vy.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://om.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pr.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://td.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://id.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vg.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qc.shxzukj.cn

Ruby: a.gcd(b)
来源：http://vc.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lj.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://ab.huixiangedu.cn

Py:   s == s[::-1]
来源：http://mw.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://fi.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://jw.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://yu.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gx.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ou.lnxyls.cn

Ruby: s == s.reverse
来源：http://cd.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zy.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://bc.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pq.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ft.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gd.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://qs.colortex.cn

Java: // 手写 HashMap
来源：http://ks.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://bg.szxytkj.cn

Ruby: // 手写 Hash
来源：http://pl.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sw.wgjwhj.cn

[N08] 生成全排列
来源：http://fm.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://gf.nszjky.cn

PHP:  // 手写递归交换
来源：http://gy.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://uq.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://lb.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://lo.nszjky.cn

Go:   // 手写回溯递归
来源：http://he.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zu.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://sj.huanxung.cn

[N09] 栈与队列
来源：http://ce.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ak.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oh.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tv.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jk.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qs.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ja.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qd.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ly.hahajie.cn

[N10] 链表节点定义
来源：http://gd.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jv.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qg.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mv.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dc.521024.cn

Java: class Node { int v; Node next; }
来源：http://fk.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nt.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gj.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zu.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://ai.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hv.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://oi.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tp.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.jctech888.com.cn

Java: // 手写递归
来源：http://wq.huanxung.cn

Go:   // 手写递归
来源：http://ro.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yz.hahajie.cn

C#:   // 手写递归
来源：http://cr.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gi.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oa.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bt.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://po.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pk.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://am.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ky.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cy.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://am.asd995.cn

================================================================================
来源：http://ed.chemitech.net.cn

O. 并发与异步
来源：http://dl.newstarts.cn

================================================================================
来源：http://bp.asd995.cn

[O01] 启动一个线程
来源：http://za.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ry.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fn.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://em.hahajie.cn

TS:   // 同 JS
来源：http://dg.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://kc.colortex.cn

Go:   go f()
来源：http://hf.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://xb.huanxung.cn

C#:   Task.Run(() => F());
来源：http://bc.shxzskj.cn

[O02] 使用线程池
来源：http://np.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tj.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uc.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://id.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://mt.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ay.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mx.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fa.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ju.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://aj.hahajie.cn

Py:   with lock: shared += 1
来源：http://ft.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://ke.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fr.9csxet.cn

TS:   // 同 JS
来源：http://hd.521024.cn

Java: synchronized (this) { shared++; }
来源：http://fi.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bk.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kv.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://hs.nszjky.cn

[O04] 定义异步函数并等待
来源：http://yn.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://dw.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dv.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://qy.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kr.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pb.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zy.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wr.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://dv.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://jp.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://ip.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://al.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://uh.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://bo.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eq.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qd.newstarts.cn

Ruby: threads.map(&:join)
来源：http://uf.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oo.huixiangedu.cn

[O06] 使用进程池
来源：http://cl.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ex.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qp.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://ab.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://xb.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ce.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wh.nszjky.cn

Ruby: // fork 块
来源：http://ox.shxzskj.cn

C#:   Parallel.For
来源：http://qe.wgjwhj.cn

================================================================================
来源：http://yu.yuntaijiaju.cn

P. 常用工具函数
来源：http://cc.gzmigu.cn

================================================================================
来源：http://uo.szsharing.cn

[P01] 生成 UUID
来源：http://oh.asd995.cn

Py:   str(uuid.uuid4())
来源：http://hm.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hq.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://gy.9csxet.cn

TS:   crypto.randomUUID()
来源：http://vg.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://oe.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://tg.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://wm.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://wh.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://kk.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qd.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jr.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dg.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ud.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://el.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ov.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bg.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://si.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://gs.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cy.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://we.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oz.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nw.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yy.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ql.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vq.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uy.jianghongdianzi.cn

[P04] 求长度
来源：http://dr.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vt.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jp.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ph.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gk.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://vf.szsharing.cn

Go:   len(arr);  len(m)
来源：http://zy.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://xr.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oh.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://qs.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zd.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wz.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://co.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ye.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ok.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bz.wgjwhj.cn

Ruby: a == b
来源：http://td.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ci.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://za.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lz.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://qo.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fl.szsharing.cn

TS:   if (x == null) {}
来源：http://ec.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zf.gzmigu.cn

Go:   if x == nil {}
来源：http://ie.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://he.newstarts.cn

C#:   if (x is null) {}
来源：http://dl.shxzukj.cn

[P07] 防抖与节流
来源：http://ov.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aw.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ta.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vq.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ia.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rq.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rj.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ie.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://ki.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sr.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rp.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tm.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://td.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cv.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ok.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uw.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nx.haigaiapp.cn

================================================================================
来源：http://lp.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ws.huanxung.cn

================================================================================
来源：http://nu.shxzukj.cn

[Q01] 创建表
来源：http://qp.shxzukj.cn

CREATE TABLE users (
来源：http://nw.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://of.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://hk.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://ns.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rw.shtwfgs.cn

);
来源：http://em.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://dq.muxihuayi.cn

CREATE TABLE orders (
来源：http://hw.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sq.shtwfgs.cn

user_id INT NOT NULL,
来源：http://ob.9csxet.cn

amount DECIMAL(10, 2),
来源：http://sy.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://so.jianghongdianzi.cn

);
来源：http://tr.nszjky.cn

[Q03] 增加列
来源：http://wp.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wx.lnxyls.cn

[Q04] 修改列类型
来源：http://do.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nr.9csxet.cn

[Q05] 重命名列
来源：http://xe.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nz.muxihuayi.cn

[Q06] 删除列
来源：http://ez.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ez.wgjwhj.cn

[Q07] 删除表
来源：http://vg.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://xy.bjjhwx.cn

[Q08] 创建普通索引
来源：http://ny.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bc.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ui.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xm.colortex.cn

[Q10] 插入单行
来源：http://cf.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fu.521024.cn

[Q11] 一次插入多行
来源：http://xm.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ag.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://ua.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xw.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uv.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://sz.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fw.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://sj.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ns.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nm.muxihuayi.cn

[Q15] 查询全部
来源：http://fz.521024.cn


<!-- 参考信息 -->