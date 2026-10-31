代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vu.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jo.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wr.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uw.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ep.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jg.shxzskj.cn

================================================================================
来源：http://hc.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://xy.panjiajie.cn

================================================================================
来源：http://ym.nszjky.cn

[M01] 读取命令行参数
来源：http://yz.shxzskj.cn

Py:   sys.argv[1:]
来源：http://um.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://mr.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://yt.nicolike.cn

TS:   process.argv.slice(2)
来源：http://bu.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://sz.panjiajie.cn

Go:   os.Args[1:]
来源：http://ps.chemitech.net.cn

Ruby: ARGV
来源：http://sk.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://nf.9csxet.cn

[M02] 读取环境变量
来源：http://ox.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://pl.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bn.huanxung.cn

JS:   process.env.HOME
来源：http://by.wgjwhj.cn

TS:   process.env.HOME
来源：http://sf.9csxet.cn

Java: System.getenv("HOME")
来源：http://uy.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rr.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://ds.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wv.nicolike.cn

[M03] 执行外部命令
来源：http://la.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wq.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://he.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ne.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lc.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://up.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sz.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wy.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://rw.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://rn.jctech888.com.cn

Py:   os.getcwd()
来源：http://bq.muxihuayi.cn

PHP:  getcwd();
来源：http://ee.jctech888.com.cn

JS:   process.cwd()
来源：http://ox.wgjwhj.cn

TS:   process.cwd()
来源：http://tc.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://np.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ha.huixiangedu.cn

Ruby: Dir.pwd
来源：http://mq.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ui.lnxyls.cn

[M05] 设置退出码
来源：http://jk.huanxung.cn

Py:   sys.exit(1)
来源：http://hl.panjiajie.cn

PHP:  exit(1);
来源：http://kk.lnxyls.cn

JS:   process.exit(1)
来源：http://yb.lnxyls.cn

TS:   process.exit(1)
来源：http://qo.hahajie.cn

Java: System.exit(1)
来源：http://gv.shxzukj.cn

Go:   os.Exit(1)
来源：http://ih.jianghongdianzi.cn

Ruby: exit 1
来源：http://ju.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ya.haigaiapp.cn

[M06] 向标准错误输出
来源：http://th.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ut.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lq.hnjuh.cn

JS:   console.error("err")
来源：http://ek.shtwfgs.cn

TS:   console.error("err")
来源：http://zg.chemitech.net.cn

Java: System.err.println("err")
来源：http://oe.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ha.haigaiapp.cn

Ruby: warn "err"
来源：http://of.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://sd.nszjky.cn

[M07] 判断是否为主入口
来源：http://br.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://xc.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ij.lnxyls.cn

JS:   require.main === module
来源：http://ru.huanxung.cn

TS:   require.main === module
来源：http://ji.asd995.cn

Java: public static void main(String[] args)
来源：http://uv.bjjhwx.cn

Go:   func main()
来源：http://ql.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ku.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://mv.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://qs.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://bn.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://cd.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://un.newstarts.cn

TS:   process.platform;  process.version
来源：http://be.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ju.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zf.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yt.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wj.muxihuayi.cn

================================================================================
来源：http://vr.huanxung.cn

N. 数据结构与算法
来源：http://ss.shxzskj.cn

================================================================================
来源：http://ij.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://qn.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ao.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mz.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ou.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://qg.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oo.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ne.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://is.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ud.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ns.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qy.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nc.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://om.newstarts.cn

Go:   slices.Sort(arr)
来源：http://fc.huanxung.cn

Ruby: arr.sort
来源：http://dl.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wp.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://cd.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hc.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://tb.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://by.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://if.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jw.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zl.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nf.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ws.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://oh.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ch.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ps.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ua.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zo.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://do.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ve.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ai.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wf.shxzskj.cn

[N05] 最大公约数
来源：http://uo.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://go.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ru.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://so.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ew.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yq.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ik.lnxyls.cn

Ruby: a.gcd(b)
来源：http://nq.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nv.haigaiapp.cn

[N06] 判断回文字符串
来源：http://aj.shxzukj.cn

Py:   s == s[::-1]
来源：http://ac.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ha.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://wd.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://md.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ej.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ek.shxzukj.cn

Ruby: s == s.reverse
来源：http://lc.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hc.colortex.cn

