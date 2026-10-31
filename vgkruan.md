代发 wailian999

C#:   (int)resp.StatusCode
来源：http://qs.9csxet.cn

[L08] 并发请求多个地址
来源：http://rj.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kw.521024.cn

PHP:  curl_multi_init() 系列
来源：http://kk.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vv.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fs.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tz.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lv.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xi.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fy.shxzskj.cn

================================================================================
来源：http://qu.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://xw.asd995.cn

================================================================================
来源：http://lm.nicolike.cn

[M01] 读取命令行参数
来源：http://cl.colortex.cn

Py:   sys.argv[1:]
来源：http://pv.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://uq.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://bj.colortex.cn

TS:   process.argv.slice(2)
来源：http://dl.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://li.jctech888.com.cn

Go:   os.Args[1:]
来源：http://kr.huixiangedu.cn

Ruby: ARGV
来源：http://ej.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://gv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://kx.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://ee.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qn.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ra.szsharing.cn

TS:   process.env.HOME
来源：http://iv.szxytkj.cn

Java: System.getenv("HOME")
来源：http://em.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://td.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://dt.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xp.bjjhwx.cn

[M03] 执行外部命令
来源：http://ze.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hq.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eq.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gp.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oi.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://av.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ud.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xf.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://yo.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://pn.521024.cn

Py:   os.getcwd()
来源：http://xu.lnxyls.cn

PHP:  getcwd();
来源：http://ou.gzmigu.cn

JS:   process.cwd()
来源：http://ki.asd995.cn

TS:   process.cwd()
来源：http://za.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://yn.shxzskj.cn

Go:   os.Getwd()
来源：http://fq.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://pp.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uq.huixiangedu.cn

[M05] 设置退出码
来源：http://wh.hnjuh.cn

Py:   sys.exit(1)
来源：http://zh.huixiangedu.cn

PHP:  exit(1);
来源：http://vm.lnxyls.cn

JS:   process.exit(1)
来源：http://yx.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://dw.shxzskj.cn

Java: System.exit(1)
来源：http://gk.newstarts.cn

Go:   os.Exit(1)
来源：http://rq.haigaiapp.cn

Ruby: exit 1
来源：http://lc.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ha.muxihuayi.cn

[M06] 向标准错误输出
来源：http://pr.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://uu.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ph.shxzskj.cn

JS:   console.error("err")
来源：http://ko.newstarts.cn

TS:   console.error("err")
来源：http://cp.newstarts.cn

Java: System.err.println("err")
来源：http://se.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wf.bjjhwx.cn

Ruby: warn "err"
来源：http://sa.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://be.asd995.cn

[M07] 判断是否为主入口
来源：http://et.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://av.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ae.bookmarksfly.cn

JS:   require.main === module
来源：http://oc.huanxung.cn

TS:   require.main === module
来源：http://ub.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://mn.9csxet.cn

Go:   func main()
来源：http://kz.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dt.hahajie.cn

C#:   static void Main(string[] args)
来源：http://xh.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://mn.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://mj.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://fj.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://vx.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://kl.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hf.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ab.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://er.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ro.newstarts.cn

================================================================================
来源：http://rk.huixinmuqiang.cn

N. 数据结构与算法
来源：http://id.lnxyls.cn

================================================================================
来源：http://rs.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://rb.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ok.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cs.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uw.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ax.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://lg.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iu.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ep.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://yv.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://by.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ve.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xd.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bn.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ey.nszjky.cn

Go:   slices.Sort(arr)
来源：http://ch.hnjuh.cn

Ruby: arr.sort
来源：http://jo.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ij.asd995.cn

[N03] 快速排序（分治示例）
来源：http://eb.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mc.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://iw.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ka.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ky.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ch.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xn.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vh.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zi.panjiajie.cn

[N04] 斐波那契数列
来源：http://li.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vb.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pw.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yd.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mn.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pp.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hv.bjjhwx.cn

[N05] 最大公约数
来源：http://qc.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://jf.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ix.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://he.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dv.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://re.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://ln.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qj.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://tj.newstarts.cn

Py:   s == s[::-1]
来源：http://ct.huanxung.cn

