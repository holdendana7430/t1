代发 wailian999

C#:   (int)resp.StatusCode
来源：http://aa.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://jt.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vo.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://hu.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wn.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mz.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rt.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vi.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qm.gzmigu.cn

================================================================================
来源：http://sl.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://hh.shxzukj.cn

================================================================================
来源：http://gg.szxytkj.cn

[M01] 读取命令行参数
来源：http://cc.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://gd.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://mb.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://pr.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://yu.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://hb.wgjwhj.cn

Go:   os.Args[1:]
来源：http://ln.muxihuayi.cn

Ruby: ARGV
来源：http://na.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://sr.jctech888.com.cn

[M02] 读取环境变量
来源：http://kf.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://wg.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qs.panjiajie.cn

JS:   process.env.HOME
来源：http://cq.asd995.cn

TS:   process.env.HOME
来源：http://ic.nszjky.cn

Java: System.getenv("HOME")
来源：http://ag.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qf.huanxung.cn

Ruby: ENV["HOME"]
来源：http://bn.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ue.521024.cn

[M03] 执行外部命令
来源：http://hj.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gz.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bc.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oq.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://du.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xv.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bi.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bk.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://fw.asd995.cn

[M04] 获取当前工作目录
来源：http://ta.yuexingan06.cn

Py:   os.getcwd()
来源：http://xv.colortex.cn

PHP:  getcwd();
来源：http://sz.huixinmuqiang.cn

JS:   process.cwd()
来源：http://io.szxytkj.cn

TS:   process.cwd()
来源：http://pr.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://yt.haigaiapp.cn

Go:   os.Getwd()
来源：http://qm.szxytkj.cn

Ruby: Dir.pwd
来源：http://sv.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gz.521024.cn

[M05] 设置退出码
来源：http://gc.shxzskj.cn

Py:   sys.exit(1)
来源：http://bb.shtwfgs.cn

PHP:  exit(1);
来源：http://vo.asd995.cn

JS:   process.exit(1)
来源：http://gw.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ti.gzmigu.cn

Java: System.exit(1)
来源：http://fw.wgjwhj.cn

Go:   os.Exit(1)
来源：http://qj.chemitech.net.cn

Ruby: exit 1
来源：http://wg.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://od.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ou.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://vq.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ts.szsharing.cn

JS:   console.error("err")
来源：http://qj.yuexingan06.cn

TS:   console.error("err")
来源：http://wv.521024.cn

Java: System.err.println("err")
来源：http://yq.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gu.bjjhwx.cn

Ruby: warn "err"
来源：http://ea.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://vo.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://qo.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://oi.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gv.huixinmuqiang.cn

JS:   require.main === module
来源：http://xa.newstarts.cn

TS:   require.main === module
来源：http://uu.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://vy.yuexingan06.cn

Go:   func main()
来源：http://kb.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yb.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://fk.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://bp.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ss.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ja.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://ad.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://sy.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xu.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jj.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qk.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ai.yuexingan06.cn

================================================================================
来源：http://sf.gzmigu.cn

N. 数据结构与算法
来源：http://bu.muxihuayi.cn

================================================================================
来源：http://fu.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://lo.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tl.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fn.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mu.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wn.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vq.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fu.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ys.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://mm.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://wx.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ze.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ax.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gl.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ye.nicolike.cn

Go:   slices.Sort(arr)
来源：http://of.huanxung.cn

Ruby: arr.sort
来源：http://ht.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://no.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://tb.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ih.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://xa.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xd.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tv.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mb.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ke.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jo.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qd.shxzukj.cn

[N04] 斐波那契数列
来源：http://fb.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ce.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sw.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xa.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ik.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iv.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ky.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lj.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cz.panjiajie.cn

[N05] 最大公约数
来源：http://up.521024.cn

Py:   math.gcd(a, b)
来源：http://uw.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rd.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bb.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zm.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kz.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pz.huanxung.cn

Ruby: a.gcd(b)
来源：http://ln.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://re.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://py.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://xs.huanxung.cn

