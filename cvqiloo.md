代发 wailian999

TS:   resp.ok;  resp.status
来源：http://dy.bjjhwx.cn

Java: resp.statusCode()
来源：http://zl.lnxyls.cn

Go:   resp.StatusCode
来源：http://ix.colortex.cn

Ruby: resp.code.to_i
来源：http://gy.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://sx.colortex.cn

[L08] 并发请求多个地址
来源：http://ue.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xd.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://xg.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jk.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://be.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wg.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://av.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nh.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jn.jianghongdianzi.cn

================================================================================
来源：http://fd.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://mp.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://fc.gzmigu.cn

Py:   sys.argv[1:]
来源：http://bv.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://ln.hahajie.cn

JS:   process.argv.slice(2)
来源：http://bz.asd995.cn

TS:   process.argv.slice(2)
来源：http://ow.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://jo.jctech888.com.cn

Go:   os.Args[1:]
来源：http://wz.hahajie.cn

Ruby: ARGV
来源：http://fa.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://zi.wgjwhj.cn

[M02] 读取环境变量
来源：http://by.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://xp.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ap.huanxung.cn

JS:   process.env.HOME
来源：http://xl.yuexingan06.cn

TS:   process.env.HOME
来源：http://ox.newstarts.cn

Java: System.getenv("HOME")
来源：http://ba.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tk.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://up.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kf.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://jo.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dl.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qr.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fo.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xl.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xd.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kk.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yd.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://fa.nicolike.cn

[M04] 获取当前工作目录
来源：http://ap.jctech888.com.cn

Py:   os.getcwd()
来源：http://gg.colortex.cn

PHP:  getcwd();
来源：http://sn.shxzskj.cn

JS:   process.cwd()
来源：http://ck.newstarts.cn

TS:   process.cwd()
来源：http://gc.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://cd.szxytkj.cn

Go:   os.Getwd()
来源：http://pd.hahajie.cn

Ruby: Dir.pwd
来源：http://mu.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yw.bookmarksfly.cn

[M05] 设置退出码
来源：http://fv.bjjhwx.cn

Py:   sys.exit(1)
来源：http://xu.colortex.cn

PHP:  exit(1);
来源：http://ze.huixiangedu.cn

JS:   process.exit(1)
来源：http://lc.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://yg.shxzukj.cn

Java: System.exit(1)
来源：http://nj.szsharing.cn

Go:   os.Exit(1)
来源：http://is.wgjwhj.cn

Ruby: exit 1
来源：http://yc.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ve.nicolike.cn

[M06] 向标准错误输出
来源：http://st.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://no.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fv.huanxung.cn

JS:   console.error("err")
来源：http://dc.bjjhwx.cn

TS:   console.error("err")
来源：http://wq.colortex.cn

Java: System.err.println("err")
来源：http://au.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pz.jctech888.com.cn

Ruby: warn "err"
来源：http://xd.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ut.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://gk.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://zo.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xl.chemitech.net.cn

JS:   require.main === module
来源：http://bd.jianghongdianzi.cn

TS:   require.main === module
来源：http://zn.huanxung.cn

Java: public static void main(String[] args)
来源：http://gn.jianghongdianzi.cn

Go:   func main()
来源：http://tl.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iz.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://ed.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://tc.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ag.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://og.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://fc.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://yf.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gq.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rm.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://up.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://au.hnjuh.cn

================================================================================
来源：http://rz.yuntaijiaju.cn

N. 数据结构与算法
来源：http://mf.nicolike.cn

================================================================================
来源：http://xj.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://jk.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sf.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wx.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://up.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oz.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qq.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://os.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xx.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://he.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://es.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cm.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aj.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yf.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ww.huanxung.cn

Go:   slices.Sort(arr)
来源：http://sg.bjjhwx.cn

Ruby: arr.sort
来源：http://uv.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sv.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://on.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cr.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://zw.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fv.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rg.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gv.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://up.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cz.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vl.szsharing.cn

[N04] 斐波那契数列
来源：http://lp.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bj.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cd.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sp.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ge.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oy.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uy.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://os.9csxet.cn

