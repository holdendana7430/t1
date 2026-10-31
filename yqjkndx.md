代发 wailian999

C#:   (int)resp.StatusCode
来源：http://vx.nszjky.cn

[L08] 并发请求多个地址
来源：http://jk.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uc.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://bq.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pw.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pf.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rz.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jg.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lj.muxihuayi.cn

================================================================================
来源：http://wh.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://fq.hahajie.cn

================================================================================
来源：http://vk.newstarts.cn

[M01] 读取命令行参数
来源：http://ld.hahajie.cn

Py:   sys.argv[1:]
来源：http://qp.szsharing.cn

PHP:  $argv;  $argc;
来源：http://au.9csxet.cn

JS:   process.argv.slice(2)
来源：http://he.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ko.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://lb.hnjuh.cn

Go:   os.Args[1:]
来源：http://mm.lnxyls.cn

Ruby: ARGV
来源：http://wv.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://of.lnxyls.cn

[M02] 读取环境变量
来源：http://oy.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://gc.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ms.9csxet.cn

JS:   process.env.HOME
来源：http://vz.chemitech.net.cn

TS:   process.env.HOME
来源：http://lu.shxzskj.cn

Java: System.getenv("HOME")
来源：http://bk.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tk.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://uz.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yf.nicolike.cn

[M03] 执行外部命令
来源：http://cu.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lf.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yn.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ke.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fp.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vu.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hk.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ge.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://eh.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ip.szsharing.cn

Py:   os.getcwd()
来源：http://lk.szxytkj.cn

PHP:  getcwd();
来源：http://jw.hnjuh.cn

JS:   process.cwd()
来源：http://ro.hahajie.cn

TS:   process.cwd()
来源：http://dq.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ld.gzmigu.cn

Go:   os.Getwd()
来源：http://vd.521024.cn

Ruby: Dir.pwd
来源：http://yf.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qf.yuntaijiaju.cn

[M05] 设置退出码
来源：http://jc.shtwfgs.cn

Py:   sys.exit(1)
来源：http://er.jctech888.com.cn

PHP:  exit(1);
来源：http://nr.muxihuayi.cn

JS:   process.exit(1)
来源：http://sp.shxzukj.cn

TS:   process.exit(1)
来源：http://vo.chemitech.net.cn

Java: System.exit(1)
来源：http://tw.szxytkj.cn

Go:   os.Exit(1)
来源：http://mh.hnjuh.cn

Ruby: exit 1
来源：http://qj.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sw.huixiangedu.cn

[M06] 向标准错误输出
来源：http://za.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://kp.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://su.shxzukj.cn

JS:   console.error("err")
来源：http://yf.haigaiapp.cn

TS:   console.error("err")
来源：http://vp.shxzukj.cn

Java: System.err.println("err")
来源：http://tu.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fy.9csxet.cn

Ruby: warn "err"
来源：http://tc.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ow.szsharing.cn

[M07] 判断是否为主入口
来源：http://bu.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://wz.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lz.huanxung.cn

JS:   require.main === module
来源：http://vd.lnxyls.cn

TS:   require.main === module
来源：http://vp.gzmigu.cn

Java: public static void main(String[] args)
来源：http://se.jctech888.com.cn

Go:   func main()
来源：http://ds.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dh.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://ew.521024.cn

[M08] 获取系统与运行时信息
来源：http://qo.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://vx.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://au.9csxet.cn

JS:   process.platform;  process.version
来源：http://xa.nicolike.cn

TS:   process.platform;  process.version
来源：http://ys.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ex.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xg.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wr.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pc.hnjuh.cn

================================================================================
来源：http://gn.haigaiapp.cn

N. 数据结构与算法
来源：http://hv.yuexingan06.cn

================================================================================
来源：http://ty.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ic.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://op.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oh.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vi.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bk.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hc.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sl.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ro.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://no.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ds.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xx.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qp.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pz.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://el.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ii.lnxyls.cn

Ruby: arr.sort
来源：http://my.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wi.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://uy.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wr.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://lk.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qk.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://va.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pd.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tr.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qy.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzmigu.cn

