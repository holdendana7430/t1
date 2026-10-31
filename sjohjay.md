代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dh.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zh.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gz.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rk.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://up.bjjhwx.cn

================================================================================
来源：http://bg.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://xt.nszjky.cn

================================================================================
来源：http://yq.521024.cn

[M01] 读取命令行参数
来源：http://re.shxzskj.cn

Py:   sys.argv[1:]
来源：http://kx.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://ht.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://iu.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://th.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://dq.gzmigu.cn

Go:   os.Args[1:]
来源：http://no.9csxet.cn

Ruby: ARGV
来源：http://nq.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://ra.bjjhwx.cn

[M02] 读取环境变量
来源：http://sm.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://vi.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ds.panjiajie.cn

JS:   process.env.HOME
来源：http://sd.lnxyls.cn

TS:   process.env.HOME
来源：http://qt.huanxung.cn

Java: System.getenv("HOME")
来源：http://bj.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://td.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ol.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ms.haigaiapp.cn

[M03] 执行外部命令
来源：http://ez.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pr.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vr.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ln.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jr.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rp.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hv.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ma.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ow.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ee.nszjky.cn

Py:   os.getcwd()
来源：http://ez.huixinmuqiang.cn

PHP:  getcwd();
来源：http://gg.jctech888.com.cn

JS:   process.cwd()
来源：http://wq.chemitech.net.cn

TS:   process.cwd()
来源：http://jo.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://lu.wgjwhj.cn

Go:   os.Getwd()
来源：http://gd.colortex.cn

Ruby: Dir.pwd
来源：http://jb.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://re.wgjwhj.cn

[M05] 设置退出码
来源：http://qo.shtwfgs.cn

Py:   sys.exit(1)
来源：http://uy.9csxet.cn

PHP:  exit(1);
来源：http://py.panjiajie.cn

JS:   process.exit(1)
来源：http://fi.panjiajie.cn

TS:   process.exit(1)
来源：http://mt.bookmarksfly.cn

Java: System.exit(1)
来源：http://cq.bjjhwx.cn

Go:   os.Exit(1)
来源：http://fc.shxzukj.cn

Ruby: exit 1
来源：http://on.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://br.muxihuayi.cn

[M06] 向标准错误输出
来源：http://sz.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://lm.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iu.colortex.cn

JS:   console.error("err")
来源：http://nx.huixiangedu.cn

TS:   console.error("err")
来源：http://qv.wgjwhj.cn

Java: System.err.println("err")
来源：http://qu.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rq.shxzskj.cn

Ruby: warn "err"
来源：http://et.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://mq.9csxet.cn

[M07] 判断是否为主入口
来源：http://jm.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://mi.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ju.9csxet.cn

JS:   require.main === module
来源：http://td.shxzukj.cn

TS:   require.main === module
来源：http://if.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://tx.nszjky.cn

Go:   func main()
来源：http://tq.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mf.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://mn.521024.cn

[M08] 获取系统与运行时信息
来源：http://zj.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://mz.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://du.colortex.cn

JS:   process.platform;  process.version
来源：http://um.colortex.cn

TS:   process.platform;  process.version
来源：http://qz.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ve.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fs.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xz.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cg.colortex.cn

================================================================================
来源：http://li.haigaiapp.cn

N. 数据结构与算法
来源：http://ob.huixiangedu.cn

================================================================================
来源：http://kv.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://fu.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pu.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ek.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://za.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vi.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jx.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bn.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zn.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gk.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ol.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://wj.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ga.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gg.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ir.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sy.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://oy.nszjky.cn

Ruby: arr.sort
来源：http://fd.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://as.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://vz.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pi.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://sh.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fo.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hx.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jd.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hf.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pn.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hf.hahajie.cn

[N04] 斐波那契数列
来源：http://bm.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sm.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mr.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yq.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qj.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wj.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://na.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lh.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://or.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ac.hahajie.cn

Py:   math.gcd(a, b)
来源：http://gc.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yy.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tt.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://el.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ua.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wb.colortex.cn

Ruby: a.gcd(b)
来源：http://jd.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bq.nszjky.cn

