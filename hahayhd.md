代发 wailian999

================================================================================
来源：http://ye.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://gm.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ai.9csxet.cn

PHP:  $argv;  $argc;
来源：http://ps.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://od.colortex.cn

TS:   process.argv.slice(2)
来源：http://sq.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://wd.huixiangedu.cn

Go:   os.Args[1:]
来源：http://cz.haigaiapp.cn

Ruby: ARGV
来源：http://tt.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://mr.9csxet.cn

[M02] 读取环境变量
来源：http://zq.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://pj.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ej.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://nm.hnjuh.cn

TS:   process.env.HOME
来源：http://ji.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://yt.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nj.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://xu.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vm.bjjhwx.cn

[M03] 执行外部命令
来源：http://je.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ne.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bp.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ct.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rx.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hw.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rv.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://me.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://vd.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://fs.bjjhwx.cn

Py:   os.getcwd()
来源：http://cd.521024.cn

PHP:  getcwd();
来源：http://kn.panjiajie.cn

JS:   process.cwd()
来源：http://ni.panjiajie.cn

TS:   process.cwd()
来源：http://ex.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ah.yuexingan06.cn

Go:   os.Getwd()
来源：http://jn.hnjuh.cn

Ruby: Dir.pwd
来源：http://vl.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zk.asd995.cn

[M05] 设置退出码
来源：http://je.wgjwhj.cn

Py:   sys.exit(1)
来源：http://xr.jianghongdianzi.cn

PHP:  exit(1);
来源：http://hy.nszjky.cn

JS:   process.exit(1)
来源：http://eg.szsharing.cn

TS:   process.exit(1)
来源：http://ey.szxytkj.cn

Java: System.exit(1)
来源：http://iq.shxzskj.cn

Go:   os.Exit(1)
来源：http://fh.nszjky.cn

Ruby: exit 1
来源：http://lx.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rf.asd995.cn

[M06] 向标准错误输出
来源：http://is.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://lx.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bo.huixiangedu.cn

JS:   console.error("err")
来源：http://ra.huixinmuqiang.cn

TS:   console.error("err")
来源：http://kf.jctech888.com.cn

Java: System.err.println("err")
来源：http://rw.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ih.yuexingan06.cn

Ruby: warn "err"
来源：http://fk.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://nl.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://qq.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://tv.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mo.huixiangedu.cn

JS:   require.main === module
来源：http://jl.szsharing.cn

TS:   require.main === module
来源：http://jo.newstarts.cn

Java: public static void main(String[] args)
来源：http://sz.gzmigu.cn

Go:   func main()
来源：http://qq.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ca.newstarts.cn

C#:   static void Main(string[] args)
来源：http://wa.colortex.cn

[M08] 获取系统与运行时信息
来源：http://tj.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://sm.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ug.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://cu.lnxyls.cn

TS:   process.platform;  process.version
来源：http://eb.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oa.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kc.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ue.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cr.muxihuayi.cn

================================================================================
来源：http://xm.haigaiapp.cn

N. 数据结构与算法
来源：http://hz.521024.cn

================================================================================
来源：http://ib.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://yy.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vq.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qt.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sj.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cl.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mi.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://wv.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cp.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dk.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://mm.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ck.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ev.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xp.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tw.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ev.colortex.cn

Go:   slices.Sort(arr)
来源：http://gw.jctech888.com.cn

Ruby: arr.sort
来源：http://xg.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fu.colortex.cn

[N03] 快速排序（分治示例）
来源：http://zf.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ve.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://pz.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hd.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hd.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dz.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oy.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rl.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fs.chemitech.net.cn

[N04] 斐波那契数列
来源：http://zh.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rw.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wt.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ee.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://si.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zk.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ja.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xi.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rd.lnxyls.cn

[N05] 最大公约数
来源：http://dr.521024.cn

Py:   math.gcd(a, b)
来源：http://dp.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gp.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hl.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ce.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fx.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ft.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://uh.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lg.newstarts.cn

[N06] 判断回文字符串
来源：http://yz.hnjuh.cn

Py:   s == s[::-1]
来源：http://ro.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://bk.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://jb.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://pn.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fk.nszjky.cn