[N05] 最大公约数
来源：http://qn.colortex.cn

Py:   math.gcd(a, b)
来源：http://oh.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vz.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ca.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vr.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://os.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://xm.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://an.wgjwhj.cn

[N06] 判断回文字符串
来源：http://wp.muxihuayi.cn

Py:   s == s[::-1]
来源：http://dx.huanxung.cn

PHP:  $s === strrev($s);
来源：http://cm.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://em.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://wh.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hm.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://um.haigaiapp.cn

Ruby: s == s.reverse
来源：http://za.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gn.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://ma.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xf.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ta.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wo.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://gk.nicolike.cn

Java: // 手写 HashMap
来源：http://uu.hahajie.cn

Go:   // 手写 map[int]int
来源：http://hj.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://js.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kt.huixinmuqiang.cn

[N08] 生成全排列
来源：http://gi.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://xi.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://kg.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://xm.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://fa.bjjhwx.cn

Java: // 手写回溯递归
来源：http://zz.shxzskj.cn

Go:   // 手写回溯递归
来源：http://fe.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://op.nszjky.cn

C#:   // 手写回溯递归
来源：http://ti.huixinmuqiang.cn

[N09] 栈与队列
来源：http://rp.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://su.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pa.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jn.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rj.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xk.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xs.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kh.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ic.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://iw.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sd.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kq.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://in.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vx.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://sh.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wt.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xy.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aw.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://yr.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jh.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://xa.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pa.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wx.asd995.cn

Java: // 手写递归
来源：http://md.muxihuayi.cn

Go:   // 手写递归
来源：http://cl.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lu.521024.cn

C#:   // 手写递归
来源：http://jw.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xf.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uj.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pw.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cy.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mz.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sc.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ph.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ag.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pc.huixiangedu.cn

================================================================================
来源：http://vu.shtwfgs.cn

O. 并发与异步
来源：http://pm.hahajie.cn

================================================================================
来源：http://lv.panjiajie.cn

[O01] 启动一个线程
来源：http://ah.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yt.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sq.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ie.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ft.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://mt.bookmarksfly.cn

Go:   go f()
来源：http://hw.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://ed.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://gr.nszjky.cn

[O02] 使用线程池
来源：http://xn.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ax.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://br.nszjky.cn

JS:   // worker_threads 线程池
来源：http://ch.asd995.cn

TS:   // worker_threads 线程池
来源：http://tx.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kc.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ge.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://me.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yn.asd995.cn

[O03] 加锁保护共享数据
来源：http://go.newstarts.cn

Py:   with lock: shared += 1
来源：http://nc.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://xh.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rj.gzmigu.cn

TS:   // 同 JS
来源：http://mr.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://vy.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qp.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jr.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ds.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://yq.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://uh.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vz.huanxung.cn

JS:   async function f() { await g(); }
来源：http://vo.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bx.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gr.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://db.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gg.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://cr.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ni.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ha.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pm.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://nc.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://zo.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gs.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uy.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://bo.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nc.szsharing.cn

[O06] 使用进程池
来源：http://ad.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ig.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bl.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://tj.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://eu.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rl.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ic.nszjky.cn

Ruby: // fork 块
来源：http://mp.yuexingan06.cn

C#:   Parallel.For
来源：http://ii.colortex.cn

================================================================================
来源：http://ch.szsharing.cn

P. 常用工具函数
来源：http://ck.szxytkj.cn

================================================================================
来源：http://du.lnxyls.cn

[P01] 生成 UUID
来源：http://yv.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ps.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iv.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ii.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://gm.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ps.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://ak.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://an.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://px.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://dx.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qx.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ej.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uu.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dr.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jq.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://in.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gi.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://av.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://ms.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kn.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ge.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hs.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zk.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://we.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jy.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gc.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ss.bjjhwx.cn

[P04] 求长度
来源：http://xx.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ax.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gp.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fk.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qy.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://uk.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://dh.newstarts.cn

Ruby: x.length;  x.size
来源：http://ed.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gd.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://xo.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://up.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ru.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yb.colortex.cn


<!-- 参考信息 -->