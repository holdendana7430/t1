代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ny.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sk.huixiangedu.cn

================================================================================
来源：http://vi.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://vl.chemitech.net.cn

================================================================================
来源：http://om.9csxet.cn

[M01] 读取命令行参数
来源：http://be.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ty.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://ft.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://ss.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://pz.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://zz.jctech888.com.cn

Go:   os.Args[1:]
来源：http://vk.szsharing.cn

Ruby: ARGV
来源：http://ig.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://cv.bookmarksfly.cn

[M02] 读取环境变量
来源：http://yz.asd995.cn

Py:   os.environ.get("HOME")
来源：http://rc.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kk.haigaiapp.cn

JS:   process.env.HOME
来源：http://mo.haigaiapp.cn

TS:   process.env.HOME
来源：http://bf.szsharing.cn

Java: System.getenv("HOME")
来源：http://wn.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://if.szsharing.cn

Ruby: ENV["HOME"]
来源：http://cb.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://no.chemitech.net.cn

[M03] 执行外部命令
来源：http://wd.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rw.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rm.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ju.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zf.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pw.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vt.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xm.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://ii.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://yz.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://pe.newstarts.cn

PHP:  getcwd();
来源：http://ob.yuntaijiaju.cn

JS:   process.cwd()
来源：http://yj.hahajie.cn

TS:   process.cwd()
来源：http://ub.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://bj.shxzukj.cn

Go:   os.Getwd()
来源：http://jk.asd995.cn

Ruby: Dir.pwd
来源：http://ew.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cm.jianghongdianzi.cn

[M05] 设置退出码
来源：http://fr.asd995.cn

Py:   sys.exit(1)
来源：http://ck.hnjuh.cn

PHP:  exit(1);
来源：http://qp.nicolike.cn

JS:   process.exit(1)
来源：http://rn.panjiajie.cn

TS:   process.exit(1)
来源：http://bf.asd995.cn

Java: System.exit(1)
来源：http://up.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ja.muxihuayi.cn

Ruby: exit 1
来源：http://hz.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yy.huixiangedu.cn

[M06] 向标准错误输出
来源：http://fi.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://dw.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oe.huanxung.cn

JS:   console.error("err")
来源：http://tb.nicolike.cn

TS:   console.error("err")
来源：http://df.asd995.cn

Java: System.err.println("err")
来源：http://wq.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yr.huixinmuqiang.cn

Ruby: warn "err"
来源：http://cb.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://sx.gzmigu.cn

[M07] 判断是否为主入口
来源：http://sc.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://gm.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qk.9csxet.cn

JS:   require.main === module
来源：http://ya.hahajie.cn

TS:   require.main === module
来源：http://pn.hnjuh.cn

Java: public static void main(String[] args)
来源：http://nk.shxzukj.cn

Go:   func main()
来源：http://ej.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ql.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://be.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://dn.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://qq.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ph.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://wm.shxzukj.cn

TS:   process.platform;  process.version
来源：http://in.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cv.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fp.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wf.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ur.muxihuayi.cn

================================================================================
来源：http://ka.gzmigu.cn

N. 数据结构与算法
来源：http://nc.yuexingan06.cn

================================================================================
来源：http://fa.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://iq.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tt.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rc.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zq.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yz.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tl.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://do.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nh.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ai.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ra.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://hp.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qi.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gg.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://om.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nf.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://yx.gzmigu.cn

Ruby: arr.sort
来源：http://oi.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uh.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://mh.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rr.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://bf.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dq.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ic.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xj.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ge.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://og.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wq.jctech888.com.cn

[N04] 斐波那契数列
来源：http://ou.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ng.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tx.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://za.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vw.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://as.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ad.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hi.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nr.hahajie.cn

[N05] 最大公约数
来源：http://dd.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://eq.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://il.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bf.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fv.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dl.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ko.nicolike.cn

Ruby: a.gcd(b)
来源：http://eu.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ec.hahajie.cn

[N06] 判断回文字符串
来源：http://du.shxzskj.cn

Py:   s == s[::-1]
来源：http://yg.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://on.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://ib.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://my.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cq.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://jh.huanxung.cn

