代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ud.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kq.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ml.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cs.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dc.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ci.colortex.cn

================================================================================
来源：http://qu.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://yd.lnxyls.cn

================================================================================
来源：http://gf.newstarts.cn

[M01] 读取命令行参数
来源：http://dt.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://la.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://qm.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://rw.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ai.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://sa.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://hv.newstarts.cn

Ruby: ARGV
来源：http://vq.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://gc.hahajie.cn

[M02] 读取环境变量
来源：http://iw.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://uk.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dn.gzmigu.cn

JS:   process.env.HOME
来源：http://hb.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://ct.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://cs.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://by.9csxet.cn

Ruby: ENV["HOME"]
来源：http://cx.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oz.newstarts.cn

[M03] 执行外部命令
来源：http://kj.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eo.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://we.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ie.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ra.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hk.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://en.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oy.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://mm.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://fe.wgjwhj.cn

Py:   os.getcwd()
来源：http://pn.yuntaijiaju.cn

PHP:  getcwd();
来源：http://fj.newstarts.cn

JS:   process.cwd()
来源：http://bu.gzmigu.cn

TS:   process.cwd()
来源：http://hs.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://dx.asd995.cn

Go:   os.Getwd()
来源：http://vg.huanxung.cn

Ruby: Dir.pwd
来源：http://xr.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qv.yuntaijiaju.cn

[M05] 设置退出码
来源：http://xf.hahajie.cn

Py:   sys.exit(1)
来源：http://cz.bjjhwx.cn

PHP:  exit(1);
来源：http://lp.newstarts.cn

JS:   process.exit(1)
来源：http://mg.jctech888.com.cn

TS:   process.exit(1)
来源：http://jj.yuntaijiaju.cn

Java: System.exit(1)
来源：http://if.wgjwhj.cn

Go:   os.Exit(1)
来源：http://cj.huixiangedu.cn

Ruby: exit 1
来源：http://ud.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ah.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://fe.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://al.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tf.nicolike.cn

JS:   console.error("err")
来源：http://qc.521024.cn

TS:   console.error("err")
来源：http://rt.jctech888.com.cn

Java: System.err.println("err")
来源：http://we.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pg.nicolike.cn

Ruby: warn "err"
来源：http://qx.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://iv.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://sn.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://gr.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vg.panjiajie.cn

JS:   require.main === module
来源：http://mp.bookmarksfly.cn

TS:   require.main === module
来源：http://rv.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://dp.asd995.cn

Go:   func main()
来源：http://iz.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ir.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://mg.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://lh.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://je.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://gc.lnxyls.cn

JS:   process.platform;  process.version
来源：http://tb.shxzukj.cn

TS:   process.platform;  process.version
来源：http://ej.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bq.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sv.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mm.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kp.nszjky.cn

================================================================================
来源：http://lp.asd995.cn

N. 数据结构与算法
来源：http://zj.jianghongdianzi.cn

================================================================================
来源：http://kr.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ec.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ax.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://je.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kj.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vq.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xz.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://bq.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bq.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cf.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://jf.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qk.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wf.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wu.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rd.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://ty.huixiangedu.cn

Ruby: arr.sort
来源：http://qa.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mb.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://dd.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qt.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://qt.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dh.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ee.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://im.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hp.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ul.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tp.jctech888.com.cn

[N04] 斐波那契数列
来源：http://ia.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://al.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lv.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sn.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cm.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rp.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lq.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kt.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cb.haigaiapp.cn

[N05] 最大公约数
来源：http://wx.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://na.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xo.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ug.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uz.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hn.nicolike.cn

Ruby: a.gcd(b)
来源：http://sv.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jl.shxzskj.cn

[N06] 判断回文字符串
来源：http://zz.muxihuayi.cn

Py:   s == s[::-1]
来源：http://fm.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://xd.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://qx.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://jd.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bx.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://lv.9csxet.cn

Ruby: s == s.reverse
来源：http://ci.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hj.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://cb.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tf.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vi.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xg.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://on.muxihuayi.cn

