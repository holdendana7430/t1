代发 wailian999

C#:   (int)resp.StatusCode
来源：http://uy.hnjuh.cn

[L08] 并发请求多个地址
来源：http://hz.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rz.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://mt.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vg.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uj.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gz.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mk.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://is.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://co.shtwfgs.cn

================================================================================
来源：http://ba.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://id.szsharing.cn

================================================================================
来源：http://di.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://bn.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ax.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://dm.hahajie.cn

JS:   process.argv.slice(2)
来源：http://mc.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://pv.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://qo.jctech888.com.cn

Go:   os.Args[1:]
来源：http://yx.huanxung.cn

Ruby: ARGV
来源：http://dw.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://rf.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://pg.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://ob.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qa.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://iv.szsharing.cn

TS:   process.env.HOME
来源：http://ir.szsharing.cn

Java: System.getenv("HOME")
来源：http://tq.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mh.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://pi.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bi.muxihuayi.cn

[M03] 执行外部命令
来源：http://kn.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tp.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bk.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ac.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jz.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ei.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kd.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dq.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://ie.asd995.cn

[M04] 获取当前工作目录
来源：http://yh.muxihuayi.cn

Py:   os.getcwd()
来源：http://xi.haigaiapp.cn

PHP:  getcwd();
来源：http://ez.bjjhwx.cn

JS:   process.cwd()
来源：http://ia.huixiangedu.cn

TS:   process.cwd()
来源：http://gn.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://gp.muxihuayi.cn

Go:   os.Getwd()
来源：http://ja.panjiajie.cn

Ruby: Dir.pwd
来源：http://tv.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tk.huixiangedu.cn

[M05] 设置退出码
来源：http://ii.hnjuh.cn

Py:   sys.exit(1)
来源：http://fe.yuntaijiaju.cn

PHP:  exit(1);
来源：http://mf.huixiangedu.cn

JS:   process.exit(1)
来源：http://ar.huixiangedu.cn

TS:   process.exit(1)
来源：http://nw.521024.cn

Java: System.exit(1)
来源：http://km.panjiajie.cn

Go:   os.Exit(1)
来源：http://en.shxzskj.cn

Ruby: exit 1
来源：http://cg.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ab.haigaiapp.cn

[M06] 向标准错误输出
来源：http://sa.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://qt.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ev.szsharing.cn

JS:   console.error("err")
来源：http://sp.hnjuh.cn

TS:   console.error("err")
来源：http://jp.bjjhwx.cn

Java: System.err.println("err")
来源：http://xv.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ts.panjiajie.cn

Ruby: warn "err"
来源：http://fc.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://jy.521024.cn

[M07] 判断是否为主入口
来源：http://ph.asd995.cn

Py:   if __name__ == "__main__":
来源：http://nm.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tl.jianghongdianzi.cn

JS:   require.main === module
来源：http://tz.yuntaijiaju.cn

TS:   require.main === module
来源：http://zh.newstarts.cn

Java: public static void main(String[] args)
来源：http://bz.asd995.cn

Go:   func main()
来源：http://my.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nq.asd995.cn

C#:   static void Main(string[] args)
来源：http://dq.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://va.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://vg.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.szxytkj.cn

JS:   process.platform;  process.version
来源：http://im.colortex.cn

TS:   process.platform;  process.version
来源：http://mb.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vm.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pv.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://af.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vj.hahajie.cn

================================================================================
来源：http://wd.szsharing.cn

N. 数据结构与算法
来源：http://yg.chemitech.net.cn

================================================================================
来源：http://db.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://uh.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cx.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sr.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pj.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uf.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://sl.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bm.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jy.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://if.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lf.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yg.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://us.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ai.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nj.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://dj.lnxyls.cn

Ruby: arr.sort
来源：http://mh.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dn.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://qw.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kt.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://wm.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fd.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mn.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lr.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pm.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://id.asd995.cn

[N04] 斐波那契数列
来源：http://fd.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ty.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://go.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ih.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://af.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://th.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rb.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kl.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qt.newstarts.cn

[N05] 最大公约数
来源：http://ss.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ve.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lf.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oi.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tk.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dd.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ik.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://oy.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qo.szxytkj.cn

