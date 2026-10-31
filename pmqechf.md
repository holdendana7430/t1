代发 wailian999

================================================================================
来源：http://tb.wgjwhj.cn

[M01] 读取命令行参数
来源：http://xo.lnxyls.cn

Py:   sys.argv[1:]
来源：http://bf.colortex.cn

PHP:  $argv;  $argc;
来源：http://gd.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://dr.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://ti.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://jy.huixiangedu.cn

Go:   os.Args[1:]
来源：http://hc.newstarts.cn

Ruby: ARGV
来源：http://de.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://xa.nicolike.cn

[M02] 读取环境变量
来源：http://yz.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://sb.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mf.yuexingan06.cn

JS:   process.env.HOME
来源：http://yl.nicolike.cn

TS:   process.env.HOME
来源：http://oi.szsharing.cn

Java: System.getenv("HOME")
来源：http://or.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oz.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ob.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vo.muxihuayi.cn

[M03] 执行外部命令
来源：http://rx.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pu.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ag.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wq.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://th.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cw.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jm.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://mt.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ed.wgjwhj.cn

Py:   os.getcwd()
来源：http://pl.yuexingan06.cn

PHP:  getcwd();
来源：http://lt.jctech888.com.cn

JS:   process.cwd()
来源：http://cs.shxzukj.cn

TS:   process.cwd()
来源：http://vr.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bg.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://gd.huanxung.cn

Ruby: Dir.pwd
来源：http://vx.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aa.hnjuh.cn

[M05] 设置退出码
来源：http://jn.chemitech.net.cn

Py:   sys.exit(1)
来源：http://hb.yuexingan06.cn

PHP:  exit(1);
来源：http://hs.panjiajie.cn

JS:   process.exit(1)
来源：http://at.hnjuh.cn

TS:   process.exit(1)
来源：http://ui.521024.cn

Java: System.exit(1)
来源：http://eq.colortex.cn

Go:   os.Exit(1)
来源：http://wl.asd995.cn

Ruby: exit 1
来源：http://or.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qj.lnxyls.cn

[M06] 向标准错误输出
来源：http://pr.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zc.yuexingan06.cn

JS:   console.error("err")
来源：http://zh.huanxung.cn

TS:   console.error("err")
来源：http://qc.bjjhwx.cn

Java: System.err.println("err")
来源：http://nh.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sm.szxytkj.cn

Ruby: warn "err"
来源：http://ga.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://lz.gzmigu.cn

[M07] 判断是否为主入口
来源：http://bm.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://bz.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://il.yuexingan06.cn

JS:   require.main === module
来源：http://lj.521024.cn

TS:   require.main === module
来源：http://jd.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://rk.newstarts.cn

Go:   func main()
来源：http://tm.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hv.nicolike.cn

C#:   static void Main(string[] args)
来源：http://da.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://tu.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://ua.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xi.shxzskj.cn

JS:   process.platform;  process.version
来源：http://pv.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://px.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wt.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qw.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xp.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jb.yuntaijiaju.cn

================================================================================
来源：http://iv.asd995.cn

N. 数据结构与算法
来源：http://vi.huixinmuqiang.cn

================================================================================
来源：http://jp.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://lx.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vn.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sc.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jz.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fk.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zy.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://ku.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ul.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wf.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://wl.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://cv.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kk.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fe.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ht.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yv.newstarts.cn

Go:   slices.Sort(arr)
来源：http://xz.szsharing.cn

Ruby: arr.sort
来源：http://qj.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://na.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://nr.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ec.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://xr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oc.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bl.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cf.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qh.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fj.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ty.newstarts.cn

[N04] 斐波那契数列
来源：http://on.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mp.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uw.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uv.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iu.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ss.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://so.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://be.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gv.muxihuayi.cn

[N05] 最大公约数
来源：http://vr.asd995.cn

Py:   math.gcd(a, b)
来源：http://ya.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uq.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cb.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cp.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bn.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vj.panjiajie.cn

Ruby: a.gcd(b)
来源：http://kd.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ss.szsharing.cn

[N06] 判断回文字符串
来源：http://bn.shtwfgs.cn

Py:   s == s[::-1]
来源：http://uu.nszjky.cn

PHP:  $s === strrev($s);
来源：http://eo.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://qi.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://ul.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yf.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://ht.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ce.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ii.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://wg.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ai.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lf.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ma.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://th.521024.cn

