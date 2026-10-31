代发 wailian999

C#:   (int)resp.StatusCode
来源：http://pf.9csxet.cn

[L08] 并发请求多个地址
来源：http://gt.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sp.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://xn.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vv.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iq.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fo.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hc.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vv.haigaiapp.cn

================================================================================
来源：http://gv.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://jr.haigaiapp.cn

================================================================================
来源：http://ty.asd995.cn

[M01] 读取命令行参数
来源：http://ik.szxytkj.cn

Py:   sys.argv[1:]
来源：http://bz.newstarts.cn

PHP:  $argv;  $argc;
来源：http://sd.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://oj.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ni.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://xd.shxzukj.cn

Go:   os.Args[1:]
来源：http://xt.szxytkj.cn

Ruby: ARGV
来源：http://cn.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ho.lnxyls.cn

[M02] 读取环境变量
来源：http://yq.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://qb.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://os.szxytkj.cn

JS:   process.env.HOME
来源：http://lb.panjiajie.cn

TS:   process.env.HOME
来源：http://xu.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://lk.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gt.9csxet.cn

Ruby: ENV["HOME"]
来源：http://pi.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ur.9csxet.cn

[M03] 执行外部命令
来源：http://oo.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pa.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mw.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ol.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rq.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vm.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zw.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rr.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://to.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://ys.shxzukj.cn

Py:   os.getcwd()
来源：http://iu.lnxyls.cn

PHP:  getcwd();
来源：http://bu.chemitech.net.cn

JS:   process.cwd()
来源：http://xw.nszjky.cn

TS:   process.cwd()
来源：http://hy.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://tg.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://xk.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ol.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ti.huixiangedu.cn

[M05] 设置退出码
来源：http://pv.9csxet.cn

Py:   sys.exit(1)
来源：http://br.muxihuayi.cn

PHP:  exit(1);
来源：http://lh.shxzskj.cn

JS:   process.exit(1)
来源：http://yr.muxihuayi.cn

TS:   process.exit(1)
来源：http://wd.chemitech.net.cn

Java: System.exit(1)
来源：http://mx.shtwfgs.cn

Go:   os.Exit(1)
来源：http://sm.lnxyls.cn

Ruby: exit 1
来源：http://mk.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qh.shtwfgs.cn

[M06] 向标准错误输出
来源：http://hq.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://dk.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pm.jianghongdianzi.cn

JS:   console.error("err")
来源：http://tf.nicolike.cn

TS:   console.error("err")
来源：http://sl.huixiangedu.cn

Java: System.err.println("err")
来源：http://uh.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fj.asd995.cn

Ruby: warn "err"
来源：http://uq.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://ly.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://xo.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://et.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ks.gzmigu.cn

JS:   require.main === module
来源：http://ka.shtwfgs.cn

TS:   require.main === module
来源：http://wx.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://fi.521024.cn

Go:   func main()
来源：http://ip.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vt.newstarts.cn

C#:   static void Main(string[] args)
来源：http://fj.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://fl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://qc.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://tr.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://yu.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://yy.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ot.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qt.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rf.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pb.nszjky.cn

================================================================================
来源：http://ze.szxytkj.cn

N. 数据结构与算法
来源：http://ef.panjiajie.cn

================================================================================
来源：http://kh.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://tz.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ch.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ik.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ny.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qg.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hl.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://pj.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zz.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gx.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://sm.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wo.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nq.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fv.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://er.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ey.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ps.chemitech.net.cn

Ruby: arr.sort
来源：http://pb.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vi.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://dy.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pu.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://ig.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sd.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qn.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://re.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zg.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://os.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qg.nszjky.cn

[N04] 斐波那契数列
来源：http://yw.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ox.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lp.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kb.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://de.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mo.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wh.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://df.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kk.haigaiapp.cn

[N05] 最大公约数
来源：http://tb.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://em.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pj.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mm.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lm.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kg.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sv.hahajie.cn

Ruby: a.gcd(b)
来源：http://cc.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ls.panjiajie.cn

[N06] 判断回文字符串
来源：http://kq.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://st.nicolike.cn

