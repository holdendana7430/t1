代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ol.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://he.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dp.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rw.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ap.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lc.chemitech.net.cn

================================================================================
来源：http://fw.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ok.chemitech.net.cn

================================================================================
来源：http://he.9csxet.cn

[M01] 读取命令行参数
来源：http://ja.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://ms.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://gw.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://fl.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://wb.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://up.huanxung.cn

Go:   os.Args[1:]
来源：http://uu.wgjwhj.cn

Ruby: ARGV
来源：http://bi.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://fa.szxytkj.cn

[M02] 读取环境变量
来源：http://lq.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://gx.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lg.muxihuayi.cn

JS:   process.env.HOME
来源：http://qa.colortex.cn

TS:   process.env.HOME
来源：http://xi.lnxyls.cn

Java: System.getenv("HOME")
来源：http://ic.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://td.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://mw.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wn.yuexingan06.cn

[M03] 执行外部命令
来源：http://ue.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ny.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nt.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mz.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ll.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tv.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bg.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xj.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ks.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://qf.huixiangedu.cn

Py:   os.getcwd()
来源：http://nt.shtwfgs.cn

PHP:  getcwd();
来源：http://sp.panjiajie.cn

JS:   process.cwd()
来源：http://mb.yuntaijiaju.cn

TS:   process.cwd()
来源：http://gs.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://ld.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://kk.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ie.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rf.gzmigu.cn

[M05] 设置退出码
来源：http://rg.huixiangedu.cn

Py:   sys.exit(1)
来源：http://lu.9csxet.cn

PHP:  exit(1);
来源：http://sm.newstarts.cn

JS:   process.exit(1)
来源：http://oz.shtwfgs.cn

TS:   process.exit(1)
来源：http://lu.bookmarksfly.cn

Java: System.exit(1)
来源：http://ff.521024.cn

Go:   os.Exit(1)
来源：http://bv.gzmigu.cn

Ruby: exit 1
来源：http://xm.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pj.shxzukj.cn

[M06] 向标准错误输出
来源：http://ok.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://yo.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qq.szsharing.cn

JS:   console.error("err")
来源：http://uj.nszjky.cn

TS:   console.error("err")
来源：http://ib.chemitech.net.cn

Java: System.err.println("err")
来源：http://rb.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iz.nicolike.cn

Ruby: warn "err"
来源：http://pt.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://mr.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://br.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://jh.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hj.jianghongdianzi.cn

JS:   require.main === module
来源：http://ge.nicolike.cn

TS:   require.main === module
来源：http://un.shxzukj.cn

Java: public static void main(String[] args)
来源：http://zl.huixinmuqiang.cn

Go:   func main()
来源：http://yc.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ui.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://ve.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://kg.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ok.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://lx.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://dv.shxzskj.cn

TS:   process.platform;  process.version
来源：http://fy.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://it.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ex.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vn.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lf.521024.cn

================================================================================
来源：http://yp.hnjuh.cn

N. 数据结构与算法
来源：http://cg.huanxung.cn

================================================================================
来源：http://da.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://yw.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zq.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wp.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zr.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://im.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://im.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qk.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vd.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://cl.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://hc.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cz.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wx.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kd.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ln.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://qq.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ao.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pv.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://iy.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gu.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://zv.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uu.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aa.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ib.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tu.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://we.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vq.wgjwhj.cn

[N04] 斐波那契数列
来源：http://at.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yx.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nn.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tu.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://je.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ds.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xg.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mc.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vz.newstarts.cn

[N05] 最大公约数
来源：http://xf.huanxung.cn

Py:   math.gcd(a, b)
来源：http://mb.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aq.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://um.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yq.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yq.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ep.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://vc.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fw.colortex.cn

[N06] 判断回文字符串
来源：http://hi.shxzukj.cn

Py:   s == s[::-1]
来源：http://ad.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://nu.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://ot.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://co.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gk.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://su.shtwfgs.cn

Ruby: s == s.reverse
来源：http://jr.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iw.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://lf.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kz.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pm.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ms.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://ak.szsharing.cn

