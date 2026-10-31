代发 wailian999

================================================================================
来源：http://sn.panjiajie.cn

[M01] 读取命令行参数
来源：http://eo.9csxet.cn

Py:   sys.argv[1:]
来源：http://ba.newstarts.cn

PHP:  $argv;  $argc;
来源：http://jt.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://pl.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://yt.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://nq.hahajie.cn

Go:   os.Args[1:]
来源：http://kf.shxzskj.cn

Ruby: ARGV
来源：http://xj.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://gr.yuexingan06.cn

[M02] 读取环境变量
来源：http://pn.521024.cn

Py:   os.environ.get("HOME")
来源：http://wj.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gl.colortex.cn

JS:   process.env.HOME
来源：http://dv.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://fy.shxzskj.cn

Java: System.getenv("HOME")
来源：http://cm.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gp.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://qq.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://so.haigaiapp.cn

[M03] 执行外部命令
来源：http://lx.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ah.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ja.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hv.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dp.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wp.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sj.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nk.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://tq.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://vr.muxihuayi.cn

Py:   os.getcwd()
来源：http://kq.nicolike.cn

PHP:  getcwd();
来源：http://nc.hahajie.cn

JS:   process.cwd()
来源：http://fz.szxytkj.cn

TS:   process.cwd()
来源：http://xm.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://tp.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://gf.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://dg.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ab.bjjhwx.cn

[M05] 设置退出码
来源：http://vd.nszjky.cn

Py:   sys.exit(1)
来源：http://fg.nszjky.cn

PHP:  exit(1);
来源：http://gp.hahajie.cn

JS:   process.exit(1)
来源：http://js.shtwfgs.cn

TS:   process.exit(1)
来源：http://gh.bjjhwx.cn

Java: System.exit(1)
来源：http://yw.shxzskj.cn

Go:   os.Exit(1)
来源：http://fn.szxytkj.cn

Ruby: exit 1
来源：http://sh.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://es.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ef.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://tb.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hi.yuexingan06.cn

JS:   console.error("err")
来源：http://ii.huixiangedu.cn

TS:   console.error("err")
来源：http://md.huanxung.cn

Java: System.err.println("err")
来源：http://aw.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kh.bjjhwx.cn

Ruby: warn "err"
来源：http://rl.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ka.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://bo.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://fl.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cf.bookmarksfly.cn

JS:   require.main === module
来源：http://yc.shxzukj.cn

TS:   require.main === module
来源：http://tc.hahajie.cn

Java: public static void main(String[] args)
来源：http://za.bjjhwx.cn

Go:   func main()
来源：http://su.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mo.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://vz.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://sq.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://lh.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://nx.szsharing.cn

TS:   process.platform;  process.version
来源：http://am.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ec.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lr.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gp.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aa.shtwfgs.cn

================================================================================
来源：http://kq.yuexingan06.cn

N. 数据结构与算法
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://ze.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://nn.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hp.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yh.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vy.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jp.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://we.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ex.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cc.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://li.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ad.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uh.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ji.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gu.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ey.newstarts.cn

Go:   slices.Sort(arr)
来源：http://cz.hnjuh.cn

Ruby: arr.sort
来源：http://wu.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vc.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ke.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qp.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://xv.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ri.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lz.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ds.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://py.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zq.9csxet.cn

[N04] 斐波那契数列
来源：http://mh.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wm.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xk.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ku.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://or.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mc.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kr.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jw.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ay.gzmigu.cn

[N05] 最大公约数
来源：http://oc.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://lk.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eu.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wt.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://si.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iu.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://if.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xi.nicolike.cn

[N06] 判断回文字符串
来源：http://wb.bjjhwx.cn

Py:   s == s[::-1]
来源：http://pg.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://if.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://js.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://ag.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ee.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://jp.jctech888.com.cn

Ruby: s == s.reverse
来源：http://ig.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uh.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://kg.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ez.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jf.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yy.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://gn.521024.cn

Java: // 手写 HashMap
来源：http://ge.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://wk.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ws.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://km.newstarts.cn

