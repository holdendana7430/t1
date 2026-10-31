代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qr.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ga.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pq.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vr.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aa.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nk.shxzukj.cn

================================================================================
来源：http://cd.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://yk.nszjky.cn

================================================================================
来源：http://lg.hahajie.cn

[M01] 读取命令行参数
来源：http://ae.newstarts.cn

Py:   sys.argv[1:]
来源：http://gm.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://va.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://nt.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ra.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://gg.huanxung.cn

Go:   os.Args[1:]
来源：http://iq.huanxung.cn

Ruby: ARGV
来源：http://wo.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://qb.gzmigu.cn

[M02] 读取环境变量
来源：http://fh.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ox.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bl.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://cn.shxzskj.cn

TS:   process.env.HOME
来源：http://jh.nszjky.cn

Java: System.getenv("HOME")
来源：http://wu.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ga.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ks.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zm.jctech888.com.cn

[M03] 执行外部命令
来源：http://qi.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://de.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pk.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nk.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gw.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://by.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ti.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kt.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://ji.nszjky.cn

[M04] 获取当前工作目录
来源：http://is.panjiajie.cn

Py:   os.getcwd()
来源：http://pk.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ri.huixinmuqiang.cn

JS:   process.cwd()
来源：http://dz.yuexingan06.cn

TS:   process.cwd()
来源：http://jg.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://aq.hnjuh.cn

Go:   os.Getwd()
来源：http://ei.nicolike.cn

Ruby: Dir.pwd
来源：http://yo.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yb.asd995.cn

[M05] 设置退出码
来源：http://nc.9csxet.cn

Py:   sys.exit(1)
来源：http://rq.wgjwhj.cn

PHP:  exit(1);
来源：http://bx.muxihuayi.cn

JS:   process.exit(1)
来源：http://aw.gzmigu.cn

TS:   process.exit(1)
来源：http://jx.haigaiapp.cn

Java: System.exit(1)
来源：http://ld.haigaiapp.cn

Go:   os.Exit(1)
来源：http://hc.colortex.cn

Ruby: exit 1
来源：http://vj.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://po.wgjwhj.cn

[M06] 向标准错误输出
来源：http://og.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://sy.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pl.panjiajie.cn

JS:   console.error("err")
来源：http://oe.bjjhwx.cn

TS:   console.error("err")
来源：http://aj.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://vy.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vh.9csxet.cn

Ruby: warn "err"
来源：http://or.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://wh.colortex.cn

[M07] 判断是否为主入口
来源：http://wv.asd995.cn

Py:   if __name__ == "__main__":
来源：http://qy.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://il.panjiajie.cn

JS:   require.main === module
来源：http://de.nicolike.cn

TS:   require.main === module
来源：http://xe.szxytkj.cn

Java: public static void main(String[] args)
来源：http://jv.shxzukj.cn

Go:   func main()
来源：http://be.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hn.huanxung.cn

C#:   static void Main(string[] args)
来源：http://kl.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://yb.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://gu.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ge.nszjky.cn

JS:   process.platform;  process.version
来源：http://ga.szsharing.cn

TS:   process.platform;  process.version
来源：http://ba.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bc.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qp.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hr.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cn.shxzukj.cn

================================================================================
来源：http://dp.colortex.cn

N. 数据结构与算法
来源：http://ap.lnxyls.cn

================================================================================
来源：http://ci.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://wu.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hk.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vm.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jn.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wc.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cr.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://zk.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gx.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ya.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://rv.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://js.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ho.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ux.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cu.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://io.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://fk.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ve.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xs.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://jl.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wr.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ts.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vh.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qf.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uk.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://es.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cd.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ya.nicolike.cn

[N04] 斐波那契数列
来源：http://mz.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bq.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eh.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jc.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dd.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tp.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://km.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ak.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pl.9csxet.cn

[N05] 最大公约数
来源：http://cv.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://gd.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cv.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xb.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rj.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ie.nicolike.cn

