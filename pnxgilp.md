代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://wv.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sb.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ve.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ie.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://rb.lnxyls.cn

Java: resp.statusCode()
来源：http://mq.bjjhwx.cn

Go:   resp.StatusCode
来源：http://um.521024.cn

Ruby: resp.code.to_i
来源：http://tb.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://mz.huanxung.cn

[L08] 并发请求多个地址
来源：http://vl.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aq.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://ew.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vj.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pf.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wl.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uh.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tk.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zv.panjiajie.cn

================================================================================
来源：http://bz.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://ja.newstarts.cn

================================================================================
来源：http://sf.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://bf.shxzskj.cn

Py:   sys.argv[1:]
来源：http://si.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://tn.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://tv.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://or.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://la.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://fn.9csxet.cn

Ruby: ARGV
来源：http://ee.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://en.lnxyls.cn

[M02] 读取环境变量
来源：http://tc.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://te.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.panjiajie.cn

JS:   process.env.HOME
来源：http://xt.hnjuh.cn

TS:   process.env.HOME
来源：http://ya.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://vo.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qc.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://tt.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ry.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://lu.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jn.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qi.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wh.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wv.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fq.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fu.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://en.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://qf.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://wi.9csxet.cn

Py:   os.getcwd()
来源：http://xb.panjiajie.cn

PHP:  getcwd();
来源：http://vv.jctech888.com.cn

JS:   process.cwd()
来源：http://nk.asd995.cn

TS:   process.cwd()
来源：http://ag.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://vk.chemitech.net.cn

Go:   os.Getwd()
来源：http://xp.hnjuh.cn

Ruby: Dir.pwd
来源：http://sq.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zs.shtwfgs.cn

[M05] 设置退出码
来源：http://tg.huixiangedu.cn

Py:   sys.exit(1)
来源：http://lu.bjjhwx.cn

PHP:  exit(1);
来源：http://nn.521024.cn

JS:   process.exit(1)
来源：http://ux.huanxung.cn

TS:   process.exit(1)
来源：http://bk.shtwfgs.cn

Java: System.exit(1)
来源：http://ba.shxzukj.cn

Go:   os.Exit(1)
来源：http://jc.lnxyls.cn

Ruby: exit 1
来源：http://qh.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ek.9csxet.cn

[M06] 向标准错误输出
来源：http://ra.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://jp.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dr.yuntaijiaju.cn

JS:   console.error("err")
来源：http://bh.nszjky.cn

TS:   console.error("err")
来源：http://kb.szsharing.cn

Java: System.err.println("err")
来源：http://ka.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mj.521024.cn

Ruby: warn "err"
来源：http://ny.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://mi.huanxung.cn

[M07] 判断是否为主入口
来源：http://uz.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://og.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wd.521024.cn

JS:   require.main === module
来源：http://va.szsharing.cn

TS:   require.main === module
来源：http://uz.nszjky.cn

Java: public static void main(String[] args)
来源：http://zo.huanxung.cn

Go:   func main()
来源：http://gt.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://om.asd995.cn

C#:   static void Main(string[] args)
来源：http://kj.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://yt.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://ig.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dm.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://bn.newstarts.cn

TS:   process.platform;  process.version
来源：http://qy.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ej.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yk.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gj.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://se.hahajie.cn

================================================================================
来源：http://gu.shxzukj.cn

N. 数据结构与算法
来源：http://rt.shxzskj.cn

================================================================================
来源：http://ip.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://fi.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vj.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yb.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cf.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mb.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ht.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://fu.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vm.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://st.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://xb.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://nk.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nq.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://io.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mz.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://es.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://gi.huanxung.cn

Ruby: arr.sort
来源：http://ls.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lp.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://kw.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ou.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://xp.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wv.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yf.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yp.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wm.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cx.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mz.wgjwhj.cn

[N04] 斐波那契数列
来源：http://bi.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jp.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xr.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pi.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vd.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wr.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tx.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ri.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bz.newstarts.cn

[N05] 最大公约数
来源：http://xp.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://nr.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lw.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://py.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jm.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xb.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wt.hahajie.cn

