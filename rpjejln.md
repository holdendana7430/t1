代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sm.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sj.gzmigu.cn

================================================================================
来源：http://ar.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://au.hahajie.cn

================================================================================
来源：http://tj.nicolike.cn

[M01] 读取命令行参数
来源：http://my.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://cg.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://pe.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://cr.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://yg.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://hd.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://le.chemitech.net.cn

Ruby: ARGV
来源：http://gw.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://rw.nicolike.cn

[M02] 读取环境变量
来源：http://oc.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://ls.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qe.panjiajie.cn

JS:   process.env.HOME
来源：http://rk.bjjhwx.cn

TS:   process.env.HOME
来源：http://dt.521024.cn

Java: System.getenv("HOME")
来源：http://sl.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jd.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ki.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ik.huanxung.cn

[M03] 执行外部命令
来源：http://bs.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pp.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ul.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ci.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mw.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rx.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xo.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pd.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://bg.colortex.cn

[M04] 获取当前工作目录
来源：http://jp.chemitech.net.cn

Py:   os.getcwd()
来源：http://ag.hnjuh.cn

PHP:  getcwd();
来源：http://sw.asd995.cn

JS:   process.cwd()
来源：http://me.jianghongdianzi.cn

TS:   process.cwd()
来源：http://le.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://nf.hnjuh.cn

Go:   os.Getwd()
来源：http://pt.szxytkj.cn

Ruby: Dir.pwd
来源：http://zx.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://in.bjjhwx.cn

[M05] 设置退出码
来源：http://ut.hnjuh.cn

Py:   sys.exit(1)
来源：http://un.panjiajie.cn

PHP:  exit(1);
来源：http://dt.hahajie.cn

JS:   process.exit(1)
来源：http://du.haigaiapp.cn

TS:   process.exit(1)
来源：http://ul.lnxyls.cn

Java: System.exit(1)
来源：http://cf.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://fc.jianghongdianzi.cn

Ruby: exit 1
来源：http://uq.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qn.asd995.cn

[M06] 向标准错误输出
来源：http://yh.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://sc.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kg.521024.cn

JS:   console.error("err")
来源：http://ve.wgjwhj.cn

TS:   console.error("err")
来源：http://pm.gzmigu.cn

Java: System.err.println("err")
来源：http://es.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zk.yuexingan06.cn

Ruby: warn "err"
来源：http://si.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://tr.521024.cn

[M07] 判断是否为主入口
来源：http://uk.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://xw.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sn.panjiajie.cn

JS:   require.main === module
来源：http://gy.bookmarksfly.cn

TS:   require.main === module
来源：http://ti.asd995.cn

Java: public static void main(String[] args)
来源：http://mm.yuexingan06.cn

Go:   func main()
来源：http://ij.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lb.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://bv.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://sr.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://mx.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://oy.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://bp.szxytkj.cn

TS:   process.platform;  process.version
来源：http://ea.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cg.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dt.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gm.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://tr.9csxet.cn

N. 数据结构与算法
来源：http://fk.jianghongdianzi.cn

================================================================================
来源：http://wg.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://hk.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mq.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kw.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nn.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yk.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nv.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://qq.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qa.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uv.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://se.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://nv.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ix.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tv.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nm.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sm.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://bn.asd995.cn

Ruby: arr.sort
来源：http://vt.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rx.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://kn.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mc.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://lz.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ly.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uv.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://on.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gv.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oo.9csxet.cn

[N04] 斐波那契数列
来源：http://zr.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://je.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://et.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dd.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ys.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yu.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iu.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dv.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xe.asd995.cn

[N05] 最大公约数
来源：http://bc.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ks.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yt.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sd.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mc.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dt.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tt.nicolike.cn

Ruby: a.gcd(b)
来源：http://rd.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ey.gzmigu.cn

[N06] 判断回文字符串
来源：http://ck.shxzukj.cn

Py:   s == s[::-1]
来源：http://pe.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://dp.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://gg.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://cd.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://es.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://wa.shtwfgs.cn