PHP:  $s === strrev($s);
来源：http://dy.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://pc.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://ym.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bf.newstarts.cn

Go:   // 双指针从两端比较
来源：http://jc.bjjhwx.cn

Ruby: s == s.reverse
来源：http://op.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pd.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://pk.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uy.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yh.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bu.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://tm.chemitech.net.cn

Java: // 手写 HashMap
来源：http://fp.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://wp.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ib.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ed.huanxung.cn

[N08] 生成全排列
来源：http://wl.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://yw.nszjky.cn

PHP:  // 手写递归交换
来源：http://sj.panjiajie.cn

JS:   // 手写回溯递归
来源：http://ue.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://uf.shtwfgs.cn

Java: // 手写回溯递归
来源：http://tw.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://wt.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://lq.nicolike.cn

C#:   // 手写回溯递归
来源：http://cv.hnjuh.cn

[N09] 栈与队列
来源：http://ft.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fs.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bi.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ob.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ie.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ef.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xp.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kx.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://om.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://oo.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gc.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qe.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xt.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rh.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://tx.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ok.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ej.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sl.huanxung.cn

[N11] 二叉树中序遍历
来源：http://lq.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ul.shxzskj.cn

PHP:  // 手写递归函数
来源：http://xe.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://na.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vt.521024.cn

Java: // 手写递归
来源：http://qd.yuexingan06.cn

Go:   // 手写递归
来源：http://pl.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ji.colortex.cn

C#:   // 手写递归
来源：http://xa.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gz.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uq.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ph.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ua.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xp.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ph.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://li.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aj.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cx.shxzskj.cn

================================================================================
来源：http://wc.jianghongdianzi.cn

O. 并发与异步
来源：http://mu.yuntaijiaju.cn

================================================================================
来源：http://yn.shtwfgs.cn

[O01] 启动一个线程
来源：http://si.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vs.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://po.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://la.nszjky.cn

TS:   // 同 JS
来源：http://uk.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://th.hahajie.cn

Go:   go f()
来源：http://gf.huanxung.cn

Ruby: Thread.new { f }
来源：http://hd.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://zm.yuntaijiaju.cn

[O02] 使用线程池
来源：http://fb.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jy.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://la.asd995.cn

JS:   // worker_threads 线程池
来源：http://jm.hahajie.cn

TS:   // worker_threads 线程池
来源：http://bj.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lb.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iq.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hy.hahajie.cn

[O03] 加锁保护共享数据
来源：http://qn.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://od.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://zw.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eg.521024.cn

TS:   // 同 JS
来源：http://cb.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://rw.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mp.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rn.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://fn.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ku.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://tm.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kg.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://oy.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tw.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ob.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vh.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ba.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://tk.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://km.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://cd.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://te.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://ne.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://lz.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ld.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uj.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://oe.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://so.colortex.cn

[O06] 使用进程池
来源：http://hr.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bx.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://em.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://zb.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://eu.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yz.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://va.jctech888.com.cn

Ruby: // fork 块
来源：http://by.jianghongdianzi.cn

C#:   Parallel.For
来源：http://pv.shxzukj.cn

================================================================================
来源：http://fh.szxytkj.cn

P. 常用工具函数
来源：http://va.newstarts.cn

================================================================================
来源：http://eq.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://eg.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://ci.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ut.9csxet.cn

JS:   crypto.randomUUID()
来源：http://mz.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://yz.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://iw.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://if.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://tt.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ix.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ly.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jo.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sh.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qx.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tv.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mw.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bg.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zt.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nd.hnjuh.cn

[P03] 生成短随机字符串
来源：http://ik.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wu.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ca.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xy.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wd.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jp.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wo.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uw.szxytkj.cn

[P04] 求长度
来源：http://jn.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rk.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bz.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://im.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xd.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://hk.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ei.nicolike.cn

Ruby: x.length;  x.size
来源：http://sn.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fh.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://tt.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pj.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iv.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bh.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jh.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bm.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vt.lnxyls.cn

Ruby: a == b
来源：http://hi.colortex.cn


<!-- 参考信息 -->