[N04] 斐波那契数列
来源：http://rm.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tq.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ku.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zt.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://av.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bx.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ug.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qz.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ls.colortex.cn

[N05] 最大公约数
来源：http://zm.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://gw.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kt.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pb.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ya.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sj.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xn.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://ho.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hm.szsharing.cn

[N06] 判断回文字符串
来源：http://uc.nszjky.cn

Py:   s == s[::-1]
来源：http://kb.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://uy.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ey.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://nk.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gs.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://oo.wgjwhj.cn

Ruby: s == s.reverse
来源：http://qu.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://li.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://zu.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fz.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dt.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zq.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://yf.huixiangedu.cn

Java: // 手写 HashMap
来源：http://vy.nicolike.cn

Go:   // 手写 map[int]int
来源：http://gq.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://mk.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mo.colortex.cn

[N08] 生成全排列
来源：http://wz.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://mi.9csxet.cn

PHP:  // 手写递归交换
来源：http://gh.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://wn.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://bi.nszjky.cn

Java: // 手写回溯递归
来源：http://qy.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://cg.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://ui.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://ng.panjiajie.cn

[N09] 栈与队列
来源：http://ru.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eu.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yi.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://av.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dv.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ao.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aj.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vd.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sr.newstarts.cn

[N10] 链表节点定义
来源：http://ol.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pv.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://af.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wa.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qn.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://km.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ev.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hf.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://od.szsharing.cn

[N11] 二叉树中序遍历
来源：http://rp.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rv.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ap.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xe.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rt.szsharing.cn

Java: // 手写递归
来源：http://ae.szxytkj.cn

Go:   // 手写递归
来源：http://aj.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sa.9csxet.cn

C#:   // 手写递归
来源：http://cw.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wo.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aj.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://to.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ai.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://po.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qs.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eb.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pe.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://jc.yuntaijiaju.cn

O. 并发与异步
来源：http://xm.yuntaijiaju.cn

================================================================================
来源：http://yb.shxzukj.cn

[O01] 启动一个线程
来源：http://kz.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jl.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://np.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sg.521024.cn

TS:   // 同 JS
来源：http://ze.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://yc.lnxyls.cn

Go:   go f()
来源：http://fy.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://dd.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://cs.jctech888.com.cn

[O02] 使用线程池
来源：http://mz.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qn.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oi.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://wh.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://rp.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fv.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ae.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://re.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jw.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://kq.lnxyls.cn

Py:   with lock: shared += 1
来源：http://ox.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://qk.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ym.panjiajie.cn

TS:   // 同 JS
来源：http://yd.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://vc.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dl.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cq.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://nb.hahajie.cn

[O04] 定义异步函数并等待
来源：http://xf.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://qk.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mt.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://fd.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ak.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wh.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wh.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nc.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://sk.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://ms.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://ep.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ud.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://zn.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://cs.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://il.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dc.9csxet.cn

Ruby: threads.map(&:join)
来源：http://jp.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ya.jianghongdianzi.cn

[O06] 使用进程池
来源：http://zr.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ya.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ol.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ij.asd995.cn

TS:   // child_process / cluster 模块
来源：http://vl.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gi.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vi.shxzskj.cn

Ruby: // fork 块
来源：http://kr.lnxyls.cn

C#:   Parallel.For
来源：http://xl.jctech888.com.cn

================================================================================
来源：http://vz.wgjwhj.cn

P. 常用工具函数
来源：http://dp.521024.cn

================================================================================
来源：http://lj.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://yc.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://hz.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bz.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://nq.colortex.cn

TS:   crypto.randomUUID()
来源：http://qd.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://nw.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ne.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://jd.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://iz.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://qx.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gi.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://om.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yk.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aq.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kz.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tv.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hj.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oi.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://eb.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tl.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://or.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hs.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bu.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://po.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://it.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yv.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xw.bjjhwx.cn

[P04] 求长度
来源：http://ur.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ie.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nc.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qe.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ci.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://um.nicolike.cn

Ruby: x.length;  x.size
来源：http://zx.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vy.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://wz.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://co.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bl.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ct.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ft.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hr.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hs.szxytkj.cn

Ruby: a == b
来源：http://eb.jctech888.com.cn


<!-- 参考信息 -->