PHP:  $s === strrev($s);
来源：http://nx.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://si.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://pz.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kq.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ad.haigaiapp.cn

Ruby: s == s.reverse
来源：http://na.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ff.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://qc.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oz.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nw.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ug.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://om.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://ia.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://vg.lnxyls.cn

Ruby: // 手写 Hash
来源：http://ti.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://do.bookmarksfly.cn

[N08] 生成全排列
来源：http://hv.521024.cn

Py:   itertools.permutations(arr)
来源：http://vl.521024.cn

PHP:  // 手写递归交换
来源：http://bb.shxzukj.cn

JS:   // 手写回溯递归
来源：http://gv.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://qo.shtwfgs.cn

Java: // 手写回溯递归
来源：http://jh.panjiajie.cn

Go:   // 手写回溯递归
来源：http://at.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://bp.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://ce.wgjwhj.cn

[N09] 栈与队列
来源：http://de.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xq.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://to.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nd.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qo.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hm.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bv.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mv.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zv.newstarts.cn

[N10] 链表节点定义
来源：http://cq.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ro.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hb.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oq.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bv.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://iu.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hn.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ac.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ef.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://pj.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://er.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://lt.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aa.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://li.bjjhwx.cn

Java: // 手写递归
来源：http://aa.lnxyls.cn

Go:   // 手写递归
来源：http://vx.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lz.hahajie.cn

C#:   // 手写递归
来源：http://ot.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://su.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sx.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vb.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cf.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nn.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dw.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ut.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oo.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ux.asd995.cn

================================================================================
来源：http://up.jctech888.com.cn

O. 并发与异步
来源：http://kd.lnxyls.cn

================================================================================
来源：http://vz.haigaiapp.cn

[O01] 启动一个线程
来源：http://cs.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://er.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mm.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ej.huixinmuqiang.cn

TS:   // 同 JS
来源：http://xw.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://re.szxytkj.cn

Go:   go f()
来源：http://nn.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://lz.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://nc.shxzskj.cn

[O02] 使用线程池
来源：http://wc.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qm.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mx.521024.cn

JS:   // worker_threads 线程池
来源：http://hr.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://wh.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wb.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oo.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ld.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fc.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://hm.521024.cn

Py:   with lock: shared += 1
来源：http://pz.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://ac.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ef.yuntaijiaju.cn

TS:   // 同 JS
来源：http://gi.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://jl.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wd.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nv.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://go.hahajie.cn

[O04] 定义异步函数并等待
来源：http://jf.colortex.cn

Py:   async def f():⏎    await g()
来源：http://qg.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://te.asd995.cn

JS:   async function f() { await g(); }
来源：http://iz.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vc.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fo.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ew.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ea.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://ah.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://dq.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://cp.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yr.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://yx.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://wv.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://su.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yy.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ze.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pl.shxzskj.cn

[O06] 使用进程池
来源：http://is.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vn.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rh.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://pr.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://ep.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sf.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yh.9csxet.cn

Ruby: // fork 块
来源：http://yw.bookmarksfly.cn

C#:   Parallel.For
来源：http://yh.9csxet.cn

================================================================================
来源：http://jb.yuntaijiaju.cn

P. 常用工具函数
来源：http://rz.huixinmuqiang.cn

================================================================================
来源：http://lh.9csxet.cn

[P01] 生成 UUID
来源：http://pm.asd995.cn

Py:   str(uuid.uuid4())
来源：http://ut.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gw.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://ti.szsharing.cn

TS:   crypto.randomUUID()
来源：http://ki.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://jp.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://jw.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://vk.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xh.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://wj.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xz.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hl.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://au.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pc.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bv.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://be.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pt.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mx.asd995.cn

[P03] 生成短随机字符串
来源：http://ti.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vb.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gx.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vi.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://op.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hg.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cj.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zv.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jc.muxihuayi.cn

[P04] 求长度
来源：http://na.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jf.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wi.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xz.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xq.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ki.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://yy.nszjky.cn

Ruby: x.length;  x.size
来源：http://px.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qg.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ep.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ci.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jz.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rq.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tj.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oi.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ma.yuexingan06.cn

Ruby: a == b
来源：http://eg.521024.cn


<!-- 参考信息 -->