代发 wailian999

================================================================================
来源：http://ma.shxzukj.cn

[M01] 读取命令行参数
来源：http://ut.hahajie.cn

Py:   sys.argv[1:]
来源：http://et.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://ro.asd995.cn

JS:   process.argv.slice(2)
来源：http://wf.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://oe.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://oe.shtwfgs.cn

Go:   os.Args[1:]
来源：http://mw.panjiajie.cn

Ruby: ARGV
来源：http://yz.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://ss.szxytkj.cn

[M02] 读取环境变量
来源：http://by.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://eu.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pz.shxzukj.cn

JS:   process.env.HOME
来源：http://pj.chemitech.net.cn

TS:   process.env.HOME
来源：http://xz.nicolike.cn

Java: System.getenv("HOME")
来源：http://ir.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pe.huanxung.cn

Ruby: ENV["HOME"]
来源：http://wx.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ro.hnjuh.cn

[M03] 执行外部命令
来源：http://zp.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kg.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rl.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ay.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xe.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ht.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bb.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://el.panjiajie.cn

[M04] 获取当前工作目录
来源：http://lr.hahajie.cn

Py:   os.getcwd()
来源：http://kg.shxzskj.cn

PHP:  getcwd();
来源：http://lh.shtwfgs.cn

JS:   process.cwd()
来源：http://ve.hahajie.cn

TS:   process.cwd()
来源：http://kx.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://uq.huanxung.cn

Go:   os.Getwd()
来源：http://xg.yuexingan06.cn

Ruby: Dir.pwd
来源：http://kb.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xz.huanxung.cn

[M05] 设置退出码
来源：http://ix.nicolike.cn

Py:   sys.exit(1)
来源：http://ys.szxytkj.cn

PHP:  exit(1);
来源：http://dz.lnxyls.cn

JS:   process.exit(1)
来源：http://zr.yuexingan06.cn

TS:   process.exit(1)
来源：http://fs.jianghongdianzi.cn

Java: System.exit(1)
来源：http://gd.huanxung.cn

Go:   os.Exit(1)
来源：http://tv.shxzukj.cn

Ruby: exit 1
来源：http://gh.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wa.wgjwhj.cn

[M06] 向标准错误输出
来源：http://ky.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ez.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xl.nicolike.cn

JS:   console.error("err")
来源：http://rd.huixiangedu.cn

TS:   console.error("err")
来源：http://zi.haigaiapp.cn

Java: System.err.println("err")
来源：http://os.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ae.chemitech.net.cn

Ruby: warn "err"
来源：http://gy.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://ch.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://kj.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://sy.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xb.newstarts.cn

JS:   require.main === module
来源：http://ly.hnjuh.cn

TS:   require.main === module
来源：http://gf.colortex.cn

Java: public static void main(String[] args)
来源：http://tj.asd995.cn

Go:   func main()
来源：http://wk.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nb.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://ju.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://nd.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://qp.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://oc.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://px.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://oy.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cb.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dd.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lv.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hc.huixiangedu.cn

================================================================================
来源：http://qe.nszjky.cn

N. 数据结构与算法
来源：http://oa.panjiajie.cn

================================================================================
来源：http://cq.521024.cn

[N01] 二分查找（有序数组）
来源：http://if.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qv.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sg.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fr.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kv.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://di.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://da.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ou.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kv.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://fv.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ry.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fn.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://di.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ew.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ny.colortex.cn

Go:   slices.Sort(arr)
来源：http://yp.521024.cn

Ruby: arr.sort
来源：http://ym.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ma.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://pa.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://id.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://kn.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xr.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ie.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sp.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uq.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ee.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bp.huanxung.cn

[N04] 斐波那契数列
来源：http://pw.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://np.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dl.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fc.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yz.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zp.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://px.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zf.szsharing.cn

[N05] 最大公约数
来源：http://rl.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://wy.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sp.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oy.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ew.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wb.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rh.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://zt.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dv.521024.cn

[N06] 判断回文字符串
来源：http://ut.gzmigu.cn

Py:   s == s[::-1]
来源：http://uk.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://xx.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ix.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ak.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ql.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://uo.lnxyls.cn

