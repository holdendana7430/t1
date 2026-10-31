代发 wailian999

Ruby: exit 1
来源：http://me.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bk.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://al.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://fr.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ih.521024.cn

JS:   console.error("err")
来源：http://wk.haigaiapp.cn

TS:   console.error("err")
来源：http://tu.yuexingan06.cn

Java: System.err.println("err")
来源：http://re.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ls.szxytkj.cn

Ruby: warn "err"
来源：http://cu.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://gg.9csxet.cn

[M07] 判断是否为主入口
来源：http://wj.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://oi.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xs.haigaiapp.cn

JS:   require.main === module
来源：http://gz.chemitech.net.cn

TS:   require.main === module
来源：http://eb.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://pn.yuntaijiaju.cn

Go:   func main()
来源：http://vv.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fz.nicolike.cn

C#:   static void Main(string[] args)
来源：http://cq.asd995.cn

[M08] 获取系统与运行时信息
来源：http://dc.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ar.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://wx.nszjky.cn

JS:   process.platform;  process.version
来源：http://ac.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://oc.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oc.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sb.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ei.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sd.huixinmuqiang.cn

================================================================================
来源：http://xx.colortex.cn

N. 数据结构与算法
来源：http://ek.jianghongdianzi.cn

================================================================================
来源：http://wn.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://wj.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dh.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ar.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ej.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://us.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://uz.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qx.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ag.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://yr.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://wa.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://we.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hs.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vm.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cd.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://wh.nszjky.cn

Ruby: arr.sort
来源：http://wo.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ng.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://ro.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bw.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://om.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ap.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://td.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tk.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eh.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tt.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cz.nicolike.cn

[N04] 斐波那契数列
来源：http://cx.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://my.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gf.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xb.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ds.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ft.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://np.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hb.yuexingan06.cn

[N05] 最大公约数
来源：http://fx.hahajie.cn

Py:   math.gcd(a, b)
来源：http://yu.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pv.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fy.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://am.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://il.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oj.nszjky.cn

Ruby: a.gcd(b)
来源：http://li.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nb.9csxet.cn

[N06] 判断回文字符串
来源：http://vg.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://ia.nszjky.cn

PHP:  $s === strrev($s);
来源：http://fp.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://tj.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://tq.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ye.9csxet.cn

Go:   // 双指针从两端比较
来源：http://no.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ra.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sr.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ol.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bo.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wi.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qe.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://no.asd995.cn

Java: // 手写 HashMap
来源：http://kp.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://io.521024.cn

Ruby: // 手写 Hash
来源：http://nx.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://to.huixinmuqiang.cn

[N08] 生成全排列
来源：http://au.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://xt.newstarts.cn

PHP:  // 手写递归交换
来源：http://ex.colortex.cn

JS:   // 手写回溯递归
来源：http://hs.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://da.colortex.cn

Java: // 手写回溯递归
来源：http://pu.szxytkj.cn

Go:   // 手写回溯递归
来源：http://va.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://jc.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://sz.lnxyls.cn

[N09] 栈与队列
来源：http://lf.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cv.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://og.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pg.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ll.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pc.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ge.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://go.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sg.haigaiapp.cn

[N10] 链表节点定义
来源：http://in.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bs.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sv.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rn.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jt.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://yz.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eu.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uj.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://af.newstarts.cn

[N11] 二叉树中序遍历
来源：http://gm.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nu.shxzukj.cn

PHP:  // 手写递归函数
来源：http://nv.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vs.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ae.colortex.cn

Java: // 手写递归
来源：http://xr.shxzskj.cn

Go:   // 手写递归
来源：http://nc.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ew.colortex.cn

C#:   // 手写递归
来源：http://sz.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ab.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qx.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hs.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pf.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://db.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iy.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://db.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://do.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zq.shxzukj.cn

================================================================================
来源：http://vd.521024.cn

O. 并发与异步
来源：http://mk.huixinmuqiang.cn

================================================================================
来源：http://fj.chemitech.net.cn

[O01] 启动一个线程
来源：http://hs.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qu.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wi.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ej.lnxyls.cn