[N06] 判断回文字符串
来源：http://ai.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ix.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://zn.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://ol.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ys.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fz.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://pd.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://sf.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zi.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://ts.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zk.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hj.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ih.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ju.shtwfgs.cn

Java: // 手写 HashMap
来源：http://zz.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://xb.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://ad.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hc.shxzukj.cn

[N08] 生成全排列
来源：http://xe.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://no.shxzskj.cn

PHP:  // 手写递归交换
来源：http://hc.nszjky.cn

JS:   // 手写回溯递归
来源：http://zi.shxzukj.cn

TS:   // 手写回溯递归
来源：http://wf.muxihuayi.cn

Java: // 手写回溯递归
来源：http://eq.hahajie.cn

Go:   // 手写回溯递归
来源：http://ll.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://wu.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://ba.bookmarksfly.cn

[N09] 栈与队列
来源：http://tv.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lp.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ga.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kk.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rn.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://el.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yw.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rf.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qd.9csxet.cn

[N10] 链表节点定义
来源：http://lo.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fh.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bp.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sj.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ld.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://xb.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gx.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://km.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ey.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://ot.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vf.szsharing.cn

PHP:  // 手写递归函数
来源：http://la.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wg.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rl.yuexingan06.cn

Java: // 手写递归
来源：http://qe.gzmigu.cn

Go:   // 手写递归
来源：http://uo.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ji.shxzskj.cn

C#:   // 手写递归
来源：http://zv.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mi.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yi.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dl.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://je.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vr.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xu.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wv.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wz.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.asd995.cn

================================================================================
来源：http://by.huixinmuqiang.cn

O. 并发与异步
来源：http://ei.gzmigu.cn

================================================================================
来源：http://pn.szxytkj.cn

[O01] 启动一个线程
来源：http://it.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://or.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ly.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://is.jianghongdianzi.cn

TS:   // 同 JS
来源：http://nr.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://sc.jctech888.com.cn

Go:   go f()
来源：http://er.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://wd.asd995.cn

C#:   Task.Run(() => F());
来源：http://rn.muxihuayi.cn

[O02] 使用线程池
来源：http://xj.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bw.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uh.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ol.nicolike.cn

TS:   // worker_threads 线程池
来源：http://lr.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vc.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nd.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gc.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pd.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://uc.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://jz.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kw.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rs.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ih.521024.cn

Java: synchronized (this) { shared++; }
来源：http://cv.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://av.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://si.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://hn.asd995.cn

[O04] 定义异步函数并等待
来源：http://jl.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://jq.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ou.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://vq.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fo.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vq.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qg.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ly.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://qu.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://lc.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://xm.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xp.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://in.asd995.cn

TS:   await Promise.all(tasks)
来源：http://rl.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mz.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iq.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://uy.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vp.521024.cn

[O06] 使用进程池
来源：http://xi.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fp.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ju.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://yx.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://dz.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://az.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dz.bjjhwx.cn

Ruby: // fork 块
来源：http://mq.9csxet.cn

C#:   Parallel.For
来源：http://gd.hnjuh.cn

================================================================================
来源：http://qo.shxzukj.cn

P. 常用工具函数
来源：http://dk.nszjky.cn

================================================================================
来源：http://en.lnxyls.cn

[P01] 生成 UUID
来源：http://bj.asd995.cn

Py:   str(uuid.uuid4())
来源：http://fx.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ps.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://cs.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://bs.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://gi.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://rr.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://hb.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://vw.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://sk.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zh.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zm.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hj.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xs.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qs.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://di.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cw.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dh.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://eg.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uh.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jh.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mf.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rj.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eq.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wp.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tv.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gr.jianghongdianzi.cn

[P04] 求长度
来源：http://ml.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gw.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qp.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yj.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vn.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://bl.nicolike.cn

Go:   len(arr);  len(m)
来源：http://fu.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://cs.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bh.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://zf.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fj.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://th.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ph.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sh.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ft.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vo.muxihuayi.cn

Ruby: a == b
来源：http://hb.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pt.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bf.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yv.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://hk.bookmarksfly.cn


<!-- 参考信息 -->