Go:   // 双指针从两端比较
来源：http://aj.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://uj.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ck.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://df.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wn.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oh.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zj.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://rf.wgjwhj.cn

Java: // 手写 HashMap
来源：http://sv.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://mr.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://nq.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eq.huanxung.cn

[N08] 生成全排列
来源：http://ob.colortex.cn

Py:   itertools.permutations(arr)
来源：http://qz.shxzskj.cn

PHP:  // 手写递归交换
来源：http://wc.szxytkj.cn

JS:   // 手写回溯递归
来源：http://lr.521024.cn

TS:   // 手写回溯递归
来源：http://xr.lnxyls.cn

Java: // 手写回溯递归
来源：http://ew.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://dp.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://tg.shxzskj.cn

C#:   // 手写回溯递归
来源：http://br.shtwfgs.cn

[N09] 栈与队列
来源：http://vr.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aw.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ow.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jh.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xv.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hm.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mj.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oe.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qf.9csxet.cn

[N10] 链表节点定义
来源：http://pn.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eu.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tq.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bm.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yi.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://qt.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cp.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hi.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rt.hahajie.cn

[N11] 二叉树中序遍历
来源：http://ix.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://af.gzmigu.cn

PHP:  // 手写递归函数
来源：http://xh.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zu.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dg.lnxyls.cn

Java: // 手写递归
来源：http://zp.hahajie.cn

Go:   // 手写递归
来源：http://bl.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mj.jctech888.com.cn

C#:   // 手写递归
来源：http://zm.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mn.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uq.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wm.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sk.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://im.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ys.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fw.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mc.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://no.lnxyls.cn

================================================================================
来源：http://fn.9csxet.cn

O. 并发与异步
来源：http://fz.bjjhwx.cn

================================================================================
来源：http://ex.colortex.cn

[O01] 启动一个线程
来源：http://gb.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pd.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wc.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mv.asd995.cn

TS:   // 同 JS
来源：http://sc.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://zx.bookmarksfly.cn

Go:   go f()
来源：http://az.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://yz.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://rc.yuexingan06.cn

[O02] 使用线程池
来源：http://nk.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nn.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mr.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://qj.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://hu.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fq.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wu.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fh.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ol.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://at.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://mo.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://bc.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iy.chemitech.net.cn

TS:   // 同 JS
来源：http://nw.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://py.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pc.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ai.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://jo.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://sb.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ks.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ei.hahajie.cn

JS:   async function f() { await g(); }
来源：http://ne.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pr.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fg.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ld.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mr.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://bo.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://ms.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://yq.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zb.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://wu.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://ye.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://il.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pu.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://yz.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sf.newstarts.cn

[O06] 使用进程池
来源：http://yv.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ug.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://co.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://la.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://br.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nc.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mv.jianghongdianzi.cn

Ruby: // fork 块
来源：http://cq.bookmarksfly.cn

C#:   Parallel.For
来源：http://gu.jianghongdianzi.cn

================================================================================
来源：http://wi.szxytkj.cn

P. 常用工具函数
来源：http://dg.yuexingan06.cn

================================================================================
来源：http://ah.asd995.cn

[P01] 生成 UUID
来源：http://ul.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://xm.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kw.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://pf.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://pt.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://bm.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://zq.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://sx.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://qk.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://wh.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kl.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hu.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cl.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qp.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qh.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rq.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ar.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hs.shxzskj.cn

[P03] 生成短随机字符串
来源：http://kt.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wn.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ij.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gm.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lc.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pn.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pb.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fz.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ll.lnxyls.cn

[P04] 求长度
来源：http://ao.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mc.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jh.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xw.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://og.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ef.szsharing.cn

Go:   len(arr);  len(m)
来源：http://kc.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ba.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xs.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ox.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://he.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://if.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xi.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ln.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kq.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://an.bjjhwx.cn

Ruby: a == b
来源：http://ds.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xj.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wd.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://li.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sf.huanxung.cn

TS:   if (x == null) {}
来源：http://eq.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lq.huanxung.cn

Go:   if x == nil {}
来源：http://ly.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fo.521024.cn

C#:   if (x is null) {}
来源：http://yz.hahajie.cn

[P07] 防抖与节流
来源：http://zp.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fm.521024.cn


<!-- 参考信息 -->