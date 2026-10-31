代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ec.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pe.wgjwhj.cn

================================================================================
来源：http://qr.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://xb.asd995.cn

================================================================================
来源：http://gr.shxzskj.cn

[M01] 读取命令行参数
来源：http://jr.gzmigu.cn

Py:   sys.argv[1:]
来源：http://wx.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://wc.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://qf.colortex.cn

TS:   process.argv.slice(2)
来源：http://ad.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://bu.521024.cn

Go:   os.Args[1:]
来源：http://wa.shxzukj.cn

Ruby: ARGV
来源：http://yq.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://jo.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://gt.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://no.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wt.panjiajie.cn

JS:   process.env.HOME
来源：http://fs.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://kz.hnjuh.cn

Java: System.getenv("HOME")
来源：http://nk.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hf.szsharing.cn

Ruby: ENV["HOME"]
来源：http://mq.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zi.gzmigu.cn

[M03] 执行外部命令
来源：http://om.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kw.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wp.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kd.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qj.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fe.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ux.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kr.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://ls.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://da.haigaiapp.cn

Py:   os.getcwd()
来源：http://ga.shxzskj.cn

PHP:  getcwd();
来源：http://pc.panjiajie.cn

JS:   process.cwd()
来源：http://ke.colortex.cn

TS:   process.cwd()
来源：http://fz.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://vp.bookmarksfly.cn

Go:   os.Getwd()
来源：http://aa.wgjwhj.cn

Ruby: Dir.pwd
来源：http://mz.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tj.jianghongdianzi.cn

[M05] 设置退出码
来源：http://mz.lnxyls.cn

Py:   sys.exit(1)
来源：http://hw.colortex.cn

PHP:  exit(1);
来源：http://lo.nszjky.cn

JS:   process.exit(1)
来源：http://zz.szxytkj.cn

TS:   process.exit(1)
来源：http://ag.gzmigu.cn

Java: System.exit(1)
来源：http://ma.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ab.9csxet.cn

Ruby: exit 1
来源：http://pe.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mx.nszjky.cn

[M06] 向标准错误输出
来源：http://vf.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://ik.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tt.jianghongdianzi.cn

JS:   console.error("err")
来源：http://fb.newstarts.cn

TS:   console.error("err")
来源：http://tq.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://oe.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uw.hahajie.cn

Ruby: warn "err"
来源：http://mp.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://yh.nszjky.cn

[M07] 判断是否为主入口
来源：http://mf.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://ja.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zz.nszjky.cn

JS:   require.main === module
来源：http://qu.wgjwhj.cn

TS:   require.main === module
来源：http://ih.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://yf.newstarts.cn

Go:   func main()
来源：http://ty.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nb.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://bo.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://pi.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://xa.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://fu.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://mi.colortex.cn

TS:   process.platform;  process.version
来源：http://zf.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vb.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bj.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ql.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xp.nicolike.cn

================================================================================
来源：http://mp.muxihuayi.cn

N. 数据结构与算法
来源：http://vp.nicolike.cn

================================================================================
来源：http://ib.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://wq.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lu.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dp.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dj.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oa.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://as.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://eh.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sp.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ub.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://db.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://co.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tf.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qd.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sg.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ti.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://qb.szxytkj.cn

Ruby: arr.sort
来源：http://hz.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kx.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://tc.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pg.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://hn.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sw.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xv.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kq.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://id.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wg.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xx.szxytkj.cn

[N04] 斐波那契数列
来源：http://no.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hl.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wv.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ju.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gz.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jf.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qh.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ga.gzmigu.cn

[N05] 最大公约数
来源：http://dr.9csxet.cn

Py:   math.gcd(a, b)
来源：http://yn.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nj.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tr.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bz.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xe.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://hr.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qw.wgjwhj.cn

[N06] 判断回文字符串
来源：http://wu.gzmigu.cn

Py:   s == s[::-1]
来源：http://bh.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://pk.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://ra.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://sw.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dk.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://cb.nszjky.cn