Java: // 手写 HashMap
来源：http://be.9csxet.cn

Go:   // 手写 map[int]int
来源：http://dw.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://yj.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ja.szxytkj.cn

[N08] 生成全排列
来源：http://my.521024.cn

Py:   itertools.permutations(arr)
来源：http://aa.521024.cn

PHP:  // 手写递归交换
来源：http://jy.hnjuh.cn

JS:   // 手写回溯递归
来源：http://wi.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://pl.shxzskj.cn

Java: // 手写回溯递归
来源：http://qx.colortex.cn

Go:   // 手写回溯递归
来源：http://go.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://hy.hahajie.cn

C#:   // 手写回溯递归
来源：http://vl.shxzukj.cn

[N09] 栈与队列
来源：http://lm.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uh.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qh.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fc.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tj.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ir.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pk.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hb.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zn.shxzskj.cn

[N10] 链表节点定义
来源：http://cu.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dx.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zv.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ly.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fh.521024.cn

Java: class Node { int v; Node next; }
来源：http://jx.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nl.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zs.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xr.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://sp.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cg.szsharing.cn

PHP:  // 手写递归函数
来源：http://gl.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ex.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ou.hnjuh.cn

Java: // 手写递归
来源：http://xe.huixinmuqiang.cn

Go:   // 手写递归
来源：http://fv.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zu.huixinmuqiang.cn

C#:   // 手写递归
来源：http://gn.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vy.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ch.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iy.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iu.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bg.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uf.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jt.hahajie.cn

================================================================================
来源：http://re.bookmarksfly.cn

O. 并发与异步
来源：http://kg.chemitech.net.cn

================================================================================
来源：http://jn.colortex.cn

[O01] 启动一个线程
来源：http://wm.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bt.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dz.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ll.shxzskj.cn

TS:   // 同 JS
来源：http://tl.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://za.521024.cn

Go:   go f()
来源：http://pp.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://qx.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://mx.shxzskj.cn

[O02] 使用线程池
来源：http://xr.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ys.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jp.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://bw.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://sq.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ie.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bq.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yz.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ue.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://dg.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://fc.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://pz.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pt.jianghongdianzi.cn

TS:   // 同 JS
来源：http://yl.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://qr.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fg.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://su.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://hx.szsharing.cn

[O04] 定义异步函数并等待
来源：http://mn.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://eo.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fz.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://xw.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ww.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fl.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yk.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sp.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://nj.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://eu.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ui.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cb.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://em.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://xu.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://id.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pm.9csxet.cn

Ruby: threads.map(&:join)
来源：http://wj.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nr.bjjhwx.cn

[O06] 使用进程池
来源：http://ab.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vu.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wv.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://ho.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://cr.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qo.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ca.nszjky.cn

Ruby: // fork 块
来源：http://hr.521024.cn

C#:   Parallel.For
来源：http://gs.huixiangedu.cn

================================================================================
来源：http://jc.muxihuayi.cn

P. 常用工具函数
来源：http://jj.szxytkj.cn

================================================================================
来源：http://af.muxihuayi.cn

[P01] 生成 UUID
来源：http://zz.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://he.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xv.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://id.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://py.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://yc.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://se.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://md.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ut.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://nu.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qd.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tf.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wi.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mj.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://po.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pf.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zc.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zm.newstarts.cn

[P03] 生成短随机字符串
来源：http://lo.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qb.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tu.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://da.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hj.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uc.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sv.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fv.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mh.chemitech.net.cn

[P04] 求长度
来源：http://ks.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sc.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ue.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ok.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qr.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://jv.szsharing.cn

Go:   len(arr);  len(m)
来源：http://cm.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://uw.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vb.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://jx.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vv.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://am.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qz.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qf.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jf.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yf.huanxung.cn

Ruby: a == b
来源：http://wy.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qx.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zd.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://he.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ip.newstarts.cn


<!-- 参考信息 -->