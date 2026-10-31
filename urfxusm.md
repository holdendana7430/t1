代发 wailian999

C#:   (int)resp.StatusCode
来源：http://rm.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://xb.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jx.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://li.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dz.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ek.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vh.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mn.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ny.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sy.newstarts.cn

================================================================================
来源：http://gh.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://fl.huanxung.cn

================================================================================
来源：http://dk.gzmigu.cn

[M01] 读取命令行参数
来源：http://bw.asd995.cn

Py:   sys.argv[1:]
来源：http://hr.newstarts.cn

PHP:  $argv;  $argc;
来源：http://zy.hahajie.cn

JS:   process.argv.slice(2)
来源：http://xt.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://gz.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://jk.panjiajie.cn

Go:   os.Args[1:]
来源：http://my.huixiangedu.cn

Ruby: ARGV
来源：http://kt.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://pn.haigaiapp.cn

[M02] 读取环境变量
来源：http://ji.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://zl.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wp.hnjuh.cn

JS:   process.env.HOME
来源：http://yd.hahajie.cn

TS:   process.env.HOME
来源：http://kt.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://zo.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mf.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://yv.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ep.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://yy.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wq.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tm.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rq.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sk.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uy.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tt.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mb.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://vg.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://vr.gzmigu.cn

Py:   os.getcwd()
来源：http://lw.nszjky.cn

PHP:  getcwd();
来源：http://cw.szsharing.cn

JS:   process.cwd()
来源：http://rq.yuntaijiaju.cn

TS:   process.cwd()
来源：http://wv.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://rg.huanxung.cn

Go:   os.Getwd()
来源：http://dv.szsharing.cn

Ruby: Dir.pwd
来源：http://kz.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hm.shxzskj.cn

[M05] 设置退出码
来源：http://dm.huanxung.cn

Py:   sys.exit(1)
来源：http://to.jianghongdianzi.cn

PHP:  exit(1);
来源：http://xl.bookmarksfly.cn

JS:   process.exit(1)
来源：http://de.szsharing.cn

TS:   process.exit(1)
来源：http://kf.shxzukj.cn

Java: System.exit(1)
来源：http://wh.huixiangedu.cn

Go:   os.Exit(1)
来源：http://wz.colortex.cn

Ruby: exit 1
来源：http://wx.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bu.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://di.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://yy.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ic.521024.cn

JS:   console.error("err")
来源：http://tt.hahajie.cn

TS:   console.error("err")
来源：http://ww.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://tq.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cb.jctech888.com.cn

Ruby: warn "err"
来源：http://cx.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://wr.nszjky.cn

[M07] 判断是否为主入口
来源：http://pb.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://mj.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://om.huixinmuqiang.cn

JS:   require.main === module
来源：http://ng.haigaiapp.cn

TS:   require.main === module
来源：http://bp.lnxyls.cn

Java: public static void main(String[] args)
来源：http://cn.yuexingan06.cn

Go:   func main()
来源：http://ui.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yv.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://wm.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://oz.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://lj.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://dt.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://vt.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://vz.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iy.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yt.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ao.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ok.9csxet.cn

================================================================================
来源：http://qu.huanxung.cn

N. 数据结构与算法
来源：http://we.panjiajie.cn

================================================================================
来源：http://vy.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://az.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jh.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://na.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mw.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sn.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://io.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://wk.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ab.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://db.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://yp.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://kr.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dr.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cv.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xs.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hq.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://le.gzmigu.cn

Ruby: arr.sort
来源：http://ko.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xj.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://wg.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ox.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ee.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pn.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hf.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://af.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dp.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fj.haigaiapp.cn

[N04] 斐波那契数列
来源：http://ec.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aj.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cg.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kp.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ua.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kz.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://am.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hm.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jx.szxytkj.cn

[N05] 最大公约数
来源：http://vf.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://fv.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cc.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://is.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vo.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cq.shxzskj.cn

Ruby: a.gcd(b)
来源：http://by.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xi.gzmigu.cn

[N06] 判断回文字符串
来源：http://nt.panjiajie.cn

