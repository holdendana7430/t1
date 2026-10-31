代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ye.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oy.bookmarksfly.cn

================================================================================
来源：http://ph.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://pb.huanxung.cn

================================================================================
来源：http://kv.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://ea.nicolike.cn

Py:   sys.argv[1:]
来源：http://mu.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://qg.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://lm.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ii.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://av.asd995.cn

Go:   os.Args[1:]
来源：http://xj.nicolike.cn

Ruby: ARGV
来源：http://mf.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://ec.9csxet.cn

[M02] 读取环境变量
来源：http://si.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://ur.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ip.colortex.cn

JS:   process.env.HOME
来源：http://tc.nszjky.cn

TS:   process.env.HOME
来源：http://yb.nicolike.cn

Java: System.getenv("HOME")
来源：http://ob.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rb.szsharing.cn

Ruby: ENV["HOME"]
来源：http://hr.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lb.nszjky.cn

[M03] 执行外部命令
来源：http://pu.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kl.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mk.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sj.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fb.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qz.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hh.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lo.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://le.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://kj.521024.cn

Py:   os.getcwd()
来源：http://cq.wgjwhj.cn

PHP:  getcwd();
来源：http://ot.gzmigu.cn

JS:   process.cwd()
来源：http://zs.nszjky.cn

TS:   process.cwd()
来源：http://ov.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://vr.wgjwhj.cn

Go:   os.Getwd()
来源：http://tv.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ty.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ji.gzmigu.cn

[M05] 设置退出码
来源：http://hs.nicolike.cn

Py:   sys.exit(1)
来源：http://iy.hahajie.cn

PHP:  exit(1);
来源：http://km.shtwfgs.cn

JS:   process.exit(1)
来源：http://ky.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://am.shxzukj.cn

Java: System.exit(1)
来源：http://fa.asd995.cn

Go:   os.Exit(1)
来源：http://oz.9csxet.cn

Ruby: exit 1
来源：http://kk.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kg.wgjwhj.cn

[M06] 向标准错误输出
来源：http://ck.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://wo.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bv.huixinmuqiang.cn

JS:   console.error("err")
来源：http://pz.jianghongdianzi.cn

TS:   console.error("err")
来源：http://ph.bjjhwx.cn

Java: System.err.println("err")
来源：http://yz.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pj.9csxet.cn

Ruby: warn "err"
来源：http://do.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://go.hnjuh.cn

[M07] 判断是否为主入口
来源：http://vi.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://yy.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zf.shxzukj.cn

JS:   require.main === module
来源：http://na.szsharing.cn

TS:   require.main === module
来源：http://ar.huanxung.cn

Java: public static void main(String[] args)
来源：http://ae.lnxyls.cn

Go:   func main()
来源：http://jc.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ng.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://aj.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://zm.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://bt.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://xr.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://sq.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://kv.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jj.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mw.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gc.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uz.haigaiapp.cn

================================================================================
来源：http://im.jctech888.com.cn

N. 数据结构与算法
来源：http://ee.huixiangedu.cn

================================================================================
来源：http://ih.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://he.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://px.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://by.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tg.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wj.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jj.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://pv.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gi.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://kw.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://hs.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sk.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://va.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oi.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qr.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://ho.9csxet.cn

Ruby: arr.sort
来源：http://ot.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xx.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://rc.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pv.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://yt.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eo.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://an.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mo.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ow.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ll.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://dn.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ts.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cr.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uk.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ur.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aa.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pt.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nm.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zs.jianghongdianzi.cn

[N05] 最大公约数
来源：http://dm.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://wo.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uf.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://er.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mg.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lf.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ov.huanxung.cn

Ruby: a.gcd(b)
来源：http://eu.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zt.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://vs.shxzskj.cn

Py:   s == s[::-1]
来源：http://zn.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://mj.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://ks.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://ov.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ti.asd995.cn

