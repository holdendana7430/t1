代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pt.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vr.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oj.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qi.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ma.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://au.muxihuayi.cn

================================================================================
来源：http://by.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://pn.panjiajie.cn

================================================================================
来源：http://oy.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://cw.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://nn.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ps.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://wb.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://fm.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://aa.shxzskj.cn

Go:   os.Args[1:]
来源：http://ao.shtwfgs.cn

Ruby: ARGV
来源：http://zk.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://fa.nszjky.cn

[M02] 读取环境变量
来源：http://mt.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://cg.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nb.shtwfgs.cn

JS:   process.env.HOME
来源：http://dp.huanxung.cn

TS:   process.env.HOME
来源：http://ml.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://ee.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qo.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://yy.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rp.newstarts.cn

[M03] 执行外部命令
来源：http://lf.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cu.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vt.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ri.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cr.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xf.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ec.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zg.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://rc.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://yx.jctech888.com.cn

Py:   os.getcwd()
来源：http://yt.bjjhwx.cn

PHP:  getcwd();
来源：http://wr.szxytkj.cn

JS:   process.cwd()
来源：http://mn.yuexingan06.cn

TS:   process.cwd()
来源：http://mq.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ro.nicolike.cn

Go:   os.Getwd()
来源：http://bi.newstarts.cn

Ruby: Dir.pwd
来源：http://lg.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ae.haigaiapp.cn

[M05] 设置退出码
来源：http://lu.wgjwhj.cn

Py:   sys.exit(1)
来源：http://zj.szxytkj.cn

PHP:  exit(1);
来源：http://pu.lnxyls.cn

JS:   process.exit(1)
来源：http://ki.521024.cn

TS:   process.exit(1)
来源：http://rx.muxihuayi.cn

Java: System.exit(1)
来源：http://qh.nicolike.cn

Go:   os.Exit(1)
来源：http://tl.yuntaijiaju.cn

Ruby: exit 1
来源：http://yn.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ki.newstarts.cn

[M06] 向标准错误输出
来源：http://nl.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://zd.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rs.shxzukj.cn

JS:   console.error("err")
来源：http://dp.huanxung.cn

TS:   console.error("err")
来源：http://zu.nszjky.cn

Java: System.err.println("err")
来源：http://am.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ff.colortex.cn

Ruby: warn "err"
来源：http://kj.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://tj.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://fp.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://jd.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bv.chemitech.net.cn

JS:   require.main === module
来源：http://eb.shxzukj.cn

TS:   require.main === module
来源：http://wj.nszjky.cn

Java: public static void main(String[] args)
来源：http://ji.newstarts.cn

Go:   func main()
来源：http://mt.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fz.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ds.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://ux.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ik.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xg.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://lw.panjiajie.cn

TS:   process.platform;  process.version
来源：http://lm.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vy.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ju.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hy.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://af.hnjuh.cn

================================================================================
来源：http://iu.szsharing.cn

N. 数据结构与算法
来源：http://gh.hnjuh.cn

================================================================================
来源：http://oc.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://mq.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jj.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ov.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://be.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rp.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ra.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://ew.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ts.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pu.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://zb.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ai.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kn.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vb.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lm.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mh.hahajie.cn

Go:   slices.Sort(arr)
来源：http://xw.yuntaijiaju.cn

Ruby: arr.sort
来源：http://uy.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kj.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://qz.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fl.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://wt.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mu.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kj.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cn.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ad.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lz.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tk.gzmigu.cn

[N04] 斐波那契数列
来源：http://mr.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ys.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qr.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://go.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vp.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fu.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ee.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://en.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fi.asd995.cn

[N05] 最大公约数
来源：http://kt.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://al.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ia.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sg.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rn.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dy.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ys.hnjuh.cn

Ruby: a.gcd(b)
来源：http://dh.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oz.colortex.cn

[N06] 判断回文字符串
来源：http://ot.chemitech.net.cn

Py:   s == s[::-1]
来源：http://by.nszjky.cn

PHP:  $s === strrev($s);
来源：http://jt.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://hv.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://gt.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iw.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://he.colortex.cn