Java: // 手写 HashMap
来源：http://rw.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ik.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://fe.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ee.hnjuh.cn

[N08] 生成全排列
来源：http://cq.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://xi.521024.cn

PHP:  // 手写递归交换
来源：http://qa.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://gh.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ct.muxihuayi.cn

Java: // 手写回溯递归
来源：http://jh.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://ev.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://bl.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://gj.9csxet.cn

[N09] 栈与队列
来源：http://pt.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aa.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ta.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vo.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lh.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://um.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nh.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fc.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dc.gzmigu.cn

[N10] 链表节点定义
来源：http://op.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sn.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yf.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eu.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ur.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://nn.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fo.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hf.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wr.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://xc.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rw.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://mu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rx.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bu.shxzskj.cn

Java: // 手写递归
来源：http://eh.szsharing.cn

Go:   // 手写递归
来源：http://nv.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vl.jctech888.com.cn

C#:   // 手写递归
来源：http://mt.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kd.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zc.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xf.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vv.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ao.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ts.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gd.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uz.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ud.szsharing.cn

================================================================================
来源：http://hk.muxihuayi.cn

O. 并发与异步
来源：http://ii.hnjuh.cn

================================================================================
来源：http://mr.panjiajie.cn

[O01] 启动一个线程
来源：http://im.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://si.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nx.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ok.chemitech.net.cn

TS:   // 同 JS
来源：http://qk.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://ir.asd995.cn

Go:   go f()
来源：http://gl.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://ko.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ia.panjiajie.cn

[O02] 使用线程池
来源：http://lf.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://em.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cy.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://lz.huanxung.cn

TS:   // worker_threads 线程池
来源：http://zy.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oq.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hv.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ps.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zt.newstarts.cn

[O03] 加锁保护共享数据
来源：http://wv.colortex.cn

Py:   with lock: shared += 1
来源：http://vc.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://el.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tm.chemitech.net.cn

TS:   // 同 JS
来源：http://pz.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://dp.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zg.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oq.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://su.colortex.cn

[O04] 定义异步函数并等待
来源：http://jk.asd995.cn

Py:   async def f():⏎    await g()
来源：http://cu.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hs.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://ux.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eu.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ft.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bv.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xd.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://iy.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://hr.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://tm.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rz.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://sp.asd995.cn

TS:   await Promise.all(tasks)
来源：http://yk.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ux.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yc.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ow.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ns.nicolike.cn

[O06] 使用进程池
来源：http://lv.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xc.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pq.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://tq.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://lk.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vk.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sa.521024.cn

Ruby: // fork 块
来源：http://sk.yuexingan06.cn

C#:   Parallel.For
来源：http://nn.bookmarksfly.cn

================================================================================
来源：http://xn.9csxet.cn

P. 常用工具函数
来源：http://bs.bookmarksfly.cn

================================================================================
来源：http://dx.szxytkj.cn

[P01] 生成 UUID
来源：http://mm.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://qz.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cm.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://dn.nszjky.cn

TS:   crypto.randomUUID()
来源：http://an.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://on.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://mp.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://zl.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://tq.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://iw.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ia.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zq.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://st.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dw.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ev.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sn.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dg.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kf.huanxung.cn

[P03] 生成短随机字符串
来源：http://ef.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hk.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fe.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vh.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yf.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rr.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ti.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qq.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ja.yuntaijiaju.cn

[P04] 求长度
来源：http://gq.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aj.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oh.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fr.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xm.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://cc.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://rt.shxzukj.cn

Ruby: x.length;  x.size
来源：http://fk.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ad.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://pz.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bb.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gw.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bo.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cr.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ba.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://np.huixinmuqiang.cn

Ruby: a == b
来源：http://yg.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xb.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ro.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fz.colortex.cn

PHP:  if (empty($x)) {}
来源：http://pt.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yd.szsharing.cn

TS:   if (x == null) {}
来源：http://ku.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ti.asd995.cn

Go:   if x == nil {}
来源：http://qn.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wy.chemitech.net.cn

C#:   if (x is null) {}
来源：http://lu.gzmigu.cn

[P07] 防抖与节流
来源：http://bp.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://go.wgjwhj.cn


<!-- 参考信息 -->