Go:   // 双指针从两端比较
来源：http://nh.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://xj.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ot.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://rr.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xf.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xo.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://za.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://nq.nszjky.cn

Java: // 手写 HashMap
来源：http://oi.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://bj.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://ga.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ak.jctech888.com.cn

[N08] 生成全排列
来源：http://cr.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://mh.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://ch.szsharing.cn

JS:   // 手写回溯递归
来源：http://sf.nszjky.cn

TS:   // 手写回溯递归
来源：http://sp.lnxyls.cn

Java: // 手写回溯递归
来源：http://dr.panjiajie.cn

Go:   // 手写回溯递归
来源：http://zg.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://gz.521024.cn

C#:   // 手写回溯递归
来源：http://zk.chemitech.net.cn

[N09] 栈与队列
来源：http://jn.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tx.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zy.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sz.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rf.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lg.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nd.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ce.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mv.huanxung.cn

[N10] 链表节点定义
来源：http://gd.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uu.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zg.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zr.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jx.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://ws.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://am.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://al.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kr.hahajie.cn

[N11] 二叉树中序遍历
来源：http://wn.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rr.shxzukj.cn

PHP:  // 手写递归函数
来源：http://li.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://do.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xs.bjjhwx.cn

Java: // 手写递归
来源：http://yk.szsharing.cn

Go:   // 手写递归
来源：http://ny.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jh.yuntaijiaju.cn

C#:   // 手写递归
来源：http://ud.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xr.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cy.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vz.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://un.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nh.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ch.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ct.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ad.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://od.haigaiapp.cn

================================================================================
来源：http://li.szxytkj.cn

O. 并发与异步
来源：http://vj.huixinmuqiang.cn

================================================================================
来源：http://kz.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://sp.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wn.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pf.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xb.newstarts.cn

TS:   // 同 JS
来源：http://ga.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://ua.szsharing.cn

Go:   go f()
来源：http://va.szxytkj.cn

Ruby: Thread.new { f }
来源：http://dd.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://fj.chemitech.net.cn

[O02] 使用线程池
来源：http://uh.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uv.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eh.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ht.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://zj.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hn.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cs.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xu.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qv.szsharing.cn

[O03] 加锁保护共享数据
来源：http://fe.huanxung.cn

Py:   with lock: shared += 1
来源：http://rq.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://py.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zc.huixiangedu.cn

TS:   // 同 JS
来源：http://bm.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://gh.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oa.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pp.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://we.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://pr.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://tg.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ij.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://cq.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nv.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ok.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sd.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oo.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://br.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://dd.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://xv.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lc.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://je.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://hm.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ar.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rl.nszjky.cn

Ruby: threads.map(&:join)
来源：http://vd.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://go.szsharing.cn

[O06] 使用进程池
来源：http://wx.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xo.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cm.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ik.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://vy.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yr.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vn.huixiangedu.cn

Ruby: // fork 块
来源：http://jx.newstarts.cn

C#:   Parallel.For
来源：http://ur.szsharing.cn

================================================================================
来源：http://pf.huixiangedu.cn

P. 常用工具函数
来源：http://vn.newstarts.cn

================================================================================
来源：http://py.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://lq.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://bp.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oz.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://vz.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://cm.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://qh.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://cf.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://bg.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://jj.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://ut.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dm.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oy.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ax.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ck.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xx.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qa.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wy.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qy.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://bm.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ec.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dq.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bo.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yx.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://md.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xb.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jg.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mw.jctech888.com.cn

[P04] 求长度
来源：http://gj.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://os.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hl.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ds.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cq.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://gm.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://jt.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://zj.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bd.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://rf.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fm.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zb.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ab.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hr.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dw.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vh.9csxet.cn

Ruby: a == b
来源：http://iv.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ru.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fu.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ci.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://wa.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pz.jctech888.com.cn

TS:   if (x == null) {}
来源：http://no.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uc.szxytkj.cn

Go:   if x == nil {}
来源：http://nl.nszjky.cn


<!-- 参考信息 -->