Ruby: s == s.reverse
来源：http://kj.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dg.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://wt.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jm.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://am.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://en.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ad.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://cm.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://cv.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://av.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jm.huixiangedu.cn

[N08] 生成全排列
来源：http://bp.521024.cn

Py:   itertools.permutations(arr)
来源：http://ce.hahajie.cn

PHP:  // 手写递归交换
来源：http://cf.asd995.cn

JS:   // 手写回溯递归
来源：http://oi.shxzskj.cn

TS:   // 手写回溯递归
来源：http://yw.521024.cn

Java: // 手写回溯递归
来源：http://mn.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://cl.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://un.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://jp.nszjky.cn

[N09] 栈与队列
来源：http://yl.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jc.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hs.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yy.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://so.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tf.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://im.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://va.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.muxihuayi.cn

[N10] 链表节点定义
来源：http://bp.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sc.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nr.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://az.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://cn.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nw.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tl.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gp.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://vp.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cx.shxzskj.cn

PHP:  // 手写递归函数
来源：http://wj.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iy.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.chemitech.net.cn

Java: // 手写递归
来源：http://nu.panjiajie.cn

Go:   // 手写递归
来源：http://vq.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pf.9csxet.cn

C#:   // 手写递归
来源：http://ho.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dl.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ai.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jp.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yj.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aj.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rc.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fw.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.szsharing.cn

================================================================================
来源：http://vn.bookmarksfly.cn

O. 并发与异步
来源：http://oy.jctech888.com.cn

================================================================================
来源：http://iv.muxihuayi.cn

[O01] 启动一个线程
来源：http://oz.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nf.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xe.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tp.gzmigu.cn

TS:   // 同 JS
来源：http://hq.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://yt.jctech888.com.cn

Go:   go f()
来源：http://nr.szsharing.cn

Ruby: Thread.new { f }
来源：http://jz.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://hy.521024.cn

[O02] 使用线程池
来源：http://kt.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sr.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fz.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://ju.9csxet.cn

TS:   // worker_threads 线程池
来源：http://eh.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://my.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ad.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ys.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lm.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://pr.colortex.cn

Py:   with lock: shared += 1
来源：http://ed.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ke.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xp.szsharing.cn

TS:   // 同 JS
来源：http://av.521024.cn

Java: synchronized (this) { shared++; }
来源：http://du.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bn.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wg.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://jv.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://ev.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://sd.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ck.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://ye.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ww.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ir.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xl.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vs.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://nd.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://kh.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://vs.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gc.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://di.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://lu.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://en.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pk.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://va.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ip.jianghongdianzi.cn

[O06] 使用进程池
来源：http://jt.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ag.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kz.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://gn.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ld.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yn.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://of.chemitech.net.cn

Ruby: // fork 块
来源：http://cx.asd995.cn

C#:   Parallel.For
来源：http://ql.shxzukj.cn

================================================================================
来源：http://hv.asd995.cn

P. 常用工具函数
来源：http://ps.hnjuh.cn

================================================================================
来源：http://tp.nicolike.cn

[P01] 生成 UUID
来源：http://ge.colortex.cn

Py:   str(uuid.uuid4())
来源：http://rr.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fe.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://kd.nicolike.cn

TS:   crypto.randomUUID()
来源：http://ax.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://qy.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://sj.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://qg.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://mt.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://qn.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mo.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://er.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xo.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uw.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rl.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qh.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xr.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hn.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ib.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aa.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gs.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gr.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ol.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ob.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hi.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oc.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://so.shxzukj.cn

[P04] 求长度
来源：http://bg.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tx.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jb.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sr.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yv.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://jd.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://bx.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://ko.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rk.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://fm.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uc.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vi.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vf.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dy.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zm.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ht.haigaiapp.cn

Ruby: a == b
来源：http://cj.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rm.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qg.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qp.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://sh.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wo.wgjwhj.cn

TS:   if (x == null) {}
来源：http://pt.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kx.wgjwhj.cn

Go:   if x == nil {}
来源：http://pb.muxihuayi.cn


<!-- 参考信息 -->