Ruby: a.gcd(b)
来源：http://bb.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ih.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://na.huanxung.cn

Py:   s == s[::-1]
来源：http://go.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://iy.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ja.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://bo.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rp.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://ll.wgjwhj.cn

Ruby: s == s.reverse
来源：http://ua.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ek.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://hm.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ix.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cv.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vx.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://em.huixiangedu.cn

Java: // 手写 HashMap
来源：http://pt.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://nk.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://tu.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fp.muxihuayi.cn

[N08] 生成全排列
来源：http://tc.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ll.9csxet.cn

PHP:  // 手写递归交换
来源：http://ky.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://bq.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://sa.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://zz.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://wt.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://bn.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://uz.yuexingan06.cn

[N09] 栈与队列
来源：http://hi.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mo.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fj.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fu.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ga.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ho.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kj.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vw.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ri.chemitech.net.cn

[N10] 链表节点定义
来源：http://sv.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tj.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hu.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ie.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://po.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://hd.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bo.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bs.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pv.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://yn.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rn.gzmigu.cn

PHP:  // 手写递归函数
来源：http://qs.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mf.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ml.asd995.cn

Java: // 手写递归
来源：http://dy.nicolike.cn

Go:   // 手写递归
来源：http://gy.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hq.shxzskj.cn

C#:   // 手写递归
来源：http://ru.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ye.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xx.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://my.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mc.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://su.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fe.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gt.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ga.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://io.yuexingan06.cn

================================================================================
来源：http://ux.newstarts.cn

O. 并发与异步
来源：http://re.muxihuayi.cn

================================================================================
来源：http://md.szsharing.cn

[O01] 启动一个线程
来源：http://cr.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vk.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qe.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kw.shxzskj.cn

TS:   // 同 JS
来源：http://ar.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://ou.huixiangedu.cn

Go:   go f()
来源：http://pw.newstarts.cn

Ruby: Thread.new { f }
来源：http://aw.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://vw.haigaiapp.cn

[O02] 使用线程池
来源：http://bg.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jz.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wv.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://pe.9csxet.cn

TS:   // worker_threads 线程池
来源：http://dy.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ko.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://li.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hg.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mm.nicolike.cn

[O03] 加锁保护共享数据
来源：http://gh.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://sj.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://mn.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jr.wgjwhj.cn

TS:   // 同 JS
来源：http://wn.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://jg.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ri.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ek.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://nf.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://wr.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://th.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vh.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://bj.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bi.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pu.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://au.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://si.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://je.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://lk.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://nm.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jn.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://tl.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://oz.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qz.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wc.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://rd.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jf.haigaiapp.cn

[O06] 使用进程池
来源：http://nn.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qv.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ap.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://jp.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://ur.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://be.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lh.huixinmuqiang.cn

Ruby: // fork 块
来源：http://mv.bjjhwx.cn

C#:   Parallel.For
来源：http://sr.yuexingan06.cn

================================================================================
来源：http://ca.huanxung.cn

P. 常用工具函数
来源：http://gp.huanxung.cn

================================================================================
来源：http://ln.huixiangedu.cn

[P01] 生成 UUID
来源：http://cg.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://yh.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vq.colortex.cn

JS:   crypto.randomUUID()
来源：http://om.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://fp.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://eo.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://ec.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://yq.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://ca.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://px.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qn.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ed.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oy.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://el.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eu.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://il.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jh.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wv.szxytkj.cn

[P03] 生成短随机字符串
来源：http://pj.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cw.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xr.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qn.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mq.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sb.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kx.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hf.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xj.gzmigu.cn

[P04] 求长度
来源：http://lp.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://db.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tw.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zy.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eo.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://yq.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://wp.hahajie.cn

Ruby: x.length;  x.size
来源：http://jp.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xf.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ux.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://re.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jb.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cc.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zm.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nk.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cn.lnxyls.cn

Ruby: a == b
来源：http://fd.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hn.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://on.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ml.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://tx.chemitech.net.cn


<!-- 参考信息 -->