Py:   s == s[::-1]
来源：http://rv.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://bm.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://po.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://yj.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lu.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://gm.9csxet.cn

Ruby: s == s.reverse
来源：http://ae.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pu.colortex.cn

[N07] 两数之和（返回下标）
来源：http://tb.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sv.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jr.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cx.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://qq.muxihuayi.cn

Java: // 手写 HashMap
来源：http://wb.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://rn.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://kn.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://va.panjiajie.cn

[N08] 生成全排列
来源：http://iz.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://jt.nszjky.cn

PHP:  // 手写递归交换
来源：http://pu.asd995.cn

JS:   // 手写回溯递归
来源：http://nl.gzmigu.cn

TS:   // 手写回溯递归
来源：http://rb.panjiajie.cn

Java: // 手写回溯递归
来源：http://no.nicolike.cn

Go:   // 手写回溯递归
来源：http://gy.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://wm.szsharing.cn

C#:   // 手写回溯递归
来源：http://zc.nszjky.cn

[N09] 栈与队列
来源：http://vk.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yz.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zn.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://da.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uj.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xm.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://td.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sj.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fz.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ek.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sj.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yy.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pd.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ia.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://aw.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nr.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ws.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bw.asd995.cn

[N11] 二叉树中序遍历
来源：http://gh.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ta.gzmigu.cn

PHP:  // 手写递归函数
来源：http://dv.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bl.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rm.newstarts.cn

Java: // 手写递归
来源：http://tc.chemitech.net.cn

Go:   // 手写递归
来源：http://dw.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ng.lnxyls.cn

C#:   // 手写递归
来源：http://il.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bn.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ei.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ea.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vr.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://by.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ce.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eo.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ip.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rr.lnxyls.cn

================================================================================
来源：http://jv.hahajie.cn

O. 并发与异步
来源：http://gq.yuntaijiaju.cn

================================================================================
来源：http://dz.colortex.cn

[O01] 启动一个线程
来源：http://ec.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kw.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zf.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fl.lnxyls.cn

TS:   // 同 JS
来源：http://bi.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://iu.szsharing.cn

Go:   go f()
来源：http://pj.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://tl.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://sy.shxzukj.cn

[O02] 使用线程池
来源：http://ro.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gx.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sk.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://rx.521024.cn

TS:   // worker_threads 线程池
来源：http://wr.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://is.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hy.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nh.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ld.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://oi.hnjuh.cn

Py:   with lock: shared += 1
来源：http://wp.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://aj.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xt.9csxet.cn

TS:   // 同 JS
来源：http://zd.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://sr.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wc.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kl.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://ir.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://nc.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://pa.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tb.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://ln.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xb.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sw.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fn.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mu.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ow.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://mt.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://pq.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sj.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://js.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://bf.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qx.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nt.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://vw.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://il.szxytkj.cn

[O06] 使用进程池
来源：http://mu.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gf.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hv.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://lv.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://sj.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bo.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bv.huixinmuqiang.cn

Ruby: // fork 块
来源：http://zj.haigaiapp.cn

C#:   Parallel.For
来源：http://un.muxihuayi.cn

================================================================================
来源：http://gi.newstarts.cn

P. 常用工具函数
来源：http://ou.lnxyls.cn

================================================================================
来源：http://zu.newstarts.cn

[P01] 生成 UUID
来源：http://dm.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://si.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ll.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://jk.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://fs.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://uw.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://ym.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ni.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://td.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://yt.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jr.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vx.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://es.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rr.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vx.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lf.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rh.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yt.shxzukj.cn

[P03] 生成短随机字符串
来源：http://fo.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wu.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nh.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://om.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cd.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xb.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tc.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xb.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tc.newstarts.cn

[P04] 求长度
来源：http://vm.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pz.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rh.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ud.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ed.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://na.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://aw.nicolike.cn

Ruby: x.length;  x.size
来源：http://cd.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uv.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://hb.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fu.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kv.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nv.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yf.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ld.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://di.nicolike.cn

Ruby: a == b
来源：http://qu.szsharing.cn


<!-- 参考信息 -->