[N08] 生成全排列
来源：http://wf.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://nx.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://pv.asd995.cn

JS:   // 手写回溯递归
来源：http://an.shxzskj.cn

TS:   // 手写回溯递归
来源：http://nj.szxytkj.cn

Java: // 手写回溯递归
来源：http://gg.colortex.cn

Go:   // 手写回溯递归
来源：http://ld.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://hy.hahajie.cn

C#:   // 手写回溯递归
来源：http://dv.huixiangedu.cn

[N09] 栈与队列
来源：http://jq.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gg.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ab.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vv.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gx.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://em.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nt.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yu.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://of.szxytkj.cn

[N10] 链表节点定义
来源：http://mv.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iy.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ey.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://in.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tl.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://yo.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rp.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ca.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ab.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://ns.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wi.hahajie.cn

PHP:  // 手写递归函数
来源：http://oh.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qv.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kr.gzmigu.cn

Java: // 手写递归
来源：http://pp.shtwfgs.cn

Go:   // 手写递归
来源：http://qn.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vc.haigaiapp.cn

C#:   // 手写递归
来源：http://an.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gp.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sq.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pa.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lz.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fy.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mt.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ft.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://is.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://so.9csxet.cn

================================================================================
来源：http://yr.bookmarksfly.cn

O. 并发与异步
来源：http://gy.colortex.cn

================================================================================
来源：http://wb.haigaiapp.cn

[O01] 启动一个线程
来源：http://cu.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wx.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hi.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://io.haigaiapp.cn

TS:   // 同 JS
来源：http://kc.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://nb.9csxet.cn

Go:   go f()
来源：http://la.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://qk.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://by.yuexingan06.cn

[O02] 使用线程池
来源：http://wc.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://la.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ac.szsharing.cn

JS:   // worker_threads 线程池
来源：http://bm.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://ud.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ef.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nm.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wp.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ac.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://cm.panjiajie.cn

Py:   with lock: shared += 1
来源：http://aq.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://hm.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ef.521024.cn

TS:   // 同 JS
来源：http://kv.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://fh.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lm.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jl.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://mx.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://wb.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://cb.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oz.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://te.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qe.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bw.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eu.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uv.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://hk.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://en.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://zs.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dm.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://oc.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://yl.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bp.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eu.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ey.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hg.lnxyls.cn

[O06] 使用进程池
来源：http://jc.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mg.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hr.asd995.cn

JS:   // child_process / cluster 模块
来源：http://bn.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://dk.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nj.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yo.szxytkj.cn

Ruby: // fork 块
来源：http://tf.szsharing.cn

C#:   Parallel.For
来源：http://lg.huanxung.cn

================================================================================
来源：http://nw.panjiajie.cn

P. 常用工具函数
来源：http://oo.jctech888.com.cn

================================================================================
来源：http://dp.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://kn.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://oa.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dp.hahajie.cn

JS:   crypto.randomUUID()
来源：http://qi.szsharing.cn

TS:   crypto.randomUUID()
来源：http://tw.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://vx.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://ee.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://jv.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://aj.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ci.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vt.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qt.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dr.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nv.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wy.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vg.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rh.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ii.panjiajie.cn

[P03] 生成短随机字符串
来源：http://bn.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bp.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ba.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ra.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ik.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://so.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sc.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ff.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iz.bookmarksfly.cn

[P04] 求长度
来源：http://if.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yh.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jb.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gm.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pi.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://fe.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://vo.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://us.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xs.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://av.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ap.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ov.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zc.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mi.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kj.shxzskj.cn

Ruby: a == b
来源：http://za.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gc.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rx.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xe.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://zq.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qs.gzmigu.cn

TS:   if (x == null) {}
来源：http://it.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yo.asd995.cn

Go:   if x == nil {}
来源：http://lo.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rl.521024.cn

C#:   if (x is null) {}
来源：http://jf.shxzukj.cn

[P07] 防抖与节流
来源：http://vz.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wu.huanxung.cn


<!-- 参考信息 -->