[N06] 判断回文字符串
来源：http://qp.jctech888.com.cn

Py:   s == s[::-1]
来源：http://dk.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://rf.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://yq.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://qz.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://za.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://zw.asd995.cn

Ruby: s == s.reverse
来源：http://bl.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vx.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://mu.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ms.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pq.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sb.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://kk.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://lt.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://nu.newstarts.cn

Ruby: // 手写 Hash
来源：http://sk.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ns.bookmarksfly.cn

[N08] 生成全排列
来源：http://ly.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ba.panjiajie.cn

PHP:  // 手写递归交换
来源：http://fe.521024.cn

JS:   // 手写回溯递归
来源：http://dz.lnxyls.cn

TS:   // 手写回溯递归
来源：http://kh.szsharing.cn

Java: // 手写回溯递归
来源：http://ds.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://qm.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://vc.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://oa.bjjhwx.cn

[N09] 栈与队列
来源：http://um.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wx.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hc.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ig.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wb.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xr.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lh.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ra.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wn.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://hj.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qo.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ln.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yy.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sl.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://gy.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ek.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iw.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://av.521024.cn

[N11] 二叉树中序遍历
来源：http://kx.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rk.huanxung.cn

PHP:  // 手写递归函数
来源：http://mj.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xs.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gp.521024.cn

Java: // 手写递归
来源：http://ar.szsharing.cn

Go:   // 手写递归
来源：http://wu.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hl.wgjwhj.cn

C#:   // 手写递归
来源：http://nu.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pb.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ou.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bb.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nq.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ll.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fd.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oq.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ct.gzmigu.cn

================================================================================
来源：http://rz.jianghongdianzi.cn

O. 并发与异步
来源：http://hu.wgjwhj.cn

================================================================================
来源：http://vz.hnjuh.cn

[O01] 启动一个线程
来源：http://yx.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://up.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mk.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wq.shxzukj.cn

TS:   // 同 JS
来源：http://bw.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ul.huanxung.cn

Go:   go f()
来源：http://we.asd995.cn

Ruby: Thread.new { f }
来源：http://np.nicolike.cn

C#:   Task.Run(() => F());
来源：http://vf.jianghongdianzi.cn

[O02] 使用线程池
来源：http://dx.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wu.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hg.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ob.huanxung.cn

TS:   // worker_threads 线程池
来源：http://xk.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xp.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yh.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://re.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jn.colortex.cn

[O03] 加锁保护共享数据
来源：http://lf.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://km.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://ol.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hc.yuexingan06.cn

TS:   // 同 JS
来源：http://ug.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://cw.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jv.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tb.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://vs.521024.cn

[O04] 定义异步函数并等待
来源：http://iw.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://cn.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vg.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://ol.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://at.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://po.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dc.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gh.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://ec.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ps.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://ej.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pt.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://vz.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://bl.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ou.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fw.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://fx.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rg.bjjhwx.cn

[O06] 使用进程池
来源：http://xi.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://om.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gt.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://gg.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://rc.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ti.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zh.muxihuayi.cn

Ruby: // fork 块
来源：http://vk.nszjky.cn

C#:   Parallel.For
来源：http://ku.hnjuh.cn

================================================================================
来源：http://ot.yuexingan06.cn

P. 常用工具函数
来源：http://pu.nicolike.cn

================================================================================
来源：http://yw.hnjuh.cn

[P01] 生成 UUID
来源：http://go.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://za.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://or.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://po.hahajie.cn

TS:   crypto.randomUUID()
来源：http://lo.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://ud.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://xj.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ps.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://ho.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://fh.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ct.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://br.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://si.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jj.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rs.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zv.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nx.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://at.huanxung.cn

[P03] 生成短随机字符串
来源：http://cp.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ej.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vz.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ot.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kd.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vd.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rc.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ex.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jf.szsharing.cn

[P04] 求长度
来源：http://up.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zu.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ro.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yu.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gc.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://li.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://wr.szsharing.cn

Ruby: x.length;  x.size
来源：http://gw.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://au.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://ge.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sm.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sv.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dj.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zy.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fu.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sf.shxzukj.cn

Ruby: a == b
来源：http://jj.shtwfgs.cn


<!-- 参考信息 -->