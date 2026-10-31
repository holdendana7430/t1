代发 wailian999

TS:   resp.ok;  resp.status
来源：http://bf.newstarts.cn

Java: resp.statusCode()
来源：http://zn.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://co.hnjuh.cn

Ruby: resp.code.to_i
来源：http://xx.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://ie.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://ky.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kd.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://rl.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bq.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ax.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://md.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oh.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ej.shtwfgs.cn

================================================================================
来源：http://ph.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://kx.huixiangedu.cn

================================================================================
来源：http://uy.jctech888.com.cn

[M01] 读取命令行参数
来源：http://ai.9csxet.cn

Py:   sys.argv[1:]
来源：http://aq.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://sf.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://cb.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://zk.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://fn.hnjuh.cn

Go:   os.Args[1:]
来源：http://jc.muxihuayi.cn

Ruby: ARGV
来源：http://il.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://hv.gzmigu.cn

[M02] 读取环境变量
来源：http://rw.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ro.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nc.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://nz.shxzukj.cn

TS:   process.env.HOME
来源：http://rs.9csxet.cn

Java: System.getenv("HOME")
来源：http://nj.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://np.huanxung.cn

Ruby: ENV["HOME"]
来源：http://gu.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mx.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://pr.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bl.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mu.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://as.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wn.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yd.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xx.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lq.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://pq.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://pf.wgjwhj.cn

Py:   os.getcwd()
来源：http://rs.hahajie.cn

PHP:  getcwd();
来源：http://nx.szxytkj.cn

JS:   process.cwd()
来源：http://gl.panjiajie.cn

TS:   process.cwd()
来源：http://mk.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://us.newstarts.cn

Go:   os.Getwd()
来源：http://jx.bjjhwx.cn

Ruby: Dir.pwd
来源：http://mg.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gv.bjjhwx.cn

[M05] 设置退出码
来源：http://zh.asd995.cn

Py:   sys.exit(1)
来源：http://tg.shxzskj.cn

PHP:  exit(1);
来源：http://gp.bookmarksfly.cn

JS:   process.exit(1)
来源：http://kt.nicolike.cn

TS:   process.exit(1)
来源：http://zl.huixiangedu.cn

Java: System.exit(1)
来源：http://js.521024.cn

Go:   os.Exit(1)
来源：http://nq.muxihuayi.cn

Ruby: exit 1
来源：http://zy.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ud.panjiajie.cn

[M06] 向标准错误输出
来源：http://it.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://sf.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kr.newstarts.cn

JS:   console.error("err")
来源：http://ul.szsharing.cn

TS:   console.error("err")
来源：http://xp.521024.cn

Java: System.err.println("err")
来源：http://wh.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xc.wgjwhj.cn

Ruby: warn "err"
来源：http://go.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://lb.colortex.cn

[M07] 判断是否为主入口
来源：http://cy.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://yn.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qt.shtwfgs.cn

JS:   require.main === module
来源：http://if.bjjhwx.cn

TS:   require.main === module
来源：http://oz.hnjuh.cn

Java: public static void main(String[] args)
来源：http://pd.bjjhwx.cn

Go:   func main()
来源：http://jl.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ss.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://qu.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://tu.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://xp.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://rd.szxytkj.cn

JS:   process.platform;  process.version
来源：http://aa.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://xu.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cl.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sv.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xq.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dl.9csxet.cn

================================================================================
来源：http://wc.bjjhwx.cn

N. 数据结构与算法
来源：http://bu.muxihuayi.cn

================================================================================
来源：http://bx.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://xj.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mh.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eu.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kq.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://va.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yl.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://hw.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://al.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ny.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://td.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://tk.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dy.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hh.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lm.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jz.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://kf.szxytkj.cn

Ruby: arr.sort
来源：http://xv.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wa.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://bi.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gl.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://qv.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dp.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yd.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ue.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kz.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bd.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xp.chemitech.net.cn

[N04] 斐波那契数列
来源：http://ih.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tu.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jw.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gx.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pr.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xu.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sz.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bj.shtwfgs.cn

[N05] 最大公约数
来源：http://iu.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://fz.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ru.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://as.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mn.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kk.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://da.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://xo.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sd.9csxet.cn

