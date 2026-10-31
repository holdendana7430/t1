代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ig.muxihuayi.cn

Ruby: warn "err"
来源：http://br.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://jg.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://zm.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://hz.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lo.bjjhwx.cn

JS:   require.main === module
来源：http://lg.chemitech.net.cn

TS:   require.main === module
来源：http://lc.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://su.huixinmuqiang.cn

Go:   func main()
来源：http://ky.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rh.newstarts.cn

C#:   static void Main(string[] args)
来源：http://cj.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://cv.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://em.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://nh.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://ej.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://yu.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vt.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gi.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yo.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ck.shtwfgs.cn

================================================================================
来源：http://fh.yuexingan06.cn

N. 数据结构与算法
来源：http://yh.muxihuayi.cn

================================================================================
来源：http://vb.521024.cn

[N01] 二分查找（有序数组）
来源：http://cm.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dj.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gg.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pv.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jf.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yb.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://aw.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yf.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pn.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://kj.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://gp.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ef.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gk.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sw.9csxet.cn

Go:   slices.Sort(arr)
来源：http://fq.gzmigu.cn

Ruby: arr.sort
来源：http://tm.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cc.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://da.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mz.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://dn.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zl.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ig.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ki.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gt.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ox.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zd.hnjuh.cn

[N04] 斐波那契数列
来源：http://kf.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gl.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eu.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lz.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ng.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://el.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zc.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mh.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sd.haigaiapp.cn

[N05] 最大公约数
来源：http://qb.szsharing.cn

Py:   math.gcd(a, b)
来源：http://dj.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://um.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ch.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jf.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zz.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eu.szxytkj.cn

Ruby: a.gcd(b)
来源：http://xc.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bm.asd995.cn

[N06] 判断回文字符串
来源：http://zw.nicolike.cn

Py:   s == s[::-1]
来源：http://lx.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://kj.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://hb.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://td.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://up.nszjky.cn

Go:   // 双指针从两端比较
来源：http://gi.shxzskj.cn

Ruby: s == s.reverse
来源：http://cl.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://um.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://kt.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kx.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eo.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xs.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://nk.muxihuayi.cn

Java: // 手写 HashMap
来源：http://rl.newstarts.cn

Go:   // 手写 map[int]int
来源：http://tl.asd995.cn

Ruby: // 手写 Hash
来源：http://xr.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iq.asd995.cn

[N08] 生成全排列
来源：http://ly.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://eu.newstarts.cn

PHP:  // 手写递归交换
来源：http://fk.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://uz.colortex.cn

TS:   // 手写回溯递归
来源：http://yo.hahajie.cn

Java: // 手写回溯递归
来源：http://tn.nszjky.cn

Go:   // 手写回溯递归
来源：http://is.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://tb.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://mp.yuexingan06.cn

[N09] 栈与队列
来源：http://ub.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jz.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://to.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nb.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pt.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cf.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://on.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ee.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kq.bookmarksfly.cn

[N10] 链表节点定义
来源：http://zw.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jx.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zg.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fm.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xb.colortex.cn

Java: class Node { int v; Node next; }
来源：http://ki.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nn.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kh.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pi.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://un.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oy.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://bp.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tl.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sw.shxzukj.cn

Java: // 手写递归
来源：http://fz.nicolike.cn

Go:   // 手写递归
来源：http://dj.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rf.hnjuh.cn

C#:   // 手写递归
来源：http://tf.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lu.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tj.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://av.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yn.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sf.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://is.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yc.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mg.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ks.shxzukj.cn

================================================================================
来源：http://jr.nicolike.cn

O. 并发与异步
来源：http://rf.chemitech.net.cn

================================================================================
来源：http://vx.muxihuayi.cn

[O01] 启动一个线程
来源：http://rd.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wx.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yn.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mn.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ht.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://zk.chemitech.net.cn

Go:   go f()
来源：http://ck.newstarts.cn

Ruby: Thread.new { f }
来源：http://kn.szsharing.cn

C#:   Task.Run(() => F());
来源：http://og.9csxet.cn

[O02] 使用线程池
来源：http://ab.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lh.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pv.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://ly.hahajie.cn

TS:   // worker_threads 线程池
来源：http://bo.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ka.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xs.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tj.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gw.huanxung.cn

[O03] 加锁保护共享数据
来源：http://vl.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://dm.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://hn.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jy.asd995.cn

TS:   // 同 JS
来源：http://cm.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://gl.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ff.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zw.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ey.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://bc.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://vi.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://au.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://qy.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kz.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qz.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gv.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gd.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://wy.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://no.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://fq.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nz.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://jy.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://vj.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ax.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rx.colortex.cn

Ruby: threads.map(&:join)
来源：http://ye.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nq.shxzukj.cn

[O06] 使用进程池
来源：http://ov.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bl.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ej.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://ba.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://ou.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://go.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ni.newstarts.cn

Ruby: // fork 块
来源：http://sx.colortex.cn

C#:   Parallel.For
来源：http://dy.shxzukj.cn

================================================================================
来源：http://jj.shtwfgs.cn

P. 常用工具函数
来源：http://qy.shxzskj.cn

================================================================================
来源：http://oe.nicolike.cn

[P01] 生成 UUID
来源：http://sl.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://em.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jx.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://he.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://uv.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://pn.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://km.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://kx.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://bn.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://pd.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hc.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uk.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jf.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://of.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uy.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cn.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ow.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nj.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://tx.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://od.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gi.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tq.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fc.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hl.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://or.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jx.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wi.jianghongdianzi.cn

[P04] 求长度
来源：http://ai.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ty.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ls.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aw.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vb.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://ak.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://gp.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://uv.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qa.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://vu.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rq.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iy.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vo.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bs.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wa.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nu.gzmigu.cn

Ruby: a == b
来源：http://vp.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qg.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ai.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nb.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://ft.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uj.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://yb.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rl.shtwfgs.cn

Go:   if x == nil {}
来源：http://th.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://br.shtwfgs.cn

C#:   if (x is null) {}
来源：http://rg.hahajie.cn

[P07] 防抖与节流
来源：http://ok.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://it.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://gd.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ah.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ag.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sq.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dn.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gk.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ed.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://qq.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uc.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jh.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ms.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yc.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://de.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tm.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tk.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.lnxyls.cn

================================================================================
来源：http://ij.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cx.yuntaijiaju.cn

================================================================================
来源：http://ky.colortex.cn

[Q01] 创建表
来源：http://vu.bookmarksfly.cn

CREATE TABLE users (
来源：http://sg.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ci.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://gi.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://ro.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xy.yuexingan06.cn

);
来源：http://to.huanxung.cn

[Q02] 创建带外键的表
来源：http://ph.muxihuayi.cn

CREATE TABLE orders (
来源：http://iz.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fz.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://py.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://re.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sl.colortex.cn

);
来源：http://bu.asd995.cn

[Q03] 增加列
来源：http://jp.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cl.szxytkj.cn

[Q04] 修改列类型
来源：http://ra.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xa.521024.cn

[Q05] 重命名列
来源：http://ji.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jm.huixiangedu.cn

[Q06] 删除列
来源：http://hw.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fc.hahajie.cn

[Q07] 删除表
来源：http://tc.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://pd.huanxung.cn

[Q08] 创建普通索引
来源：http://bb.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oi.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://mq.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sd.nicolike.cn

[Q10] 插入单行
来源：http://qe.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zw.szsharing.cn

[Q11] 一次插入多行
来源：http://fx.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cp.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://nk.szsharing.cn


<!-- 参考信息 -->