Ruby: s == s.reverse
来源：http://xa.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pu.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://se.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cg.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qo.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uc.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://mm.haigaiapp.cn

Java: // 手写 HashMap
来源：http://zr.huanxung.cn

Go:   // 手写 map[int]int
来源：http://sm.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://sq.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ey.shxzukj.cn

[N08] 生成全排列
来源：http://qe.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://mw.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://zt.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://mg.huanxung.cn

TS:   // 手写回溯递归
来源：http://kj.muxihuayi.cn

Java: // 手写回溯递归
来源：http://pw.colortex.cn

Go:   // 手写回溯递归
来源：http://tf.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://mj.szxytkj.cn

C#:   // 手写回溯递归
来源：http://in.yuntaijiaju.cn

[N09] 栈与队列
来源：http://gv.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ws.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oc.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xn.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dl.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vl.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://op.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fj.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ac.huanxung.cn

[N10] 链表节点定义
来源：http://yp.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ax.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mb.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xt.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cf.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://up.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://or.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kg.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ca.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://pq.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://si.asd995.cn

PHP:  // 手写递归函数
来源：http://kv.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yw.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xt.wgjwhj.cn

Java: // 手写递归
来源：http://no.shxzukj.cn

Go:   // 手写递归
来源：http://xf.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wk.jianghongdianzi.cn

C#:   // 手写递归
来源：http://uz.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pt.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cf.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tf.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wf.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vb.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fp.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vj.nicolike.cn

================================================================================
来源：http://me.haigaiapp.cn

O. 并发与异步
来源：http://us.newstarts.cn

================================================================================
来源：http://yq.bjjhwx.cn

[O01] 启动一个线程
来源：http://rb.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ed.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ro.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tk.hnjuh.cn

TS:   // 同 JS
来源：http://cc.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://gt.jianghongdianzi.cn

Go:   go f()
来源：http://nm.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://ez.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://fw.yuntaijiaju.cn

[O02] 使用线程池
来源：http://qm.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kd.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yi.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://zf.newstarts.cn

TS:   // worker_threads 线程池
来源：http://ub.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gb.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tm.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dn.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ga.newstarts.cn

[O03] 加锁保护共享数据
来源：http://nd.521024.cn

Py:   with lock: shared += 1
来源：http://uv.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ef.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pj.newstarts.cn

TS:   // 同 JS
来源：http://bl.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://qu.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qx.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hv.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://pm.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://ru.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ci.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dv.nszjky.cn

JS:   async function f() { await g(); }
来源：http://yi.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hc.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://be.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://au.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://at.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://qs.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://om.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://sb.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uu.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://is.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://uh.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qu.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ej.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://dd.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ir.yuexingan06.cn

[O06] 使用进程池
来源：http://lz.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ep.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kw.521024.cn

JS:   // child_process / cluster 模块
来源：http://ou.colortex.cn

TS:   // child_process / cluster 模块
来源：http://jq.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wg.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ys.bjjhwx.cn

Ruby: // fork 块
来源：http://ke.gzmigu.cn

C#:   Parallel.For
来源：http://uq.hnjuh.cn

================================================================================
来源：http://wg.muxihuayi.cn

P. 常用工具函数
来源：http://ar.szsharing.cn

================================================================================
来源：http://tw.panjiajie.cn

[P01] 生成 UUID
来源：http://ep.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://du.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://km.colortex.cn

JS:   crypto.randomUUID()
来源：http://vo.szsharing.cn

TS:   crypto.randomUUID()
来源：http://fo.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://bg.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://zl.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://ew.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://wp.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ic.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://je.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gs.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wd.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hg.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pt.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zn.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tc.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vm.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://ry.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ny.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jk.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mk.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uq.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mo.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dp.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://un.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wo.chemitech.net.cn

[P04] 求长度
来源：http://ek.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ry.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wi.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zh.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://co.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://dw.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ae.szxytkj.cn

Ruby: x.length;  x.size
来源：http://kq.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zo.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://fi.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iq.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tt.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ax.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vl.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xi.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aa.shxzskj.cn

Ruby: a == b
来源：http://bo.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pg.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ii.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dl.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://ab.gzmigu.cn


<!-- 参考信息 -->