[N06] 判断回文字符串
来源：http://hj.9csxet.cn

Py:   s == s[::-1]
来源：http://gk.9csxet.cn

PHP:  $s === strrev($s);
来源：http://xe.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://oi.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://pg.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mk.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://bu.jctech888.com.cn

Ruby: s == s.reverse
来源：http://ts.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hq.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://oi.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pu.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gw.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kd.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://zq.panjiajie.cn

Java: // 手写 HashMap
来源：http://js.colortex.cn

Go:   // 手写 map[int]int
来源：http://ny.shxzukj.cn

Ruby: // 手写 Hash
来源：http://px.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bj.bookmarksfly.cn

[N08] 生成全排列
来源：http://ih.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://xt.newstarts.cn

PHP:  // 手写递归交换
来源：http://ni.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://sk.newstarts.cn

TS:   // 手写回溯递归
来源：http://il.9csxet.cn

Java: // 手写回溯递归
来源：http://zq.asd995.cn

Go:   // 手写回溯递归
来源：http://vj.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://jp.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://wj.panjiajie.cn

[N09] 栈与队列
来源：http://de.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uz.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://te.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ra.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pq.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mu.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ob.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ml.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ar.szxytkj.cn

[N10] 链表节点定义
来源：http://za.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://us.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://to.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://op.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tw.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://fv.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ik.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fs.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vo.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://go.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iq.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://ll.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://na.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gr.colortex.cn

Java: // 手写递归
来源：http://ew.yuntaijiaju.cn

Go:   // 手写递归
来源：http://qy.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wy.jctech888.com.cn

C#:   // 手写递归
来源：http://zr.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zi.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rv.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oe.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zj.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ip.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vm.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vp.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://we.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rh.muxihuayi.cn

================================================================================
来源：http://up.yuexingan06.cn

O. 并发与异步
来源：http://of.asd995.cn

================================================================================
来源：http://ms.szsharing.cn

[O01] 启动一个线程
来源：http://hr.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vq.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bd.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ig.colortex.cn

TS:   // 同 JS
来源：http://ua.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://yu.9csxet.cn

Go:   go f()
来源：http://en.hnjuh.cn

Ruby: Thread.new { f }
来源：http://lk.szsharing.cn

C#:   Task.Run(() => F());
来源：http://ax.szxytkj.cn

[O02] 使用线程池
来源：http://rc.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eq.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nd.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://kq.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://sb.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ll.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hm.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kg.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vm.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://di.hahajie.cn

Py:   with lock: shared += 1
来源：http://hc.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ho.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xk.shxzskj.cn

TS:   // 同 JS
来源：http://ka.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://wb.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ag.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ad.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://vh.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://sz.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://rj.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hy.szsharing.cn

JS:   async function f() { await g(); }
来源：http://ce.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xi.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mn.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aq.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://po.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://ts.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ru.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://kc.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gq.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://fx.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://na.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://et.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fw.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://qf.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iu.haigaiapp.cn

[O06] 使用进程池
来源：http://yn.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ys.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lj.asd995.cn

JS:   // child_process / cluster 模块
来源：http://ma.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://xq.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zl.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kl.szxytkj.cn

Ruby: // fork 块
来源：http://sr.bookmarksfly.cn

C#:   Parallel.For
来源：http://df.hnjuh.cn

================================================================================
来源：http://cu.shtwfgs.cn

P. 常用工具函数
来源：http://kz.shxzskj.cn

================================================================================
来源：http://wa.gzmigu.cn

[P01] 生成 UUID
来源：http://hf.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://yh.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sa.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://pj.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://dt.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://gd.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://vf.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ng.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://qh.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://gl.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hd.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ar.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kl.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ws.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ii.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ze.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qo.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://li.colortex.cn

[P03] 生成短随机字符串
来源：http://ru.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bq.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ps.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lt.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bp.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hg.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dk.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ia.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mo.wgjwhj.cn

[P04] 求长度
来源：http://tt.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://on.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pd.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mn.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ba.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://uo.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://lg.panjiajie.cn

Ruby: x.length;  x.size
来源：http://xe.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ml.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://dr.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sy.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yo.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wj.hahajie.cn


<!-- 参考信息 -->