代发 wailian999

TS:   resp.ok;  resp.status
来源：http://rn.szxytkj.cn

Java: resp.statusCode()
来源：http://yo.huanxung.cn

Go:   resp.StatusCode
来源：http://ey.9csxet.cn

Ruby: resp.code.to_i
来源：http://xi.521024.cn

C#:   (int)resp.StatusCode
来源：http://oq.szxytkj.cn

[L08] 并发请求多个地址
来源：http://zm.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ko.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://ci.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vu.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ms.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ct.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://if.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gn.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vm.nszjky.cn

================================================================================
来源：http://os.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://gr.nicolike.cn

================================================================================
来源：http://kn.jctech888.com.cn

[M01] 读取命令行参数
来源：http://dv.9csxet.cn

Py:   sys.argv[1:]
来源：http://kv.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://vt.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://qp.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://od.521024.cn

Java: args 数组（main 方法参数）
来源：http://jj.huixiangedu.cn

Go:   os.Args[1:]
来源：http://kj.szsharing.cn

Ruby: ARGV
来源：http://ht.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://zr.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://ss.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://cv.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vg.colortex.cn

JS:   process.env.HOME
来源：http://sv.bjjhwx.cn

TS:   process.env.HOME
来源：http://yr.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://uw.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hx.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://cp.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cn.shxzskj.cn

[M03] 执行外部命令
来源：http://ix.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lz.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sd.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tx.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ta.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ku.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ie.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://mn.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://dn.gzmigu.cn

Py:   os.getcwd()
来源：http://je.chemitech.net.cn

PHP:  getcwd();
来源：http://cm.yuexingan06.cn

JS:   process.cwd()
来源：http://qq.jianghongdianzi.cn

TS:   process.cwd()
来源：http://fg.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://ay.shxzskj.cn

Go:   os.Getwd()
来源：http://ua.colortex.cn

Ruby: Dir.pwd
来源：http://or.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iv.jctech888.com.cn

[M05] 设置退出码
来源：http://we.9csxet.cn

Py:   sys.exit(1)
来源：http://in.colortex.cn

PHP:  exit(1);
来源：http://lz.chemitech.net.cn

JS:   process.exit(1)
来源：http://do.9csxet.cn

TS:   process.exit(1)
来源：http://re.yuexingan06.cn

Java: System.exit(1)
来源：http://xc.chemitech.net.cn

Go:   os.Exit(1)
来源：http://rt.jianghongdianzi.cn

Ruby: exit 1
来源：http://cn.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bi.9csxet.cn

[M06] 向标准错误输出
来源：http://vm.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://fi.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mk.huixinmuqiang.cn

JS:   console.error("err")
来源：http://mw.jianghongdianzi.cn

TS:   console.error("err")
来源：http://sx.9csxet.cn

Java: System.err.println("err")
来源：http://ni.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jy.wgjwhj.cn

Ruby: warn "err"
来源：http://dg.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://of.gzmigu.cn

[M07] 判断是否为主入口
来源：http://pg.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ae.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qa.nszjky.cn

JS:   require.main === module
来源：http://ra.huixiangedu.cn

TS:   require.main === module
来源：http://fx.lnxyls.cn

Java: public static void main(String[] args)
来源：http://nj.szsharing.cn

Go:   func main()
来源：http://lq.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mg.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://ho.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://he.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://eh.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://ep.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://eo.shxzskj.cn

TS:   process.platform;  process.version
来源：http://mj.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kd.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wh.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hp.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://do.shxzskj.cn

================================================================================
来源：http://xg.shxzskj.cn

N. 数据结构与算法
来源：http://is.521024.cn

================================================================================
来源：http://ht.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://le.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ls.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hx.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hs.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sn.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jq.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ap.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fi.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sn.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://al.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://gq.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pw.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oq.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kg.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ul.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://jq.9csxet.cn

Ruby: arr.sort
来源：http://kj.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fd.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://is.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://md.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://qw.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nw.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hb.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yt.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://if.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zn.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dr.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://kd.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dl.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rq.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pk.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ue.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xk.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ed.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ie.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://he.bookmarksfly.cn

[N05] 最大公约数
来源：http://co.521024.cn

Py:   math.gcd(a, b)
来源：http://jq.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qw.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mh.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mo.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yw.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zm.gzmigu.cn

