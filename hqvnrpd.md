代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ta.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mk.521024.cn

================================================================================
来源：http://qg.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://ts.bookmarksfly.cn

================================================================================
来源：http://ax.yuexingan06.cn

[M01] 读取命令行参数
来源：http://ik.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ks.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://jd.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://fy.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://nr.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://xq.colortex.cn

Go:   os.Args[1:]
来源：http://ix.szxytkj.cn

Ruby: ARGV
来源：http://xa.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://xv.bjjhwx.cn

[M02] 读取环境变量
来源：http://sf.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://ov.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mj.colortex.cn

JS:   process.env.HOME
来源：http://kt.szxytkj.cn

TS:   process.env.HOME
来源：http://dq.huanxung.cn

Java: System.getenv("HOME")
来源：http://rn.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sh.colortex.cn

Ruby: ENV["HOME"]
来源：http://ng.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ao.muxihuayi.cn

[M03] 执行外部命令
来源：http://xn.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qi.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ho.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ss.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uv.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pa.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ry.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iz.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://xk.newstarts.cn

[M04] 获取当前工作目录
来源：http://gt.yuexingan06.cn

Py:   os.getcwd()
来源：http://uk.newstarts.cn

PHP:  getcwd();
来源：http://xd.haigaiapp.cn

JS:   process.cwd()
来源：http://ge.newstarts.cn

TS:   process.cwd()
来源：http://ul.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://oh.521024.cn

Go:   os.Getwd()
来源：http://dz.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://mp.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kg.bjjhwx.cn

[M05] 设置退出码
来源：http://dp.shxzukj.cn

Py:   sys.exit(1)
来源：http://az.haigaiapp.cn

PHP:  exit(1);
来源：http://fh.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://bm.521024.cn

TS:   process.exit(1)
来源：http://fv.yuexingan06.cn

Java: System.exit(1)
来源：http://mw.colortex.cn

Go:   os.Exit(1)
来源：http://ru.shxzukj.cn

Ruby: exit 1
来源：http://sr.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ka.9csxet.cn

[M06] 向标准错误输出
来源：http://gw.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://fc.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cc.jianghongdianzi.cn

JS:   console.error("err")
来源：http://hp.muxihuayi.cn

TS:   console.error("err")
来源：http://ij.521024.cn

Java: System.err.println("err")
来源：http://qj.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dj.bjjhwx.cn

Ruby: warn "err"
来源：http://bh.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ft.9csxet.cn

[M07] 判断是否为主入口
来源：http://tv.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://hz.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dh.szxytkj.cn

JS:   require.main === module
来源：http://zi.521024.cn

TS:   require.main === module
来源：http://vy.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://mq.hahajie.cn

Go:   func main()
来源：http://lk.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ai.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ps.colortex.cn

[M08] 获取系统与运行时信息
来源：http://us.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://ro.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://tk.hahajie.cn

JS:   process.platform;  process.version
来源：http://vz.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://ie.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wv.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cf.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nw.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jq.chemitech.net.cn

================================================================================
来源：http://rm.lnxyls.cn

N. 数据结构与算法
来源：http://ul.haigaiapp.cn

================================================================================
来源：http://vm.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://wi.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://no.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mc.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bv.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sa.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wx.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://yd.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://en.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ec.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://os.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yw.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ex.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lo.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hm.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://so.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://jg.huixiangedu.cn

Ruby: arr.sort
来源：http://oc.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tl.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://fv.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ls.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://de.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zo.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mf.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sl.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xu.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oe.jctech888.com.cn

[N04] 斐波那契数列
来源：http://jo.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sx.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zo.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ke.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qg.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uy.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rv.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gi.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oy.huixinmuqiang.cn

[N05] 最大公约数
来源：http://vk.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://tk.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dv.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://av.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fo.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nq.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://io.colortex.cn

Ruby: a.gcd(b)
来源：http://ov.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://as.chemitech.net.cn

[N06] 判断回文字符串
来源：http://yw.521024.cn

Py:   s == s[::-1]
来源：http://ta.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://zx.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://pq.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://sx.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yh.szsharing.cn