Ruby: a.gcd(b)
来源：http://oo.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wg.shxzskj.cn

[N06] 判断回文字符串
来源：http://zi.muxihuayi.cn

Py:   s == s[::-1]
来源：http://zu.nszjky.cn

PHP:  $s === strrev($s);
来源：http://xo.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://uf.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://yx.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jg.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://cv.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://ks.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cm.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://vv.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ty.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ck.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wu.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://kb.yuexingan06.cn

Java: // 手写 HashMap
来源：http://bh.huanxung.cn

Go:   // 手写 map[int]int
来源：http://pn.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://lc.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zk.521024.cn

[N08] 生成全排列
来源：http://la.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://hc.huanxung.cn

PHP:  // 手写递归交换
来源：http://zf.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ro.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://xb.haigaiapp.cn

Java: // 手写回溯递归
来源：http://lz.colortex.cn

Go:   // 手写回溯递归
来源：http://ve.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://bn.asd995.cn

C#:   // 手写回溯递归
来源：http://qg.shxzukj.cn

[N09] 栈与队列
来源：http://hy.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zj.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dq.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dc.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ih.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mt.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nr.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mn.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gm.9csxet.cn

[N10] 链表节点定义
来源：http://dy.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xw.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lx.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sd.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lv.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://qo.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ry.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zx.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ay.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://xo.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://di.asd995.cn

PHP:  // 手写递归函数
来源：http://rh.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://av.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uu.haigaiapp.cn

Java: // 手写递归
来源：http://mg.gzmigu.cn

Go:   // 手写递归
来源：http://hh.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://go.jctech888.com.cn

C#:   // 手写递归
来源：http://tq.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ct.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tb.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zi.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://td.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oz.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ys.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ui.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qy.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mg.521024.cn

================================================================================
来源：http://aw.haigaiapp.cn

O. 并发与异步
来源：http://kw.jianghongdianzi.cn

================================================================================
来源：http://vx.nszjky.cn

[O01] 启动一个线程
来源：http://ll.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qt.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vk.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cq.shtwfgs.cn

TS:   // 同 JS
来源：http://yl.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://cm.panjiajie.cn

Go:   go f()
来源：http://rv.nicolike.cn

Ruby: Thread.new { f }
来源：http://sb.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://bn.szsharing.cn

[O02] 使用线程池
来源：http://lw.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bj.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tv.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://lk.newstarts.cn

TS:   // worker_threads 线程池
来源：http://fz.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xf.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hg.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dp.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vt.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ml.9csxet.cn

Py:   with lock: shared += 1
来源：http://tm.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://qy.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vy.9csxet.cn

TS:   // 同 JS
来源：http://lh.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://lh.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jj.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://et.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://hu.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://qy.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://tx.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wj.9csxet.cn

JS:   async function f() { await g(); }
来源：http://us.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://be.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lj.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ye.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zd.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://hq.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://dk.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://nk.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vm.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://lb.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://bh.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gf.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ff.szsharing.cn

Ruby: threads.map(&:join)
来源：http://np.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tc.asd995.cn

[O06] 使用进程池
来源：http://lf.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hg.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hg.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://lf.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://hj.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nk.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://et.jianghongdianzi.cn

Ruby: // fork 块
来源：http://tk.panjiajie.cn

C#:   Parallel.For
来源：http://pe.colortex.cn

================================================================================
来源：http://ge.huixiangedu.cn

P. 常用工具函数
来源：http://rm.muxihuayi.cn

================================================================================
来源：http://lg.chemitech.net.cn

[P01] 生成 UUID
来源：http://jt.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://ej.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jl.521024.cn

JS:   crypto.randomUUID()
来源：http://ye.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://qe.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://gt.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://tx.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://gw.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://yk.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://xm.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xn.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ld.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nx.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kc.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ci.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ze.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oy.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sk.521024.cn

[P03] 生成短随机字符串
来源：http://ac.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ao.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wc.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ir.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yn.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ac.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zj.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zi.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ll.hahajie.cn

[P04] 求长度
来源：http://fs.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pj.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lk.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ta.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sz.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://pk.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://bq.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://jp.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mr.szxytkj.cn


<!-- 参考信息 -->