Ruby: s == s.reverse
来源：http://wo.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ja.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://hu.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yd.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://br.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bn.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://fk.haigaiapp.cn

Java: // 手写 HashMap
来源：http://nl.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ls.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://am.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wu.muxihuayi.cn

[N08] 生成全排列
来源：http://op.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://we.huanxung.cn

PHP:  // 手写递归交换
来源：http://dj.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://zm.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://nm.szxytkj.cn

Java: // 手写回溯递归
来源：http://nw.lnxyls.cn

Go:   // 手写回溯递归
来源：http://wj.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://hq.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://kc.newstarts.cn

[N09] 栈与队列
来源：http://nd.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fy.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://go.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tb.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qz.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ee.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eu.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vh.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gi.yuexingan06.cn

[N10] 链表节点定义
来源：http://bf.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://el.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uk.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tm.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zj.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ik.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://an.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qz.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ye.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ly.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gg.newstarts.cn

PHP:  // 手写递归函数
来源：http://ss.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uo.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mw.asd995.cn

Java: // 手写递归
来源：http://mc.wgjwhj.cn

Go:   // 手写递归
来源：http://tn.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tq.nicolike.cn

C#:   // 手写递归
来源：http://go.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sv.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vs.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gh.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://of.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jo.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tn.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sb.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zc.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.bjjhwx.cn

================================================================================
来源：http://hi.shxzukj.cn

O. 并发与异步
来源：http://az.gzmigu.cn

================================================================================
来源：http://uz.hnjuh.cn

[O01] 启动一个线程
来源：http://uq.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vu.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ul.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dj.shtwfgs.cn

TS:   // 同 JS
来源：http://zu.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://rc.nicolike.cn

Go:   go f()
来源：http://tc.panjiajie.cn

Ruby: Thread.new { f }
来源：http://zd.nicolike.cn

C#:   Task.Run(() => F());
来源：http://mm.nicolike.cn

[O02] 使用线程池
来源：http://hh.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sy.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fz.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ev.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://uj.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ln.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zq.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yv.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gn.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://od.shxzskj.cn

Py:   with lock: shared += 1
来源：http://ly.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://dr.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ui.colortex.cn

TS:   // 同 JS
来源：http://pa.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://eh.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jh.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yg.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://ux.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://og.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://bo.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nb.nicolike.cn

JS:   async function f() { await g(); }
来源：http://lo.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pq.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jt.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kc.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uw.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://vl.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://hj.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://wk.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://js.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://sk.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://xt.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ol.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ra.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://cf.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ak.shxzskj.cn

[O06] 使用进程池
来源：http://si.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cb.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hp.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://xz.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://hj.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qd.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ws.jianghongdianzi.cn

Ruby: // fork 块
来源：http://pk.huixiangedu.cn

C#:   Parallel.For
来源：http://lz.huixiangedu.cn

================================================================================
来源：http://cd.gzmigu.cn

P. 常用工具函数
来源：http://jj.colortex.cn

================================================================================
来源：http://vy.hahajie.cn

[P01] 生成 UUID
来源：http://br.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://rb.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kw.9csxet.cn

JS:   crypto.randomUUID()
来源：http://zf.nicolike.cn

TS:   crypto.randomUUID()
来源：http://kr.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://bc.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://mu.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://bo.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://sa.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://gg.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://om.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zd.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sw.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jt.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xk.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sr.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mu.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kt.gzmigu.cn

[P03] 生成短随机字符串
来源：http://dz.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tx.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hx.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ru.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jp.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gw.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iq.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rs.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vr.colortex.cn

[P04] 求长度
来源：http://sd.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://it.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qd.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sm.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ju.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://bt.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://bm.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://em.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sk.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://po.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ij.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://em.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qw.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tw.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kp.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mj.shtwfgs.cn

Ruby: a == b
来源：http://rc.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://th.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://am.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lx.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://vm.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ha.yuexingan06.cn

TS:   if (x == null) {}
来源：http://if.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yt.shxzskj.cn

Go:   if x == nil {}
来源：http://so.szxytkj.cn


<!-- 参考信息 -->