Go:   // 双指针从两端比较
来源：http://pr.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ws.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gq.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://hc.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://er.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xb.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kk.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://ya.jctech888.com.cn

Java: // 手写 HashMap
来源：http://cx.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://lh.hahajie.cn

Ruby: // 手写 Hash
来源：http://id.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xk.bjjhwx.cn

[N08] 生成全排列
来源：http://lw.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://pj.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ad.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ep.asd995.cn

TS:   // 手写回溯递归
来源：http://fh.yuexingan06.cn

Java: // 手写回溯递归
来源：http://yl.panjiajie.cn

Go:   // 手写回溯递归
来源：http://xj.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://mz.shxzskj.cn

C#:   // 手写回溯递归
来源：http://yf.szsharing.cn

[N09] 栈与队列
来源：http://vk.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rw.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wx.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cp.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rt.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wv.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fx.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qw.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ca.haigaiapp.cn

[N10] 链表节点定义
来源：http://vx.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tv.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ip.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lk.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hm.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://pe.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://je.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://me.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mz.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://tm.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mw.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ag.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dv.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bv.szsharing.cn

Java: // 手写递归
来源：http://mu.nszjky.cn

Go:   // 手写递归
来源：http://bp.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pa.hahajie.cn

C#:   // 手写递归
来源：http://cz.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ev.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kb.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fv.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://im.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ry.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://de.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eg.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ra.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yj.jctech888.com.cn

================================================================================
来源：http://js.yuntaijiaju.cn

O. 并发与异步
来源：http://wx.szsharing.cn

================================================================================
来源：http://vr.nszjky.cn

[O01] 启动一个线程
来源：http://kk.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xl.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lu.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rj.gzmigu.cn

TS:   // 同 JS
来源：http://sx.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://xy.szxytkj.cn

Go:   go f()
来源：http://ut.panjiajie.cn

Ruby: Thread.new { f }
来源：http://wp.asd995.cn

C#:   Task.Run(() => F());
来源：http://hl.newstarts.cn

[O02] 使用线程池
来源：http://ox.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://md.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jb.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://hd.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://sp.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ta.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://of.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://be.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bi.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ry.nszjky.cn

Py:   with lock: shared += 1
来源：http://pg.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://el.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mc.shxzskj.cn

TS:   // 同 JS
来源：http://ky.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://vw.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vz.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ux.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://cy.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://oy.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://gr.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yg.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://fh.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tb.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dc.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nq.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lg.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://ek.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://bp.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://me.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mn.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://rv.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://mv.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ms.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qb.hahajie.cn

Ruby: threads.map(&:join)
来源：http://zf.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bx.jianghongdianzi.cn

[O06] 使用进程池
来源：http://mr.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rc.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pm.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://sc.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://rj.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ai.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jr.nicolike.cn

Ruby: // fork 块
来源：http://ph.521024.cn

C#:   Parallel.For
来源：http://yp.newstarts.cn

================================================================================
来源：http://yr.bjjhwx.cn

P. 常用工具函数
来源：http://wh.gzmigu.cn

================================================================================
来源：http://bx.newstarts.cn

[P01] 生成 UUID
来源：http://qa.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://oj.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hr.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://di.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://pa.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://re.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://oz.521024.cn

Ruby: SecureRandom.uuid
来源：http://kk.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://dt.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://bi.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gk.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cp.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tk.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yw.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://py.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dy.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fu.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kc.hahajie.cn

[P03] 生成短随机字符串
来源：http://lo.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pu.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pe.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mq.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uf.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wq.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jr.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wo.newstarts.cn

[P04] 求长度
来源：http://fa.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zc.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kt.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vt.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uc.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://fs.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://sy.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://cj.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hh.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://ou.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ny.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hj.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tg.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://di.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hj.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hl.nicolike.cn

Ruby: a == b
来源：http://rt.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cz.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://do.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kr.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://id.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xm.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://yf.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qv.shxzukj.cn

Go:   if x == nil {}
来源：http://gs.szxytkj.cn


<!-- 参考信息 -->