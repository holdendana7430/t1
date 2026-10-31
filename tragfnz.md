代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tz.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://al.lnxyls.cn

================================================================================
来源：http://hp.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://qq.szsharing.cn

================================================================================
来源：http://rl.bjjhwx.cn

[M01] 读取命令行参数
来源：http://cq.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://tm.asd995.cn

PHP:  $argv;  $argc;
来源：http://ol.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://lj.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://aa.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://jn.hnjuh.cn

Go:   os.Args[1:]
来源：http://ru.szxytkj.cn

Ruby: ARGV
来源：http://zk.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://mu.wgjwhj.cn

[M02] 读取环境变量
来源：http://ta.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://oi.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sa.bjjhwx.cn

JS:   process.env.HOME
来源：http://bo.huixiangedu.cn

TS:   process.env.HOME
来源：http://pk.9csxet.cn

Java: System.getenv("HOME")
来源：http://fd.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yi.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://kb.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aj.shtwfgs.cn

[M03] 执行外部命令
来源：http://zt.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zo.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zy.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ij.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zl.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rz.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ye.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dg.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://hg.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://hh.bookmarksfly.cn

Py:   os.getcwd()
来源：http://wp.shxzskj.cn

PHP:  getcwd();
来源：http://lt.wgjwhj.cn

JS:   process.cwd()
来源：http://of.asd995.cn

TS:   process.cwd()
来源：http://pe.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://ue.muxihuayi.cn

Go:   os.Getwd()
来源：http://zk.shxzskj.cn

Ruby: Dir.pwd
来源：http://dx.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lu.hnjuh.cn

[M05] 设置退出码
来源：http://fh.szsharing.cn

Py:   sys.exit(1)
来源：http://ci.szxytkj.cn

PHP:  exit(1);
来源：http://ip.szxytkj.cn

JS:   process.exit(1)
来源：http://ll.asd995.cn

TS:   process.exit(1)
来源：http://qt.huixinmuqiang.cn

Java: System.exit(1)
来源：http://mh.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ue.shxzukj.cn

Ruby: exit 1
来源：http://oj.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xx.lnxyls.cn

[M06] 向标准错误输出
来源：http://kw.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://al.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ki.9csxet.cn

JS:   console.error("err")
来源：http://mi.colortex.cn

TS:   console.error("err")
来源：http://vc.shxzskj.cn

Java: System.err.println("err")
来源：http://xv.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cv.gzmigu.cn

Ruby: warn "err"
来源：http://mv.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://dv.gzmigu.cn

[M07] 判断是否为主入口
来源：http://qe.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://sg.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fa.panjiajie.cn

JS:   require.main === module
来源：http://cc.shtwfgs.cn

TS:   require.main === module
来源：http://hi.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://wu.huanxung.cn

Go:   func main()
来源：http://jj.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zv.nszjky.cn

C#:   static void Main(string[] args)
来源：http://fb.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://hk.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://ya.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://ap.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://vk.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://fi.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nd.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jg.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rx.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zr.lnxyls.cn

================================================================================
来源：http://jd.bjjhwx.cn

N. 数据结构与算法
来源：http://vu.bookmarksfly.cn

================================================================================
来源：http://an.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://fe.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ek.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mi.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ro.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ql.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jm.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://lv.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://py.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lk.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://su.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://rz.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bf.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://um.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zf.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vx.newstarts.cn

Go:   slices.Sort(arr)
来源：http://mk.jianghongdianzi.cn

Ruby: arr.sort
来源：http://yo.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rt.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://sn.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pc.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://bc.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nt.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://po.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yp.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://um.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qi.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pn.nicolike.cn

[N04] 斐波那契数列
来源：http://lt.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uc.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iz.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pm.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yo.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xs.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pw.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kq.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pe.yuexingan06.cn

[N05] 最大公约数
来源：http://ck.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://ju.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gc.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zv.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ze.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mp.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uw.nszjky.cn

Ruby: a.gcd(b)
来源：http://vy.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ox.lnxyls.cn

[N06] 判断回文字符串
来源：http://rd.asd995.cn

Py:   s == s[::-1]
来源：http://ve.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://il.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://zx.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://zg.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nz.521024.cn

