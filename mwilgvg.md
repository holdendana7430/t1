代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://ya.muxihuayi.cn

[M05] 设置退出码
来源：http://hq.9csxet.cn

Py:   sys.exit(1)
来源：http://ai.521024.cn

PHP:  exit(1);
来源：http://uh.muxihuayi.cn

JS:   process.exit(1)
来源：http://tn.bookmarksfly.cn

TS:   process.exit(1)
来源：http://qx.jianghongdianzi.cn

Java: System.exit(1)
来源：http://bz.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://cf.shtwfgs.cn

Ruby: exit 1
来源：http://hv.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tq.shxzukj.cn

[M06] 向标准错误输出
来源：http://ng.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://or.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rv.shxzskj.cn

JS:   console.error("err")
来源：http://bm.nszjky.cn

TS:   console.error("err")
来源：http://wg.hahajie.cn

Java: System.err.println("err")
来源：http://xz.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jd.jianghongdianzi.cn

Ruby: warn "err"
来源：http://sc.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://xe.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://ge.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://ej.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://td.shxzskj.cn

JS:   require.main === module
来源：http://go.jctech888.com.cn

TS:   require.main === module
来源：http://lc.521024.cn

Java: public static void main(String[] args)
来源：http://fg.colortex.cn

Go:   func main()
来源：http://kw.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ei.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://uo.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://po.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://bk.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://wn.hnjuh.cn

JS:   process.platform;  process.version
来源：http://qi.huanxung.cn

TS:   process.platform;  process.version
来源：http://zj.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wa.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oq.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xh.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rm.gzmigu.cn

================================================================================
来源：http://uj.shtwfgs.cn

N. 数据结构与算法
来源：http://fw.hahajie.cn

================================================================================
来源：http://eh.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://fz.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://os.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sh.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pt.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vp.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cy.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://io.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sf.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eb.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://kl.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ap.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jt.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jh.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qs.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yx.nszjky.cn

Go:   slices.Sort(arr)
来源：http://vp.hnjuh.cn

Ruby: arr.sort
来源：http://gr.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dv.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://hd.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://it.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://or.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ei.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jb.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bb.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ec.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vr.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gb.shxzukj.cn

[N04] 斐波那契数列
来源：http://qc.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fh.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nk.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vr.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sy.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://co.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xt.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rl.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zd.yuexingan06.cn

[N05] 最大公约数
来源：http://zc.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://wd.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ao.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qx.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dk.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mo.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ye.gzmigu.cn

Ruby: a.gcd(b)
来源：http://fg.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sg.colortex.cn

[N06] 判断回文字符串
来源：http://gn.haigaiapp.cn

Py:   s == s[::-1]
来源：http://jn.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://vm.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://dw.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://op.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://io.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://rj.nicolike.cn

Ruby: s == s.reverse
来源：http://pp.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ds.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://ul.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aw.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xg.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://go.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://pp.huixiangedu.cn

Java: // 手写 HashMap
来源：http://mc.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://yc.asd995.cn

Ruby: // 手写 Hash
来源：http://am.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ni.521024.cn

[N08] 生成全排列
来源：http://et.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://aa.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://ge.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://co.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ns.9csxet.cn

Java: // 手写回溯递归
来源：http://ng.asd995.cn

Go:   // 手写回溯递归
来源：http://bk.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://gd.huanxung.cn

C#:   // 手写回溯递归
来源：http://bx.yuntaijiaju.cn

[N09] 栈与队列
来源：http://wj.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wy.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lo.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dq.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zu.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qf.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cx.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://us.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rt.yuexingan06.cn

[N10] 链表节点定义
来源：http://ph.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pn.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zm.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bi.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ht.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://xl.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ht.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://th.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fw.huanxung.cn

[N11] 二叉树中序遍历
来源：http://gj.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pz.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://gz.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aq.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dn.newstarts.cn

Java: // 手写递归
来源：http://ae.yuexingan06.cn

Go:   // 手写递归
来源：http://oa.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wu.jctech888.com.cn

C#:   // 手写递归
来源：http://bv.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jd.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ei.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ug.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oe.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uq.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ku.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xu.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nc.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fo.521024.cn

================================================================================
来源：http://at.muxihuayi.cn

O. 并发与异步
来源：http://ly.nszjky.cn

================================================================================
来源：http://pe.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://sa.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ur.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hf.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bn.bookmarksfly.cn

TS:   // 同 JS
来源：http://gv.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://nl.haigaiapp.cn

Go:   go f()
来源：http://pn.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ij.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://nt.panjiajie.cn

[O02] 使用线程池
来源：http://uo.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kd.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rv.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://sx.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://mo.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mq.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://il.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uc.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jr.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://ba.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://pt.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://gh.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lc.muxihuayi.cn

TS:   // 同 JS
来源：http://rh.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://nf.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ll.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://as.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://pr.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://vs.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://xd.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ig.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://js.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mp.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://em.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lo.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nn.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://ph.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://eq.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://rd.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ky.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://bb.asd995.cn

TS:   await Promise.all(tasks)
来源：http://ei.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ty.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gu.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://eb.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ql.panjiajie.cn

[O06] 使用进程池
来源：http://pr.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://an.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://du.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://tx.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://ys.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fa.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ub.szxytkj.cn

Ruby: // fork 块
来源：http://qh.yuntaijiaju.cn

C#:   Parallel.For
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://kd.huixiangedu.cn

P. 常用工具函数
来源：http://jp.nicolike.cn

================================================================================
来源：http://bi.newstarts.cn

[P01] 生成 UUID
来源：http://fx.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://ll.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cz.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://mk.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://dp.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://bx.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://ma.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://ck.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://hu.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://ys.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uw.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://di.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gr.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mc.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ty.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rs.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ov.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jj.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://xy.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rv.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://og.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wi.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eu.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ny.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cd.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fa.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wn.jianghongdianzi.cn

[P04] 求长度
来源：http://wl.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kp.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jo.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dw.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mi.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://lm.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://wo.szsharing.cn

Ruby: x.length;  x.size
来源：http://jf.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cc.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://ou.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tq.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gy.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tn.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fq.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pl.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qg.9csxet.cn

Ruby: a == b
来源：http://ln.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sb.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bn.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nw.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ox.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ik.huanxung.cn

TS:   if (x == null) {}
来源：http://xm.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uc.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://my.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xb.wgjwhj.cn

C#:   if (x is null) {}
来源：http://ys.yuexingan06.cn

[P07] 防抖与节流
来源：http://yr.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ov.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://rr.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tn.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hq.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sa.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ae.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ls.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xf.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://tq.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zi.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hp.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sf.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yt.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ph.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iw.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cf.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ba.wgjwhj.cn

================================================================================
来源：http://bl.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://on.asd995.cn

================================================================================
来源：http://xm.szxytkj.cn

[Q01] 创建表
来源：http://hq.hahajie.cn

CREATE TABLE users (
来源：http://mk.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wu.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://hu.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://mt.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gp.huixiangedu.cn

);
来源：http://xo.lnxyls.cn

[Q02] 创建带外键的表
来源：http://wj.newstarts.cn

CREATE TABLE orders (
来源：http://wl.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iz.bjjhwx.cn

user_id INT NOT NULL,
来源：http://zy.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://kb.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ki.hahajie.cn

);
来源：http://pm.shtwfgs.cn

[Q03] 增加列
来源：http://oe.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xb.9csxet.cn

[Q04] 修改列类型
来源：http://df.521024.cn


<!-- 参考信息 -->