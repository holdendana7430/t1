代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sl.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://at.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xi.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://md.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uf.haigaiapp.cn

================================================================================
来源：http://tc.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://hk.bookmarksfly.cn

================================================================================
来源：http://bt.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://bg.panjiajie.cn

Py:   sys.argv[1:]
来源：http://mc.nszjky.cn

PHP:  $argv;  $argc;
来源：http://bz.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://nz.colortex.cn

TS:   process.argv.slice(2)
来源：http://hx.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://qh.shxzskj.cn

Go:   os.Args[1:]
来源：http://oz.nicolike.cn

Ruby: ARGV
来源：http://nb.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://le.panjiajie.cn

[M02] 读取环境变量
来源：http://vt.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://td.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bt.9csxet.cn

JS:   process.env.HOME
来源：http://ep.hnjuh.cn

TS:   process.env.HOME
来源：http://wo.hahajie.cn

Java: System.getenv("HOME")
来源：http://jl.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fy.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://mk.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ri.szsharing.cn

[M03] 执行外部命令
来源：http://jt.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vg.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lh.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ux.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ri.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://an.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pq.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ei.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://kv.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://ul.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://rl.huixiangedu.cn

PHP:  getcwd();
来源：http://tk.huanxung.cn

JS:   process.cwd()
来源：http://bf.yuntaijiaju.cn

TS:   process.cwd()
来源：http://vw.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://vt.yuexingan06.cn

Go:   os.Getwd()
来源：http://ji.newstarts.cn

Ruby: Dir.pwd
来源：http://yf.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ir.muxihuayi.cn

[M05] 设置退出码
来源：http://un.chemitech.net.cn

Py:   sys.exit(1)
来源：http://yl.shtwfgs.cn

PHP:  exit(1);
来源：http://mn.wgjwhj.cn

JS:   process.exit(1)
来源：http://lj.521024.cn

TS:   process.exit(1)
来源：http://cd.hahajie.cn

Java: System.exit(1)
来源：http://ao.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://ft.huanxung.cn

Ruby: exit 1
来源：http://fs.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mw.521024.cn

[M06] 向标准错误输出
来源：http://za.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://xw.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rg.gzmigu.cn

JS:   console.error("err")
来源：http://hs.shxzskj.cn

TS:   console.error("err")
来源：http://iq.muxihuayi.cn

Java: System.err.println("err")
来源：http://vo.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bp.jctech888.com.cn

Ruby: warn "err"
来源：http://ii.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://rk.huanxung.cn

[M07] 判断是否为主入口
来源：http://ec.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://wm.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yl.shxzukj.cn

JS:   require.main === module
来源：http://ph.haigaiapp.cn

TS:   require.main === module
来源：http://qj.asd995.cn

Java: public static void main(String[] args)
来源：http://nf.nszjky.cn

Go:   func main()
来源：http://dv.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ks.newstarts.cn

C#:   static void Main(string[] args)
来源：http://qn.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://sd.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://fo.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://vo.shxzskj.cn

JS:   process.platform;  process.version
来源：http://by.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://tt.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uk.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yk.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ly.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jz.asd995.cn

================================================================================
来源：http://le.asd995.cn

N. 数据结构与算法
来源：http://pe.colortex.cn

================================================================================
来源：http://hj.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://ax.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wr.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eh.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oe.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gq.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hm.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://wq.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hu.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dl.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ng.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sk.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ej.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qx.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ge.colortex.cn

Go:   slices.Sort(arr)
来源：http://of.yuexingan06.cn

Ruby: arr.sort
来源：http://zi.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dt.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://tk.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ro.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://zm.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://le.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ur.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ti.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ab.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dd.yuexingan06.cn

[N04] 斐波那契数列
来源：http://fl.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zf.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hh.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gv.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tr.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hr.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://od.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jm.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wh.yuexingan06.cn

[N05] 最大公约数
来源：http://ct.asd995.cn

Py:   math.gcd(a, b)
来源：http://wf.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kg.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sx.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fv.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iw.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mk.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://gu.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yb.shtwfgs.cn

[N06] 判断回文字符串
来源：http://cj.hahajie.cn

Py:   s == s[::-1]
来源：http://cb.newstarts.cn

