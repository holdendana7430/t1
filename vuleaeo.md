代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ap.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ex.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jc.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xx.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://du.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pw.colortex.cn

================================================================================
来源：http://ch.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://py.colortex.cn

================================================================================
来源：http://wi.huixiangedu.cn

[M01] 读取命令行参数
来源：http://oj.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://mu.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://wk.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://zb.521024.cn

TS:   process.argv.slice(2)
来源：http://uu.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://td.nicolike.cn

Go:   os.Args[1:]
来源：http://lc.bookmarksfly.cn

Ruby: ARGV
来源：http://hp.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://ay.szxytkj.cn

[M02] 读取环境变量
来源：http://bu.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://zk.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ax.shtwfgs.cn

JS:   process.env.HOME
来源：http://fm.yuexingan06.cn

TS:   process.env.HOME
来源：http://hl.9csxet.cn

Java: System.getenv("HOME")
来源：http://ms.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sr.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://iz.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ad.bjjhwx.cn

[M03] 执行外部命令
来源：http://ny.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ml.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qa.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://az.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uo.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zs.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wh.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ev.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://rp.panjiajie.cn

[M04] 获取当前工作目录
来源：http://am.haigaiapp.cn

Py:   os.getcwd()
来源：http://ny.shxzukj.cn

PHP:  getcwd();
来源：http://id.521024.cn

JS:   process.cwd()
来源：http://wr.shxzukj.cn

TS:   process.cwd()
来源：http://dp.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://yu.newstarts.cn

Go:   os.Getwd()
来源：http://jf.asd995.cn

Ruby: Dir.pwd
来源：http://sv.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kw.hahajie.cn

[M05] 设置退出码
来源：http://tb.shxzskj.cn

Py:   sys.exit(1)
来源：http://jk.colortex.cn

PHP:  exit(1);
来源：http://wi.szsharing.cn

JS:   process.exit(1)
来源：http://ze.nicolike.cn

TS:   process.exit(1)
来源：http://lp.asd995.cn

Java: System.exit(1)
来源：http://kd.huanxung.cn

Go:   os.Exit(1)
来源：http://vc.bookmarksfly.cn

Ruby: exit 1
来源：http://kq.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ve.shtwfgs.cn

[M06] 向标准错误输出
来源：http://cx.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://yg.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mi.9csxet.cn

JS:   console.error("err")
来源：http://ub.shxzskj.cn

TS:   console.error("err")
来源：http://wc.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ie.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tb.huixiangedu.cn

Ruby: warn "err"
来源：http://qi.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://ou.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://ks.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://rs.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lm.asd995.cn

JS:   require.main === module
来源：http://dl.shxzukj.cn

TS:   require.main === module
来源：http://ow.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://yt.jctech888.com.cn

Go:   func main()
来源：http://sg.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oa.newstarts.cn

C#:   static void Main(string[] args)
来源：http://dg.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://bk.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://ow.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ap.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://mg.nszjky.cn

TS:   process.platform;  process.version
来源：http://bc.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zs.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yo.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://at.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gj.jctech888.com.cn

================================================================================
来源：http://yh.yuntaijiaju.cn

N. 数据结构与算法
来源：http://nw.muxihuayi.cn

================================================================================
来源：http://lx.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://xc.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fi.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bq.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ay.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lu.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ef.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://vo.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cx.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ht.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://sb.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://sk.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xp.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ts.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kv.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hd.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://fd.newstarts.cn

Ruby: arr.sort
来源：http://ye.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gg.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://ny.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ya.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://sg.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uw.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hb.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kd.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vy.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xs.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://or.yuexingan06.cn

[N04] 斐波那契数列
来源：http://kf.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://za.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iz.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yf.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kx.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oj.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ly.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bu.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ut.9csxet.cn

[N05] 最大公约数
来源：http://co.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://fn.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vu.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ds.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mc.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wp.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iq.szxytkj.cn

Ruby: a.gcd(b)
来源：http://sh.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qg.asd995.cn

[N06] 判断回文字符串
来源：http://pg.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://mm.nicolike.cn

PHP:  $s === strrev($s);
来源：http://kx.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://po.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://ec.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wc.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://hy.muxihuayi.cn

