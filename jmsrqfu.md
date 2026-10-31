代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://th.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ve.nicolike.cn

================================================================================
来源：http://zb.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ng.shxzukj.cn

================================================================================
来源：http://zp.lnxyls.cn

[M01] 读取命令行参数
来源：http://kp.nszjky.cn

Py:   sys.argv[1:]
来源：http://mq.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://pi.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://xo.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://cb.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://rd.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://mh.szsharing.cn

Ruby: ARGV
来源：http://qv.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://zh.chemitech.net.cn

[M02] 读取环境变量
来源：http://xh.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ug.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cz.nicolike.cn

JS:   process.env.HOME
来源：http://oe.521024.cn

TS:   process.env.HOME
来源：http://ee.hnjuh.cn

Java: System.getenv("HOME")
来源：http://pm.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hx.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://ab.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://in.wgjwhj.cn

[M03] 执行外部命令
来源：http://rf.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://np.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ua.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ii.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vd.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ji.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wq.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yg.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://av.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://qk.szxytkj.cn

Py:   os.getcwd()
来源：http://kw.huanxung.cn

PHP:  getcwd();
来源：http://ux.shxzskj.cn

JS:   process.cwd()
来源：http://rk.huanxung.cn

TS:   process.cwd()
来源：http://ek.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://le.shtwfgs.cn

Go:   os.Getwd()
来源：http://zu.szsharing.cn

Ruby: Dir.pwd
来源：http://xm.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hr.chemitech.net.cn

[M05] 设置退出码
来源：http://xc.nicolike.cn

Py:   sys.exit(1)
来源：http://iu.jianghongdianzi.cn

PHP:  exit(1);
来源：http://va.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://dx.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://yn.huixinmuqiang.cn

Java: System.exit(1)
来源：http://dg.shxzskj.cn

Go:   os.Exit(1)
来源：http://tg.jianghongdianzi.cn

Ruby: exit 1
来源：http://pc.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mv.hnjuh.cn

[M06] 向标准错误输出
来源：http://as.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ow.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qg.hnjuh.cn

JS:   console.error("err")
来源：http://by.bookmarksfly.cn

TS:   console.error("err")
来源：http://ao.jctech888.com.cn

Java: System.err.println("err")
来源：http://bs.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dg.shxzukj.cn

Ruby: warn "err"
来源：http://zc.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://bl.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://vp.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://ue.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rn.panjiajie.cn

JS:   require.main === module
来源：http://lp.jianghongdianzi.cn

TS:   require.main === module
来源：http://bn.newstarts.cn

Java: public static void main(String[] args)
来源：http://fh.newstarts.cn

Go:   func main()
来源：http://yf.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bv.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://ku.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://ld.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ej.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://ad.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://xd.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gs.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lx.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cx.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://lx.hnjuh.cn

N. 数据结构与算法
来源：http://vp.muxihuayi.cn

================================================================================
来源：http://kz.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://uc.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ms.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ne.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nn.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rj.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vt.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://nc.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zx.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tn.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://vr.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://qh.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mb.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://el.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cm.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iz.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://on.521024.cn

Ruby: arr.sort
来源：http://xt.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xg.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://oa.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jj.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ok.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yw.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sk.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ty.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://um.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ho.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ky.panjiajie.cn

[N04] 斐波那契数列
来源：http://ej.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ji.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bq.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ff.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://am.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yu.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tb.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cx.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lx.shxzskj.cn

[N05] 最大公约数
来源：http://lg.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://kq.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fz.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gb.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zs.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ro.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sz.shxzskj.cn

Ruby: a.gcd(b)
来源：http://jm.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://or.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://vg.muxihuayi.cn

Py:   s == s[::-1]
来源：http://fn.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://sd.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://gl.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://oa.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ms.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://tk.wgjwhj.cn

Ruby: s == s.reverse
来源：http://dj.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://up.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://nq.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pw.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cj.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://av.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://xk.yuexingan06.cn