PHP:  $s === strrev($s);
来源：http://ae.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://yk.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://kz.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pv.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://es.hahajie.cn

Ruby: s == s.reverse
来源：http://sx.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cg.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://dj.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://br.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://in.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xi.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://wz.huixiangedu.cn

Java: // 手写 HashMap
来源：http://rp.colortex.cn

Go:   // 手写 map[int]int
来源：http://fd.newstarts.cn

Ruby: // 手写 Hash
来源：http://by.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kt.huixiangedu.cn

[N08] 生成全排列
来源：http://tb.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://jm.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://fo.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://mj.shxzskj.cn

TS:   // 手写回溯递归
来源：http://pb.jctech888.com.cn

Java: // 手写回溯递归
来源：http://qk.gzmigu.cn

Go:   // 手写回溯递归
来源：http://qj.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://gb.nszjky.cn

C#:   // 手写回溯递归
来源：http://hu.szxytkj.cn

[N09] 栈与队列
来源：http://bp.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://af.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://at.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://om.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ye.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jl.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bf.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ql.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rm.colortex.cn

[N10] 链表节点定义
来源：http://ec.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ex.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ds.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tj.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ls.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://wb.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pe.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fg.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qs.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ob.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vx.gzmigu.cn

PHP:  // 手写递归函数
来源：http://do.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oe.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uu.shtwfgs.cn

Java: // 手写递归
来源：http://hv.gzmigu.cn

Go:   // 手写递归
来源：http://wv.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://et.shtwfgs.cn

C#:   // 手写递归
来源：http://sr.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yu.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lr.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://do.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dm.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oh.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kn.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://as.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://az.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rk.gzmigu.cn

================================================================================
来源：http://br.colortex.cn

O. 并发与异步
来源：http://dt.hnjuh.cn

================================================================================
来源：http://ue.shxzukj.cn

[O01] 启动一个线程
来源：http://ni.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jx.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yw.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fw.szsharing.cn

TS:   // 同 JS
来源：http://ev.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://lx.huixinmuqiang.cn

Go:   go f()
来源：http://cg.521024.cn

Ruby: Thread.new { f }
来源：http://co.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://om.gzmigu.cn

[O02] 使用线程池
来源：http://he.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eo.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kx.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://me.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://gt.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://np.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://os.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gv.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fd.szsharing.cn

[O03] 加锁保护共享数据
来源：http://jw.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ke.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://qp.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ny.jctech888.com.cn

TS:   // 同 JS
来源：http://ik.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://hj.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dk.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ov.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://wc.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://gr.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://qw.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://av.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://as.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qz.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ei.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ka.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hp.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nd.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://ke.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://my.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cr.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://uw.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ku.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://un.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tz.huanxung.cn

Ruby: threads.map(&:join)
来源：http://kq.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://py.9csxet.cn

[O06] 使用进程池
来源：http://ch.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tb.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xy.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://lt.asd995.cn

TS:   // child_process / cluster 模块
来源：http://xs.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kv.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://po.gzmigu.cn

Ruby: // fork 块
来源：http://wr.shtwfgs.cn

C#:   Parallel.For
来源：http://gs.jctech888.com.cn

================================================================================
来源：http://uh.lnxyls.cn

P. 常用工具函数
来源：http://qw.panjiajie.cn

================================================================================
来源：http://eg.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://ej.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://ze.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uh.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://mn.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://np.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://xw.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://pe.colortex.cn

Ruby: SecureRandom.uuid
来源：http://nh.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://qn.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ip.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ca.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ry.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tx.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pe.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mw.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xh.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yr.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://do.lnxyls.cn

[P03] 生成短随机字符串
来源：http://fm.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mo.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lp.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bm.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lq.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://os.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bq.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gm.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wh.szsharing.cn

[P04] 求长度
来源：http://dj.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lt.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fm.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bf.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://id.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://kb.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://hm.szsharing.cn

Ruby: x.length;  x.size
来源：http://td.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tu.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://hf.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gu.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tx.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zg.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mb.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sg.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zq.szxytkj.cn

Ruby: a == b
来源：http://az.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zr.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qw.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sl.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://wb.panjiajie.cn


<!-- 参考信息 -->