Ruby: s == s.reverse
来源：http://wv.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gv.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://eg.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sb.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://os.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pg.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://rn.colortex.cn

Java: // 手写 HashMap
来源：http://ju.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ze.huanxung.cn

Ruby: // 手写 Hash
来源：http://my.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zr.gzmigu.cn

[N08] 生成全排列
来源：http://xi.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://zq.colortex.cn

PHP:  // 手写递归交换
来源：http://sl.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://by.newstarts.cn

TS:   // 手写回溯递归
来源：http://qm.jctech888.com.cn

Java: // 手写回溯递归
来源：http://pd.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://xn.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://so.newstarts.cn

C#:   // 手写回溯递归
来源：http://ch.521024.cn

[N09] 栈与队列
来源：http://ab.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nb.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ad.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bx.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pl.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ab.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ye.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zw.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://om.jctech888.com.cn

[N10] 链表节点定义
来源：http://fq.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qi.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jb.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zz.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vm.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://md.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rt.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jr.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vi.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://vu.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uh.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://zq.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sk.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sj.jianghongdianzi.cn

Java: // 手写递归
来源：http://pl.yuexingan06.cn

Go:   // 手写递归
来源：http://rc.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rw.huixiangedu.cn

C#:   // 手写递归
来源：http://an.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ug.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://op.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yj.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hk.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://em.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tg.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aj.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nf.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qg.haigaiapp.cn

================================================================================
来源：http://oj.lnxyls.cn

O. 并发与异步
来源：http://ew.shxzukj.cn

================================================================================
来源：http://pr.521024.cn

[O01] 启动一个线程
来源：http://zh.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gb.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yn.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qc.huanxung.cn

TS:   // 同 JS
来源：http://xv.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://sn.jctech888.com.cn

Go:   go f()
来源：http://ae.gzmigu.cn

Ruby: Thread.new { f }
来源：http://aq.colortex.cn

C#:   Task.Run(() => F());
来源：http://jd.shtwfgs.cn

[O02] 使用线程池
来源：http://gd.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uf.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hu.hahajie.cn

JS:   // worker_threads 线程池
来源：http://uf.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://xm.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rl.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uz.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nw.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hp.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://tm.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://lv.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://er.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wy.hahajie.cn

TS:   // 同 JS
来源：http://so.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://ts.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ig.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vi.521024.cn

C#:   lock (gate) { shared++; }
来源：http://qa.hahajie.cn

[O04] 定义异步函数并等待
来源：http://py.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://xl.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cm.huanxung.cn

JS:   async function f() { await g(); }
来源：http://cp.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://na.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sl.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qs.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://db.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://wh.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://tf.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://rn.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kf.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://as.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ip.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ws.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dk.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://ss.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gy.shxzukj.cn

[O06] 使用进程池
来源：http://yq.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gf.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qz.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://vc.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://me.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ub.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fv.yuntaijiaju.cn

Ruby: // fork 块
来源：http://po.shxzskj.cn

C#:   Parallel.For
来源：http://wu.bookmarksfly.cn

================================================================================
来源：http://hs.hahajie.cn

P. 常用工具函数
来源：http://ln.nszjky.cn

================================================================================
来源：http://xr.asd995.cn

[P01] 生成 UUID
来源：http://xi.asd995.cn

Py:   str(uuid.uuid4())
来源：http://lz.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cb.colortex.cn

JS:   crypto.randomUUID()
来源：http://id.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://ee.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://sw.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://cu.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://xj.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://wn.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://qt.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://em.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ip.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://td.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mf.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tv.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hq.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yl.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://us.nszjky.cn

[P03] 生成短随机字符串
来源：http://za.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gl.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zg.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sm.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fd.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kg.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eq.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nu.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://to.hnjuh.cn

[P04] 求长度
来源：http://gb.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yv.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rh.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bs.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://tu.colortex.cn

Go:   len(arr);  len(m)
来源：http://no.hahajie.cn

Ruby: x.length;  x.size
来源：http://fm.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bt.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://nz.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oy.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://he.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sr.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://or.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pi.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vv.bjjhwx.cn

Ruby: a == b
来源：http://jn.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jk.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sx.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ek.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://jn.hnjuh.cn


<!-- 参考信息 -->