PHP:  $s === strrev($s);
来源：http://ez.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://st.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://bw.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zc.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://lv.szsharing.cn

Ruby: s == s.reverse
来源：http://pv.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ik.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://wf.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jg.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kk.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sh.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://kf.shxzukj.cn

Java: // 手写 HashMap
来源：http://fd.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://wa.huanxung.cn

Ruby: // 手写 Hash
来源：http://ac.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ug.yuexingan06.cn

[N08] 生成全排列
来源：http://pf.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://se.521024.cn

PHP:  // 手写递归交换
来源：http://kl.lnxyls.cn

JS:   // 手写回溯递归
来源：http://ha.panjiajie.cn

TS:   // 手写回溯递归
来源：http://ki.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://cj.szxytkj.cn

Go:   // 手写回溯递归
来源：http://se.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://fl.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://fa.jianghongdianzi.cn

[N09] 栈与队列
来源：http://kg.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fa.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wg.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lb.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ug.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nv.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bs.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zw.bjjhwx.cn

[N10] 链表节点定义
来源：http://qd.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fn.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://js.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bb.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://es.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://vo.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bx.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kq.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ay.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://nu.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jo.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://il.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xy.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ed.gzmigu.cn

Java: // 手写递归
来源：http://yw.szsharing.cn

Go:   // 手写递归
来源：http://gk.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tc.szsharing.cn

C#:   // 手写递归
来源：http://fv.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xs.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fp.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rd.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sj.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ai.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sl.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wp.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fq.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ui.szxytkj.cn

================================================================================
来源：http://ao.bookmarksfly.cn

O. 并发与异步
来源：http://tc.9csxet.cn

================================================================================
来源：http://oe.szxytkj.cn

[O01] 启动一个线程
来源：http://jy.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fb.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vw.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qc.szxytkj.cn

TS:   // 同 JS
来源：http://so.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://tc.hnjuh.cn

Go:   go f()
来源：http://qg.newstarts.cn

Ruby: Thread.new { f }
来源：http://ch.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://fn.asd995.cn

[O02] 使用线程池
来源：http://ar.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pm.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vd.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://el.newstarts.cn

TS:   // worker_threads 线程池
来源：http://nj.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bo.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zk.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uz.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ya.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://ay.gzmigu.cn

Py:   with lock: shared += 1
来源：http://an.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://cx.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cm.muxihuayi.cn

TS:   // 同 JS
来源：http://ss.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://vb.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qy.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://io.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://jr.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://sf.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://hd.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tk.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://vg.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mo.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gz.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uz.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gi.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://mi.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://gg.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://th.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qb.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://pk.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://yh.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dh.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hg.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://vj.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gy.yuexingan06.cn

[O06] 使用进程池
来源：http://cs.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zj.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qe.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://tn.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://kb.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zb.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zn.newstarts.cn

Ruby: // fork 块
来源：http://il.shxzukj.cn

C#:   Parallel.For
来源：http://jn.huixiangedu.cn

================================================================================
来源：http://lf.muxihuayi.cn

P. 常用工具函数
来源：http://ld.lnxyls.cn

================================================================================
来源：http://xk.haigaiapp.cn

[P01] 生成 UUID
来源：http://ts.colortex.cn

Py:   str(uuid.uuid4())
来源：http://ou.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bu.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ep.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ha.521024.cn

Java: UUID.randomUUID().toString()
来源：http://lf.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://cb.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://fy.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://un.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://qo.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nr.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nd.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wo.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://va.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zp.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ae.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://be.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uh.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://bg.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://op.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cz.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tr.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://id.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://al.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gk.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lh.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gm.jianghongdianzi.cn

[P04] 求长度
来源：http://wk.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vw.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://by.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kl.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bj.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://jf.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://gs.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://kf.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gc.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://li.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vi.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pl.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bp.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wq.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bh.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kq.chemitech.net.cn

Ruby: a == b
来源：http://qg.colortex.cn


<!-- 参考信息 -->