Ruby: a.gcd(b)
来源：http://dd.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mw.bjjhwx.cn

[N06] 判断回文字符串
来源：http://pt.muxihuayi.cn

Py:   s == s[::-1]
来源：http://wf.huanxung.cn

PHP:  $s === strrev($s);
来源：http://gd.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://ww.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://da.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ui.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://pt.shtwfgs.cn

Ruby: s == s.reverse
来源：http://kw.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dd.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://wa.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://om.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://df.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://me.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://rl.9csxet.cn

Java: // 手写 HashMap
来源：http://wb.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ex.newstarts.cn

Ruby: // 手写 Hash
来源：http://hu.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rn.shtwfgs.cn

[N08] 生成全排列
来源：http://ed.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://im.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://by.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://fz.hnjuh.cn

TS:   // 手写回溯递归
来源：http://pj.lnxyls.cn

Java: // 手写回溯递归
来源：http://an.nicolike.cn

Go:   // 手写回溯递归
来源：http://jq.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://of.521024.cn

C#:   // 手写回溯递归
来源：http://vh.yuexingan06.cn

[N09] 栈与队列
来源：http://kn.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ie.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ny.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bm.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zt.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vc.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wj.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://km.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fr.521024.cn

[N10] 链表节点定义
来源：http://ky.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://co.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ex.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lf.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vq.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ij.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://db.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jl.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nd.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://mk.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lv.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://pd.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cl.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lw.shtwfgs.cn

Java: // 手写递归
来源：http://fk.nszjky.cn

Go:   // 手写递归
来源：http://at.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zx.shxzskj.cn

C#:   // 手写递归
来源：http://gx.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sr.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uv.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ps.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nk.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ye.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ll.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://my.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://am.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ez.hnjuh.cn

================================================================================
来源：http://sd.wgjwhj.cn

O. 并发与异步
来源：http://nu.521024.cn

================================================================================
来源：http://xx.newstarts.cn

[O01] 启动一个线程
来源：http://bv.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ny.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gq.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vu.chemitech.net.cn

TS:   // 同 JS
来源：http://ie.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://yr.newstarts.cn

Go:   go f()
来源：http://aw.hnjuh.cn

Ruby: Thread.new { f }
来源：http://dg.521024.cn

C#:   Task.Run(() => F());
来源：http://fg.szsharing.cn

[O02] 使用线程池
来源：http://sl.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oo.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kv.asd995.cn

JS:   // worker_threads 线程池
来源：http://by.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://yw.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mx.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jc.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nj.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ta.521024.cn

[O03] 加锁保护共享数据
来源：http://pt.lnxyls.cn

Py:   with lock: shared += 1
来源：http://zv.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://av.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zu.shtwfgs.cn

TS:   // 同 JS
来源：http://xe.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://vf.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://el.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pq.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://dn.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://db.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://xq.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wn.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://hr.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zc.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ys.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tv.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://af.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://hq.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://vt.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://di.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bk.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ie.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://af.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sg.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://df.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://sp.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tx.bookmarksfly.cn

[O06] 使用进程池
来源：http://mq.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ly.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ua.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://vn.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://gf.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tb.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uz.bookmarksfly.cn

Ruby: // fork 块
来源：http://vo.newstarts.cn

C#:   Parallel.For
来源：http://cp.shtwfgs.cn

================================================================================
来源：http://gc.jctech888.com.cn

P. 常用工具函数
来源：http://ts.asd995.cn

================================================================================
来源：http://oj.muxihuayi.cn

[P01] 生成 UUID
来源：http://zd.colortex.cn

Py:   str(uuid.uuid4())
来源：http://qo.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://au.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://cz.9csxet.cn

TS:   crypto.randomUUID()
来源：http://wj.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://jz.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://vg.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://fc.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://rk.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://mn.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ow.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kw.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gn.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xp.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vh.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wb.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aj.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vg.shxzskj.cn

[P03] 生成短随机字符串
来源：http://vm.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yb.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kh.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ef.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jp.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ph.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oz.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lt.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ne.bookmarksfly.cn

[P04] 求长度
来源：http://qw.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://is.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vu.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lh.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ht.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://em.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://ya.hnjuh.cn

Ruby: x.length;  x.size
来源：http://zk.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sj.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://ia.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zg.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fb.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aj.hahajie.cn


<!-- 参考信息 -->