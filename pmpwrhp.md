代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://on.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bp.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tn.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eg.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ry.shxzukj.cn

================================================================================
来源：http://ce.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://nr.nicolike.cn

================================================================================
来源：http://yq.bjjhwx.cn

[M01] 读取命令行参数
来源：http://di.gzmigu.cn

Py:   sys.argv[1:]
来源：http://uo.huanxung.cn

PHP:  $argv;  $argc;
来源：http://oh.newstarts.cn

JS:   process.argv.slice(2)
来源：http://fz.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://lk.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://se.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://wm.jianghongdianzi.cn

Ruby: ARGV
来源：http://wv.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://tg.huixiangedu.cn

[M02] 读取环境变量
来源：http://bt.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://pe.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xy.nicolike.cn

JS:   process.env.HOME
来源：http://pr.bookmarksfly.cn

TS:   process.env.HOME
来源：http://rg.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ps.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hm.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://cd.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mu.wgjwhj.cn

[M03] 执行外部命令
来源：http://kc.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rq.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cc.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rh.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vs.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xh.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gs.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mk.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://gq.9csxet.cn

[M04] 获取当前工作目录
来源：http://ut.shtwfgs.cn

Py:   os.getcwd()
来源：http://oc.colortex.cn

PHP:  getcwd();
来源：http://ng.colortex.cn

JS:   process.cwd()
来源：http://sj.huanxung.cn

TS:   process.cwd()
来源：http://aw.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://dc.gzmigu.cn

Go:   os.Getwd()
来源：http://hv.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://jd.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://er.521024.cn

[M05] 设置退出码
来源：http://aa.nszjky.cn

Py:   sys.exit(1)
来源：http://yl.muxihuayi.cn

PHP:  exit(1);
来源：http://rh.chemitech.net.cn

JS:   process.exit(1)
来源：http://vv.shtwfgs.cn

TS:   process.exit(1)
来源：http://qk.bjjhwx.cn

Java: System.exit(1)
来源：http://rw.lnxyls.cn

Go:   os.Exit(1)
来源：http://oh.nszjky.cn

Ruby: exit 1
来源：http://id.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://up.shxzukj.cn

[M06] 向标准错误输出
来源：http://iz.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://uw.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rq.lnxyls.cn

JS:   console.error("err")
来源：http://tr.huixiangedu.cn

TS:   console.error("err")
来源：http://ez.shxzukj.cn

Java: System.err.println("err")
来源：http://jh.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eh.newstarts.cn

Ruby: warn "err"
来源：http://wk.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://cw.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://fd.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://th.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fs.chemitech.net.cn

JS:   require.main === module
来源：http://lk.haigaiapp.cn

TS:   require.main === module
来源：http://ft.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://xr.nicolike.cn

Go:   func main()
来源：http://nj.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wk.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://ji.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://ef.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://pv.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://wd.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://zw.shxzukj.cn

TS:   process.platform;  process.version
来源：http://sx.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kn.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jn.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uk.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zb.nszjky.cn

================================================================================
来源：http://wz.szsharing.cn

N. 数据结构与算法
来源：http://ic.newstarts.cn

================================================================================
来源：http://uu.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://sw.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dj.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ob.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kx.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rb.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xl.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ql.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lf.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fu.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://nm.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://nr.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nk.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fw.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yz.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gj.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://vn.panjiajie.cn

Ruby: arr.sort
来源：http://ev.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wb.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://kv.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://op.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://bw.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zy.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zz.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bs.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qg.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xs.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kq.jctech888.com.cn

[N04] 斐波那契数列
来源：http://ef.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rf.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gd.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ji.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dg.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fj.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cl.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://al.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cu.haigaiapp.cn

[N05] 最大公约数
来源：http://gh.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://gb.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wu.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dg.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ax.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vf.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ff.huanxung.cn

Ruby: a.gcd(b)
来源：http://pj.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bq.shxzukj.cn

[N06] 判断回文字符串
来源：http://ir.newstarts.cn

Py:   s == s[::-1]
来源：http://pj.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://jd.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://ls.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://ov.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ex.colortex.cn

Go:   // 双指针从两端比较
来源：http://qa.bjjhwx.cn