TS:   // 同 JS
来源：http://tv.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://dh.colortex.cn

Go:   go f()
来源：http://hj.shxzukj.cn

Ruby: Thread.new { f }
来源：http://ik.9csxet.cn

C#:   Task.Run(() => F());
来源：http://eh.szsharing.cn

[O02] 使用线程池
来源：http://je.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zo.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://js.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://wm.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://nr.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://go.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://em.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iu.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://en.9csxet.cn

[O03] 加锁保护共享数据
来源：http://nq.gzmigu.cn

Py:   with lock: shared += 1
来源：http://xm.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://lh.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eo.shtwfgs.cn

TS:   // 同 JS
来源：http://xi.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://gm.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uo.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fv.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://ev.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://gx.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://js.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vs.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://il.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qf.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zs.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xf.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vh.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://jf.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://xw.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://cz.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pl.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://nm.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://dk.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sg.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nv.nicolike.cn

Ruby: threads.map(&:join)
来源：http://mw.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ha.colortex.cn

[O06] 使用进程池
来源：http://nr.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fa.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zx.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://xh.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://lz.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://au.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://km.panjiajie.cn

Ruby: // fork 块
来源：http://ff.huanxung.cn

C#:   Parallel.For
来源：http://zn.lnxyls.cn

================================================================================
来源：http://ih.szsharing.cn

P. 常用工具函数
来源：http://fe.shxzukj.cn

================================================================================
来源：http://zc.huanxung.cn

[P01] 生成 UUID
来源：http://tv.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://lp.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qw.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://vi.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://gl.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://hy.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://km.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://tj.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://nh.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://vh.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vd.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lj.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fz.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://im.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hr.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bk.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jv.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wq.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://cn.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kf.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ql.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ol.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sw.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://db.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lz.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ug.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tz.nicolike.cn

[P04] 求长度
来源：http://ka.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bl.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kz.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ma.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qs.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://qa.huanxung.cn

Go:   len(arr);  len(m)
来源：http://zb.szsharing.cn

Ruby: x.length;  x.size
来源：http://em.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ft.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://oi.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://es.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kr.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mt.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lt.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xq.shtwfgs.cn

Ruby: a == b
来源：http://ly.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://md.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yr.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pa.colortex.cn

PHP:  if (empty($x)) {}
来源：http://bj.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yr.nicolike.cn

TS:   if (x == null) {}
来源：http://ah.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ak.wgjwhj.cn

Go:   if x == nil {}
来源：http://lx.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xx.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://bi.jctech888.com.cn

[P07] 防抖与节流
来源：http://bn.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ka.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://ue.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sm.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tl.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pw.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yh.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://so.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oa.newstarts.cn

[P08] 处理浮点精度问题
来源：http://np.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wf.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qj.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zq.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yh.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yb.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bq.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wu.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lt.wgjwhj.cn

================================================================================
来源：http://jj.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ab.nicolike.cn

================================================================================
来源：http://uv.hnjuh.cn

[Q01] 创建表
来源：http://ke.chemitech.net.cn

CREATE TABLE users (
来源：http://jk.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vs.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://xp.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://co.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lg.shtwfgs.cn

);
来源：http://vu.panjiajie.cn

[Q02] 创建带外键的表
来源：http://hm.szsharing.cn

CREATE TABLE orders (
来源：http://xx.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qf.huixiangedu.cn

user_id INT NOT NULL,
来源：http://yr.szsharing.cn

amount DECIMAL(10, 2),
来源：http://sg.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bf.huixiangedu.cn

);
来源：http://xh.hnjuh.cn

[Q03] 增加列
来源：http://lq.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uv.panjiajie.cn

[Q04] 修改列类型
来源：http://vd.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://va.bjjhwx.cn

[Q05] 重命名列
来源：http://ul.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ue.yuntaijiaju.cn

[Q06] 删除列
来源：http://wy.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nj.yuexingan06.cn

[Q07] 删除表
来源：http://hq.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://la.lnxyls.cn

[Q08] 创建普通索引
来源：http://rh.jctech888.com.cn


<!-- 参考信息 -->