Java: // 手写 HashMap
来源：http://qv.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ii.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://hc.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://id.shxzskj.cn

[N08] 生成全排列
来源：http://cd.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://gn.panjiajie.cn

PHP:  // 手写递归交换
来源：http://vh.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://yb.shxzskj.cn

TS:   // 手写回溯递归
来源：http://se.hnjuh.cn

Java: // 手写回溯递归
来源：http://kt.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://vi.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://zb.nszjky.cn

C#:   // 手写回溯递归
来源：http://rp.nszjky.cn

[N09] 栈与队列
来源：http://xe.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vu.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lq.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://af.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xx.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rk.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://by.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sp.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yn.gzmigu.cn

[N10] 链表节点定义
来源：http://nn.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ar.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yf.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://so.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dw.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://xt.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://er.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pv.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://no.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://li.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bh.521024.cn

PHP:  // 手写递归函数
来源：http://lz.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yl.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://au.bjjhwx.cn

Java: // 手写递归
来源：http://zc.huanxung.cn

Go:   // 手写递归
来源：http://wr.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dx.gzmigu.cn

C#:   // 手写递归
来源：http://wx.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://id.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gg.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ut.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ok.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kz.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xn.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nt.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kv.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dp.bjjhwx.cn

================================================================================
来源：http://gb.bookmarksfly.cn

O. 并发与异步
来源：http://iz.bookmarksfly.cn

================================================================================
来源：http://ix.521024.cn

[O01] 启动一个线程
来源：http://wn.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://at.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jo.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sh.szxytkj.cn

TS:   // 同 JS
来源：http://rw.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://pd.haigaiapp.cn

Go:   go f()
来源：http://vg.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://wb.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://kn.newstarts.cn

[O02] 使用线程池
来源：http://aq.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zh.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nt.newstarts.cn

JS:   // worker_threads 线程池
来源：http://rw.nszjky.cn

TS:   // worker_threads 线程池
来源：http://ez.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ea.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rh.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://th.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cn.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://as.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://ti.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://zt.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fj.szxytkj.cn

TS:   // 同 JS
来源：http://vy.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://pq.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sz.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://co.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://dz.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://bl.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://ph.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qx.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://wz.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ht.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vd.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fs.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sm.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://dx.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://in.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://mj.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jc.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://pp.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://il.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lp.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cp.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://qy.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fx.haigaiapp.cn

[O06] 使用进程池
来源：http://kc.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yl.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ok.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://bi.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://zw.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sg.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wd.huixinmuqiang.cn

Ruby: // fork 块
来源：http://me.huixiangedu.cn

C#:   Parallel.For
来源：http://av.colortex.cn

================================================================================
来源：http://lt.521024.cn

P. 常用工具函数
来源：http://qc.bookmarksfly.cn

================================================================================
来源：http://bg.huanxung.cn

[P01] 生成 UUID
来源：http://lf.521024.cn

Py:   str(uuid.uuid4())
来源：http://zg.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pm.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://jt.9csxet.cn

TS:   crypto.randomUUID()
来源：http://bt.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://nf.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://jk.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://mg.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://rc.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://bg.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dh.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rw.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qx.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gt.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tf.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yc.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ip.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zc.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://cb.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qz.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xs.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qt.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rz.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bw.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xf.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pw.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mw.yuntaijiaju.cn

[P04] 求长度
来源：http://jl.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yh.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yp.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dl.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jp.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://va.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://gz.gzmigu.cn

Ruby: x.length;  x.size
来源：http://it.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bn.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://lx.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://im.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aa.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wk.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nb.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cj.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rh.521024.cn

Ruby: a == b
来源：http://tn.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iq.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://to.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rg.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://ro.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wn.chemitech.net.cn

TS:   if (x == null) {}
来源：http://vw.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ew.hnjuh.cn

Go:   if x == nil {}
来源：http://ee.shtwfgs.cn


<!-- 参考信息 -->