Ruby: s == s.reverse
来源：http://np.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://or.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://jw.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vj.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fj.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://aa.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://ab.colortex.cn

Java: // 手写 HashMap
来源：http://rg.9csxet.cn

Go:   // 手写 map[int]int
来源：http://nt.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://kt.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gy.huixinmuqiang.cn

[N08] 生成全排列
来源：http://lp.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://vj.lnxyls.cn

PHP:  // 手写递归交换
来源：http://bn.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://sz.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://ow.hahajie.cn

Java: // 手写回溯递归
来源：http://ys.gzmigu.cn

Go:   // 手写回溯递归
来源：http://qm.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://gj.panjiajie.cn

C#:   // 手写回溯递归
来源：http://kq.huixiangedu.cn

[N09] 栈与队列
来源：http://ym.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xp.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hi.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xb.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zg.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wd.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://do.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ka.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rg.colortex.cn

[N10] 链表节点定义
来源：http://ze.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pg.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wn.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kv.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ic.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://mv.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://do.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dd.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cx.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://dq.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nx.panjiajie.cn

PHP:  // 手写递归函数
来源：http://yz.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://km.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vt.chemitech.net.cn

Java: // 手写递归
来源：http://bx.hnjuh.cn

Go:   // 手写递归
来源：http://ap.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pn.panjiajie.cn

C#:   // 手写递归
来源：http://md.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ub.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iq.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://te.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yc.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hi.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mq.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://om.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gx.wgjwhj.cn

================================================================================
来源：http://sn.hnjuh.cn

O. 并发与异步
来源：http://jv.shxzskj.cn

================================================================================
来源：http://mj.shxzskj.cn

[O01] 启动一个线程
来源：http://dx.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qo.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aa.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://es.shxzskj.cn

TS:   // 同 JS
来源：http://av.521024.cn

Java: new Thread(() -> f()).start()
来源：http://lr.chemitech.net.cn

Go:   go f()
来源：http://lv.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://pb.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://pr.gzmigu.cn

[O02] 使用线程池
来源：http://ms.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mx.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://is.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://ex.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://dc.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ig.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://af.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lq.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://me.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://dq.newstarts.cn

Py:   with lock: shared += 1
来源：http://tq.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://jx.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gg.muxihuayi.cn

TS:   // 同 JS
来源：http://xc.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://do.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nr.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qv.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://py.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://pv.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://eu.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ea.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://rc.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zy.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://md.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iz.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iy.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://lr.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://xm.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://wu.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://on.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://py.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://yb.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://me.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://um.9csxet.cn

Ruby: threads.map(&:join)
来源：http://hc.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hd.bookmarksfly.cn

[O06] 使用进程池
来源：http://dc.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kg.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rd.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://pc.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://vv.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ka.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pp.szsharing.cn

Ruby: // fork 块
来源：http://ub.colortex.cn

C#:   Parallel.For
来源：http://yc.521024.cn

================================================================================
来源：http://dn.wgjwhj.cn

P. 常用工具函数
来源：http://zg.jianghongdianzi.cn

================================================================================
来源：http://ea.shtwfgs.cn

[P01] 生成 UUID
来源：http://vt.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://lm.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qb.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://ly.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://md.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://wx.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://lq.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://jy.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://ry.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://yg.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nd.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ha.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bg.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bw.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rn.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zz.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nm.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dd.521024.cn

[P03] 生成短随机字符串
来源：http://ak.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ey.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xu.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rt.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wa.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sf.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://us.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://en.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yx.wgjwhj.cn

[P04] 求长度
来源：http://qd.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ik.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eb.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ye.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ru.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://ga.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://qr.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://tq.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nc.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://gc.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wd.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pr.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vd.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bf.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ia.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ld.nszjky.cn

Ruby: a == b
来源：http://pk.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mq.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gd.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sn.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://mv.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pj.bjjhwx.cn

TS:   if (x == null) {}
来源：http://po.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dm.chemitech.net.cn

Go:   if x == nil {}
来源：http://hl.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tf.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://kw.bjjhwx.cn

[P07] 防抖与节流
来源：http://yc.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ej.shxzukj.cn


<!-- 参考信息 -->