Ruby: s == s.reverse
来源：http://qy.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://to.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://yy.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bn.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yc.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://me.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://vz.bjjhwx.cn

Java: // 手写 HashMap
来源：http://oe.huanxung.cn

Go:   // 手写 map[int]int
来源：http://ef.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ak.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wq.nszjky.cn

[N08] 生成全排列
来源：http://iq.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://tx.szxytkj.cn

PHP:  // 手写递归交换
来源：http://qt.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ri.hnjuh.cn

TS:   // 手写回溯递归
来源：http://ms.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://ai.gzmigu.cn

Go:   // 手写回溯递归
来源：http://po.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://nf.asd995.cn

C#:   // 手写回溯递归
来源：http://ye.lnxyls.cn

[N09] 栈与队列
来源：http://lb.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pt.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hl.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uz.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pd.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ne.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ig.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jr.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cw.muxihuayi.cn

[N10] 链表节点定义
来源：http://lz.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mu.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xd.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aw.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ro.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://cq.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ag.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yt.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rf.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://ef.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dv.hahajie.cn

PHP:  // 手写递归函数
来源：http://sn.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://le.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vt.chemitech.net.cn

Java: // 手写递归
来源：http://cy.newstarts.cn

Go:   // 手写递归
来源：http://ev.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mw.haigaiapp.cn

C#:   // 手写递归
来源：http://ya.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wm.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://je.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eq.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eu.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rm.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://at.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jt.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yw.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://de.szxytkj.cn

================================================================================
来源：http://gk.szsharing.cn

O. 并发与异步
来源：http://zj.hnjuh.cn

================================================================================
来源：http://sp.bjjhwx.cn

[O01] 启动一个线程
来源：http://kr.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iq.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sn.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://is.colortex.cn

TS:   // 同 JS
来源：http://xb.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ct.yuntaijiaju.cn

Go:   go f()
来源：http://oy.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://es.asd995.cn

C#:   Task.Run(() => F());
来源：http://wb.yuntaijiaju.cn

[O02] 使用线程池
来源：http://up.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ih.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cy.hahajie.cn

JS:   // worker_threads 线程池
来源：http://fy.hahajie.cn

TS:   // worker_threads 线程池
来源：http://qz.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lr.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ce.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cb.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oj.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://mu.asd995.cn

Py:   with lock: shared += 1
来源：http://vn.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://qt.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fx.muxihuayi.cn

TS:   // 同 JS
来源：http://rx.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://zv.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wr.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iv.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://mc.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ms.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://el.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mk.nszjky.cn

JS:   async function f() { await g(); }
来源：http://ic.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tb.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fz.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tm.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xe.521024.cn

C#:   async Task F() { await G(); }
来源：http://jr.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://xm.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://dq.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rp.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://yi.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://yj.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gg.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://du.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://wy.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://le.colortex.cn

[O06] 使用进程池
来源：http://xo.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vl.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sd.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://to.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://bp.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ig.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ps.9csxet.cn

Ruby: // fork 块
来源：http://gt.jianghongdianzi.cn

C#:   Parallel.For
来源：http://nq.lnxyls.cn

================================================================================
来源：http://xp.panjiajie.cn

P. 常用工具函数
来源：http://we.szxytkj.cn

================================================================================
来源：http://sd.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://gz.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://um.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kl.huanxung.cn

JS:   crypto.randomUUID()
来源：http://ub.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://gj.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://se.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://gt.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://nd.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://sy.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://fb.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qy.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ab.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tz.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vn.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ug.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://na.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ld.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://az.newstarts.cn

[P03] 生成短随机字符串
来源：http://gt.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cy.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://co.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jn.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://de.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rg.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yu.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uj.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vw.shxzukj.cn

[P04] 求长度
来源：http://ir.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lm.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qk.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ce.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fm.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://mk.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://vd.9csxet.cn

Ruby: x.length;  x.size
来源：http://yt.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bx.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://gp.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ha.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bv.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ju.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oi.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uf.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hr.newstarts.cn

Ruby: a == b
来源：http://bu.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aw.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iv.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lp.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://hl.shxzskj.cn


<!-- 参考信息 -->