Ruby: s == s.reverse
来源：http://kp.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sj.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://ox.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cn.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iq.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qe.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ek.nicolike.cn

Java: // 手写 HashMap
来源：http://jn.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://nk.panjiajie.cn

Ruby: // 手写 Hash
来源：http://cd.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gl.jianghongdianzi.cn

[N08] 生成全排列
来源：http://gx.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://md.shxzukj.cn

PHP:  // 手写递归交换
来源：http://kd.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ax.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://do.shxzskj.cn

Java: // 手写回溯递归
来源：http://gw.lnxyls.cn

Go:   // 手写回溯递归
来源：http://rr.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://xt.colortex.cn

C#:   // 手写回溯递归
来源：http://jn.huanxung.cn

[N09] 栈与队列
来源：http://ff.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://st.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wc.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vz.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gj.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fn.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iw.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oy.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xi.9csxet.cn

[N10] 链表节点定义
来源：http://hz.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kp.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zt.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pi.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fd.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://wi.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tu.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wa.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fg.nicolike.cn

[N11] 二叉树中序遍历
来源：http://rs.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vs.newstarts.cn

PHP:  // 手写递归函数
来源：http://rt.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dx.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aw.chemitech.net.cn

Java: // 手写递归
来源：http://dx.yuexingan06.cn

Go:   // 手写递归
来源：http://tf.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xr.nicolike.cn

C#:   // 手写递归
来源：http://un.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ux.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yy.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sa.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dv.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qf.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ld.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ar.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://op.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cd.521024.cn

================================================================================
来源：http://yh.szsharing.cn

O. 并发与异步
来源：http://il.shtwfgs.cn

================================================================================
来源：http://rr.huixiangedu.cn

[O01] 启动一个线程
来源：http://ag.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fx.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sr.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uc.asd995.cn

TS:   // 同 JS
来源：http://tl.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://cd.wgjwhj.cn

Go:   go f()
来源：http://qd.panjiajie.cn

Ruby: Thread.new { f }
来源：http://un.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://wi.gzmigu.cn

[O02] 使用线程池
来源：http://uc.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bz.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rn.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://bf.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://ce.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ng.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jy.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zm.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hf.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://gd.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://mf.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://rb.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xp.colortex.cn

TS:   // 同 JS
来源：http://vy.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://fi.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cc.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ms.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://fr.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://pz.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://ny.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pj.newstarts.cn

JS:   async function f() { await g(); }
来源：http://dt.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xp.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://as.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ia.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ku.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://pm.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://wv.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://hw.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cm.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://ef.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://xt.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ls.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cm.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ml.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lq.521024.cn

[O06] 使用进程池
来源：http://ee.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cd.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xw.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://qy.colortex.cn

TS:   // child_process / cluster 模块
来源：http://aq.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xg.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qk.wgjwhj.cn

Ruby: // fork 块
来源：http://bx.asd995.cn

C#:   Parallel.For
来源：http://lo.lnxyls.cn

================================================================================
来源：http://el.muxihuayi.cn

P. 常用工具函数
来源：http://wi.yuexingan06.cn

================================================================================
来源：http://sx.shtwfgs.cn

[P01] 生成 UUID
来源：http://bs.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://eg.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gg.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://yv.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://sw.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://zl.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://ek.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://qr.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://kg.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://cu.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ev.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sp.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ef.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://du.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://td.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bp.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://we.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wd.lnxyls.cn

[P03] 生成短随机字符串
来源：http://us.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pg.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zl.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tg.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vg.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ru.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ct.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rx.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ar.hnjuh.cn

[P04] 求长度
来源：http://dr.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rb.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mi.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fa.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://ng.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://ks.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://na.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zv.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://mw.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iv.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hl.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ns.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://my.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wx.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ul.muxihuayi.cn

Ruby: a == b
来源：http://vk.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vp.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sv.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qp.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://qr.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vz.bjjhwx.cn

TS:   if (x == null) {}
来源：http://tm.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wy.9csxet.cn

Go:   if x == nil {}
来源：http://he.szxytkj.cn


<!-- 参考信息 -->