[N07] 两数之和（返回下标）
来源：http://qx.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cw.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bq.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ep.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ez.lnxyls.cn

Java: // 手写 HashMap
来源：http://nm.521024.cn

Go:   // 手写 map[int]int
来源：http://ib.colortex.cn

Ruby: // 手写 Hash
来源：http://ow.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bb.huanxung.cn

[N08] 生成全排列
来源：http://co.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://vv.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://es.colortex.cn

JS:   // 手写回溯递归
来源：http://ml.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://bl.chemitech.net.cn

Java: // 手写回溯递归
来源：http://jf.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://mp.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ly.nszjky.cn

C#:   // 手写回溯递归
来源：http://ea.chemitech.net.cn

[N09] 栈与队列
来源：http://bb.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fk.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ap.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vw.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://su.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ni.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ur.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gz.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rz.yuexingan06.cn

[N10] 链表节点定义
来源：http://gq.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qo.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kk.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pw.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ek.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://yx.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tl.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ce.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://zq.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wp.szsharing.cn

PHP:  // 手写递归函数
来源：http://sd.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sl.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bm.newstarts.cn

Java: // 手写递归
来源：http://mh.nszjky.cn

Go:   // 手写递归
来源：http://ah.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bf.asd995.cn

C#:   // 手写递归
来源：http://sh.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://if.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ig.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aa.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ae.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tj.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ed.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bc.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fm.colortex.cn

================================================================================
来源：http://cn.shtwfgs.cn

O. 并发与异步
来源：http://bv.yuntaijiaju.cn

================================================================================
来源：http://fu.bjjhwx.cn

[O01] 启动一个线程
来源：http://hr.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bl.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oj.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nr.jctech888.com.cn

TS:   // 同 JS
来源：http://zq.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://sl.nicolike.cn

Go:   go f()
来源：http://hy.asd995.cn

Ruby: Thread.new { f }
来源：http://ix.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://jl.hahajie.cn

[O02] 使用线程池
来源：http://ok.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wg.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qh.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://ur.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://gx.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mv.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ft.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://er.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://de.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://ic.lnxyls.cn

Py:   with lock: shared += 1
来源：http://th.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://cy.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://my.bookmarksfly.cn

TS:   // 同 JS
来源：http://zj.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://mj.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hx.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ch.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://aw.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://nl.colortex.cn

Py:   async def f():⏎    await g()
来源：http://qp.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vs.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://dm.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://db.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kb.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bw.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wg.asd995.cn

C#:   async Task F() { await G(); }
来源：http://qb.521024.cn

[O05] 并发执行并等待全部完成
来源：http://db.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://nm.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ub.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://or.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://oc.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pd.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zk.colortex.cn

Ruby: threads.map(&:join)
来源：http://in.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ap.muxihuayi.cn

[O06] 使用进程池
来源：http://na.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rr.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zh.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://yn.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://hu.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hu.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nk.chemitech.net.cn

Ruby: // fork 块
来源：http://io.newstarts.cn

C#:   Parallel.For
来源：http://cp.nicolike.cn

================================================================================
来源：http://fq.huanxung.cn

P. 常用工具函数
来源：http://tj.shtwfgs.cn

================================================================================
来源：http://fn.hnjuh.cn

[P01] 生成 UUID
来源：http://ig.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://xv.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rr.szsharing.cn

JS:   crypto.randomUUID()
来源：http://dx.9csxet.cn

TS:   crypto.randomUUID()
来源：http://fc.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://yj.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://dv.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://re.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://gm.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://ui.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xr.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bc.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mv.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://il.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://se.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iu.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ez.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fj.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://uz.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ec.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yp.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jw.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dp.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jb.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://es.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hg.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://as.jctech888.com.cn

[P04] 求长度
来源：http://ps.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ti.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ft.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nw.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wl.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://zs.nszjky.cn

Go:   len(arr);  len(m)
来源：http://vs.hahajie.cn

Ruby: x.length;  x.size
来源：http://ol.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yy.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://ua.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hs.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://op.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lb.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qd.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vz.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ky.haigaiapp.cn

Ruby: a == b
来源：http://iv.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ls.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ae.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ka.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://on.huixinmuqiang.cn


<!-- 参考信息 -->