Java: // 手写 HashMap
来源：http://gl.nicolike.cn

Go:   // 手写 map[int]int
来源：http://ty.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://rg.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lv.yuexingan06.cn

[N08] 生成全排列
来源：http://qo.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://vc.hahajie.cn

PHP:  // 手写递归交换
来源：http://zs.521024.cn

JS:   // 手写回溯递归
来源：http://jx.nszjky.cn

TS:   // 手写回溯递归
来源：http://vg.asd995.cn

Java: // 手写回溯递归
来源：http://gl.hnjuh.cn

Go:   // 手写回溯递归
来源：http://km.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://qk.lnxyls.cn

C#:   // 手写回溯递归
来源：http://ha.yuntaijiaju.cn

[N09] 栈与队列
来源：http://zg.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ll.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xm.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yh.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xm.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yb.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wn.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xv.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kg.panjiajie.cn

[N10] 链表节点定义
来源：http://kn.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qv.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ks.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ah.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qj.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://ku.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://py.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fi.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://il.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://kt.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pj.panjiajie.cn

PHP:  // 手写递归函数
来源：http://eu.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://go.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wv.yuntaijiaju.cn

Java: // 手写递归
来源：http://td.haigaiapp.cn

Go:   // 手写递归
来源：http://sy.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ir.haigaiapp.cn

C#:   // 手写递归
来源：http://pe.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dv.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gq.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ip.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ui.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ps.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hj.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jx.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lg.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://du.9csxet.cn

================================================================================
来源：http://ix.huixinmuqiang.cn

O. 并发与异步
来源：http://pt.shxzukj.cn

================================================================================
来源：http://du.yuexingan06.cn

[O01] 启动一个线程
来源：http://tc.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ph.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mt.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tk.shxzukj.cn

TS:   // 同 JS
来源：http://ad.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://je.9csxet.cn

Go:   go f()
来源：http://vb.lnxyls.cn

Ruby: Thread.new { f }
来源：http://ez.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://ps.shxzskj.cn

[O02] 使用线程池
来源：http://iw.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qm.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hy.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://or.huanxung.cn

TS:   // worker_threads 线程池
来源：http://qn.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dl.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cy.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yo.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sp.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://bb.9csxet.cn

Py:   with lock: shared += 1
来源：http://as.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://to.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nr.szxytkj.cn

TS:   // 同 JS
来源：http://zv.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://kg.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gc.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gc.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://qu.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://xs.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://ps.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dp.9csxet.cn

JS:   async function f() { await g(); }
来源：http://vh.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gn.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://px.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ml.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yl.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://sk.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://vz.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://ct.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fa.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://bp.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://av.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yz.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sw.nicolike.cn

Ruby: threads.map(&:join)
来源：http://zu.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zw.bookmarksfly.cn

[O06] 使用进程池
来源：http://ki.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rl.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uk.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://cf.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://hf.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zq.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vs.bookmarksfly.cn

Ruby: // fork 块
来源：http://nw.huixiangedu.cn

C#:   Parallel.For
来源：http://zx.hnjuh.cn

================================================================================
来源：http://gq.haigaiapp.cn

P. 常用工具函数
来源：http://wv.panjiajie.cn

================================================================================
来源：http://ic.bookmarksfly.cn

[P01] 生成 UUID
来源：http://uo.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://ej.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wt.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://ee.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://jo.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://uu.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://mj.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://cj.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ad.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://sp.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qq.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gu.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://df.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bc.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rz.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vj.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pz.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oy.huanxung.cn

[P03] 生成短随机字符串
来源：http://zd.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cg.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oy.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bo.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mp.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hj.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sh.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hx.9csxet.cn

[P04] 求长度
来源：http://rk.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://az.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zu.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://su.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://if.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://bh.newstarts.cn

Go:   len(arr);  len(m)
来源：http://vo.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://hq.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ob.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://pv.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ru.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qj.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ym.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://li.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ef.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hw.huixiangedu.cn

Ruby: a == b
来源：http://qn.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cx.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ka.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ew.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://km.gzmigu.cn


<!-- 参考信息 -->