Go:   // 双指针从两端比较
来源：http://lb.szxytkj.cn

Ruby: s == s.reverse
来源：http://vj.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zh.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://cq.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nu.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://as.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ui.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ci.panjiajie.cn

Java: // 手写 HashMap
来源：http://xc.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://ci.panjiajie.cn

Ruby: // 手写 Hash
来源：http://sl.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tz.yuexingan06.cn

[N08] 生成全排列
来源：http://mn.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ws.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://yn.lnxyls.cn

JS:   // 手写回溯递归
来源：http://rs.asd995.cn

TS:   // 手写回溯递归
来源：http://zw.shxzskj.cn

Java: // 手写回溯递归
来源：http://qu.colortex.cn

Go:   // 手写回溯递归
来源：http://iz.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ut.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://ag.yuntaijiaju.cn

[N09] 栈与队列
来源：http://rp.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tt.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uc.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rz.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sq.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yx.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kt.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fb.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kh.521024.cn

[N10] 链表节点定义
来源：http://jj.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://je.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zr.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bx.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mw.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://cy.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mh.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bt.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pk.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://ja.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nd.shxzskj.cn

PHP:  // 手写递归函数
来源：http://uh.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yt.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://up.shxzukj.cn

Java: // 手写递归
来源：http://ls.lnxyls.cn

Go:   // 手写递归
来源：http://qu.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jr.haigaiapp.cn

C#:   // 手写递归
来源：http://ng.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lq.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yb.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ni.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nc.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qf.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://le.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bv.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yu.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tz.huixinmuqiang.cn

================================================================================
来源：http://nj.haigaiapp.cn

O. 并发与异步
来源：http://ed.colortex.cn

================================================================================
来源：http://tv.hahajie.cn

[O01] 启动一个线程
来源：http://yn.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nk.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rs.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bv.asd995.cn

TS:   // 同 JS
来源：http://qb.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://xr.muxihuayi.cn

Go:   go f()
来源：http://vr.hahajie.cn

Ruby: Thread.new { f }
来源：http://jh.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://nh.9csxet.cn

[O02] 使用线程池
来源：http://uw.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ew.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ux.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://dq.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://rk.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oe.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yf.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rq.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nf.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://hn.9csxet.cn

Py:   with lock: shared += 1
来源：http://tc.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://co.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ok.bjjhwx.cn

TS:   // 同 JS
来源：http://dl.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://bi.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://il.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ai.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://wf.521024.cn

[O04] 定义异步函数并等待
来源：http://od.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://yj.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sy.newstarts.cn

JS:   async function f() { await g(); }
来源：http://qc.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xb.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qg.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qo.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://az.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://xt.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://cd.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ui.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ok.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ob.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://rn.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hg.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qq.nszjky.cn

Ruby: threads.map(&:join)
来源：http://nq.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xb.yuntaijiaju.cn

[O06] 使用进程池
来源：http://dp.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ub.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xl.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://ej.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ft.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://py.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nl.521024.cn

Ruby: // fork 块
来源：http://yv.asd995.cn

C#:   Parallel.For
来源：http://nf.huixiangedu.cn

================================================================================
来源：http://md.bjjhwx.cn

P. 常用工具函数
来源：http://ml.newstarts.cn

================================================================================
来源：http://gc.huanxung.cn

[P01] 生成 UUID
来源：http://yr.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://my.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kq.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://pt.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://dl.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://ww.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://fv.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://ge.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://bi.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://qe.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bd.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yw.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://om.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ko.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qi.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ao.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kb.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dq.szxytkj.cn

[P03] 生成短随机字符串
来源：http://xj.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sh.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ez.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hi.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jq.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ui.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dj.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uo.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yy.huanxung.cn

[P04] 求长度
来源：http://sm.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://at.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cg.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kz.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qz.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://fe.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://qx.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://gb.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hs.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://kt.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gv.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ks.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zq.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lh.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pv.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gq.shxzskj.cn

Ruby: a == b
来源：http://xx.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gf.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pr.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sh.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://bq.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gn.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://kr.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vv.asd995.cn

Go:   if x == nil {}
来源：http://ds.9csxet.cn


<!-- 参考信息 -->