代发 wailian999

C#:   (int)resp.StatusCode
来源：http://bn.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ms.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qv.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://of.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cl.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://of.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tc.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://me.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://is.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nc.521024.cn

================================================================================
来源：http://ty.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://me.bjjhwx.cn

================================================================================
来源：http://kd.shxzukj.cn

[M01] 读取命令行参数
来源：http://ty.521024.cn

Py:   sys.argv[1:]
来源：http://zd.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://qx.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://wh.nszjky.cn

TS:   process.argv.slice(2)
来源：http://jn.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://jo.huanxung.cn

Go:   os.Args[1:]
来源：http://ba.nicolike.cn

Ruby: ARGV
来源：http://ja.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://up.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://ja.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://oe.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lg.521024.cn

JS:   process.env.HOME
来源：http://fe.bjjhwx.cn

TS:   process.env.HOME
来源：http://ux.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://ld.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rd.hahajie.cn

Ruby: ENV["HOME"]
来源：http://nd.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qc.shtwfgs.cn

[M03] 执行外部命令
来源：http://vz.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bc.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jv.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mi.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zu.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mc.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mg.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sm.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://xx.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://bb.hahajie.cn

Py:   os.getcwd()
来源：http://oz.chemitech.net.cn

PHP:  getcwd();
来源：http://av.lnxyls.cn

JS:   process.cwd()
来源：http://od.huixinmuqiang.cn

TS:   process.cwd()
来源：http://cv.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://go.shtwfgs.cn

Go:   os.Getwd()
来源：http://ms.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://lm.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cm.gzmigu.cn

[M05] 设置退出码
来源：http://vv.huixiangedu.cn

Py:   sys.exit(1)
来源：http://xr.wgjwhj.cn

PHP:  exit(1);
来源：http://gu.huanxung.cn

JS:   process.exit(1)
来源：http://pc.lnxyls.cn

TS:   process.exit(1)
来源：http://sw.szsharing.cn

Java: System.exit(1)
来源：http://cx.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ks.huixinmuqiang.cn

Ruby: exit 1
来源：http://pe.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wl.wgjwhj.cn

[M06] 向标准错误输出
来源：http://fe.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://du.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vu.hnjuh.cn

JS:   console.error("err")
来源：http://gp.bookmarksfly.cn

TS:   console.error("err")
来源：http://nk.bookmarksfly.cn

Java: System.err.println("err")
来源：http://sb.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nc.hahajie.cn

Ruby: warn "err"
来源：http://bo.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://ng.asd995.cn

[M07] 判断是否为主入口
来源：http://dv.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://zm.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sw.bookmarksfly.cn

JS:   require.main === module
来源：http://dg.huanxung.cn

TS:   require.main === module
来源：http://iq.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://be.521024.cn

Go:   func main()
来源：http://xn.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rx.nszjky.cn

C#:   static void Main(string[] args)
来源：http://lz.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://hw.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://la.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://zr.shxzskj.cn

JS:   process.platform;  process.version
来源：http://gz.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://pu.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://os.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://go.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fp.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ho.shxzukj.cn

================================================================================
来源：http://xb.bjjhwx.cn

N. 数据结构与算法
来源：http://pk.muxihuayi.cn

================================================================================
来源：http://sn.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://qo.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vw.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ja.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dk.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://to.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cz.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://dv.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xr.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zp.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://mg.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://kz.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ca.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sv.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ma.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ew.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://pu.colortex.cn

Ruby: arr.sort
来源：http://zm.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wn.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://bn.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://qj.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fh.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hr.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xo.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ft.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jz.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vq.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://rn.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yk.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kr.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fi.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ad.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zc.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sl.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ss.huanxung.cn

[N05] 最大公约数
来源：http://dd.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://oy.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kr.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gk.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oz.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lj.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mv.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://ho.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bm.shxzskj.cn

[N06] 判断回文字符串
来源：http://ac.hahajie.cn

Py:   s == s[::-1]
来源：http://li.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://ss.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://xr.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://hw.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sn.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ae.muxihuayi.cn

Ruby: s == s.reverse
来源：http://uy.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ib.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://za.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qb.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wd.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rm.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://yy.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://sb.newstarts.cn

Go:   // 手写 map[int]int
来源：http://fo.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://es.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xp.haigaiapp.cn

[N08] 生成全排列
来源：http://mb.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://kt.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://dg.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ry.panjiajie.cn

TS:   // 手写回溯递归
来源：http://dk.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://sl.nicolike.cn

Go:   // 手写回溯递归
来源：http://bj.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://pk.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://lh.huixiangedu.cn

[N09] 栈与队列
来源：http://cd.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tq.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dx.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ml.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yw.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://se.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ny.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ap.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ei.nicolike.cn

[N10] 链表节点定义
来源：http://pf.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cj.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zo.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qd.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vb.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://jt.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oh.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lj.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fq.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://ty.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oi.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://mw.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nc.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ft.yuexingan06.cn

Java: // 手写递归
来源：http://oe.shtwfgs.cn

Go:   // 手写递归
来源：http://uh.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xq.asd995.cn

C#:   // 手写递归
来源：http://sj.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jh.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vh.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dh.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ux.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ru.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uz.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://px.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dz.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bc.hnjuh.cn

================================================================================
来源：http://zg.colortex.cn

O. 并发与异步
来源：http://jy.521024.cn

================================================================================
来源：http://qo.wgjwhj.cn

[O01] 启动一个线程
来源：http://lw.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tq.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wc.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pe.huixiangedu.cn

TS:   // 同 JS
来源：http://je.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://mx.chemitech.net.cn

Go:   go f()
来源：http://we.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://na.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://lb.bookmarksfly.cn

[O02] 使用线程池
来源：http://yb.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pe.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iu.asd995.cn

JS:   // worker_threads 线程池
来源：http://qq.521024.cn

TS:   // worker_threads 线程池
来源：http://rp.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dw.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ic.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bn.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fe.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://fa.shxzskj.cn

Py:   with lock: shared += 1
来源：http://xt.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://oz.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oj.nszjky.cn

TS:   // 同 JS
来源：http://vx.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://cl.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cp.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pz.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ac.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://ez.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://is.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ng.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://gt.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://au.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ji.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mj.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sm.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://ig.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://jp.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://zd.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qn.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://oc.colortex.cn

TS:   await Promise.all(tasks)
来源：http://dv.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mf.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wn.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ox.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rw.colortex.cn

[O06] 使用进程池
来源：http://jr.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vg.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ig.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://ar.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://ck.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://me.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dy.chemitech.net.cn

Ruby: // fork 块
来源：http://tw.bookmarksfly.cn

C#:   Parallel.For
来源：http://jx.colortex.cn

================================================================================
来源：http://hz.lnxyls.cn

P. 常用工具函数
来源：http://xs.lnxyls.cn

================================================================================
来源：http://lo.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://pg.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://ce.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fq.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://nl.nszjky.cn

TS:   crypto.randomUUID()
来源：http://kf.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://jm.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://zk.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://jj.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://xj.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://hy.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xl.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://px.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ev.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yd.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://om.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ik.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qu.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ut.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://dv.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kv.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jx.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oj.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ce.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gw.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wz.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ca.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pp.asd995.cn

[P04] 求长度
来源：http://am.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zx.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://we.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fn.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ve.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://jm.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://vy.szsharing.cn

Ruby: x.length;  x.size
来源：http://mi.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://li.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://oq.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ol.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gq.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://il.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jb.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://em.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xa.nszjky.cn

Ruby: a == b
来源：http://bf.lnxyls.cn


<!-- 参考信息 -->