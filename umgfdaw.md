代发 wailian999

C#:   (int)resp.StatusCode
来源：http://ol.newstarts.cn

[L08] 并发请求多个地址
来源：http://su.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zs.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://hg.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dl.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wx.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ka.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://du.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tb.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cn.yuntaijiaju.cn

================================================================================
来源：http://zo.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://dk.9csxet.cn

================================================================================
来源：http://ad.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://rq.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://sz.nicolike.cn

PHP:  $argv;  $argc;
来源：http://xh.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://we.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://bp.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://nh.shtwfgs.cn

Go:   os.Args[1:]
来源：http://pq.colortex.cn

Ruby: ARGV
来源：http://yy.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://hq.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://xg.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://fu.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wy.asd995.cn

JS:   process.env.HOME
来源：http://xe.asd995.cn

TS:   process.env.HOME
来源：http://nm.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://bq.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iq.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://pl.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xh.colortex.cn

[M03] 执行外部命令
来源：http://zs.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ur.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yw.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gn.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oz.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ox.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ry.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ju.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://zk.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://be.lnxyls.cn

Py:   os.getcwd()
来源：http://nb.szsharing.cn

PHP:  getcwd();
来源：http://wt.szsharing.cn

JS:   process.cwd()
来源：http://ln.bookmarksfly.cn

TS:   process.cwd()
来源：http://ob.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://oc.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://qs.9csxet.cn

Ruby: Dir.pwd
来源：http://zj.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lo.colortex.cn

[M05] 设置退出码
来源：http://cg.9csxet.cn

Py:   sys.exit(1)
来源：http://fi.yuntaijiaju.cn

PHP:  exit(1);
来源：http://tk.521024.cn

JS:   process.exit(1)
来源：http://zw.gzmigu.cn

TS:   process.exit(1)
来源：http://ke.szxytkj.cn

Java: System.exit(1)
来源：http://az.szxytkj.cn

Go:   os.Exit(1)
来源：http://os.colortex.cn

Ruby: exit 1
来源：http://st.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ig.nszjky.cn

[M06] 向标准错误输出
来源：http://mt.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://eg.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://se.muxihuayi.cn

JS:   console.error("err")
来源：http://ss.shxzukj.cn

TS:   console.error("err")
来源：http://ut.wgjwhj.cn

Java: System.err.println("err")
来源：http://qf.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sd.yuntaijiaju.cn

Ruby: warn "err"
来源：http://ld.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://fs.521024.cn

[M07] 判断是否为主入口
来源：http://pi.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://qp.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://si.newstarts.cn

JS:   require.main === module
来源：http://de.shxzukj.cn

TS:   require.main === module
来源：http://dg.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://ek.shxzskj.cn

Go:   func main()
来源：http://bf.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://im.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://dz.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://jt.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://wo.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ne.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://gp.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://tc.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vf.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ri.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ug.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xr.lnxyls.cn

================================================================================
来源：http://uz.lnxyls.cn

N. 数据结构与算法
来源：http://fx.newstarts.cn

================================================================================
来源：http://zc.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://ce.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://id.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jy.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yo.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ln.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://nw.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yd.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://sg.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://mi.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uf.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cc.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xw.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jo.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://id.9csxet.cn

Ruby: arr.sort
来源：http://ok.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jl.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://sj.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kr.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ie.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wq.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://co.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qb.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pb.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nv.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pe.lnxyls.cn

[N04] 斐波那契数列
来源：http://fn.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tl.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yj.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ny.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qk.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://js.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qi.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tb.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://px.lnxyls.cn

[N05] 最大公约数
来源：http://gy.huanxung.cn

Py:   math.gcd(a, b)
来源：http://zv.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sd.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://al.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mu.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pj.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rh.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://zp.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ay.szsharing.cn

[N06] 判断回文字符串
来源：http://pj.jctech888.com.cn

Py:   s == s[::-1]
来源：http://eb.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://mo.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://pp.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://io.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://om.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://ka.nicolike.cn

Ruby: s == s.reverse
来源：http://vi.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sx.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://rw.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bq.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://up.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xb.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://og.shxzskj.cn

Java: // 手写 HashMap
来源：http://gn.521024.cn

Go:   // 手写 map[int]int
来源：http://gm.nicolike.cn

Ruby: // 手写 Hash
来源：http://kn.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xc.colortex.cn

[N08] 生成全排列
来源：http://cv.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://cu.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://jc.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ev.521024.cn

TS:   // 手写回溯递归
来源：http://or.muxihuayi.cn

Java: // 手写回溯递归
来源：http://ke.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://bw.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://nt.nszjky.cn

C#:   // 手写回溯递归
来源：http://jz.hahajie.cn

[N09] 栈与队列
来源：http://ac.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wk.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hv.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ol.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://es.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jq.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tg.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://na.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ic.bookmarksfly.cn

[N10] 链表节点定义
来源：http://lb.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://la.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lg.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mk.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kf.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://qe.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mb.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bp.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://se.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://db.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yq.szsharing.cn

PHP:  // 手写递归函数
来源：http://fs.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xe.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ok.wgjwhj.cn

Java: // 手写递归
来源：http://os.szsharing.cn

Go:   // 手写递归
来源：http://ja.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ic.hnjuh.cn

C#:   // 手写递归
来源：http://pg.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://df.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cd.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tk.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rg.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cx.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://al.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zq.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://up.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://md.haigaiapp.cn

================================================================================
来源：http://mw.shtwfgs.cn

O. 并发与异步
来源：http://ws.szsharing.cn

================================================================================
来源：http://wh.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://lp.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ns.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://in.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yh.nszjky.cn

TS:   // 同 JS
来源：http://bp.521024.cn

Java: new Thread(() -> f()).start()
来源：http://du.yuntaijiaju.cn

Go:   go f()
来源：http://ar.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://ka.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://cz.nicolike.cn

[O02] 使用线程池
来源：http://ct.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kh.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wn.521024.cn

JS:   // worker_threads 线程池
来源：http://rp.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://gn.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dz.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yx.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ly.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oz.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://jn.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://rn.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gf.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ge.colortex.cn

TS:   // 同 JS
来源：http://qz.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://qo.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mx.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hl.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://za.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://lb.521024.cn

Py:   async def f():⏎    await g()
来源：http://fu.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ji.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://vc.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nz.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ai.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zu.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://fz.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://eb.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://on.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://so.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ec.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://rc.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gr.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nq.huanxung.cn

Ruby: threads.map(&:join)
来源：http://cv.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ue.bjjhwx.cn

[O06] 使用进程池
来源：http://vz.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oj.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fd.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://qs.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://ki.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xv.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xj.shxzukj.cn

Ruby: // fork 块
来源：http://ao.shxzskj.cn

C#:   Parallel.For
来源：http://lu.jctech888.com.cn

================================================================================
来源：http://bm.asd995.cn

P. 常用工具函数
来源：http://ib.521024.cn

================================================================================
来源：http://ae.nicolike.cn

[P01] 生成 UUID
来源：http://cs.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://tn.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fv.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://pw.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://fe.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://hh.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://zc.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://dr.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://zk.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://pi.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lv.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lr.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zi.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://su.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kr.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rc.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zw.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hm.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://cg.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qv.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jm.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vx.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pe.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ez.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tf.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gx.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ox.muxihuayi.cn

[P04] 求长度
来源：http://en.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ww.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ac.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ih.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://va.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://nb.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://cr.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://sa.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vm.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://cd.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kh.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oe.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yv.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bx.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gw.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jm.yuexingan06.cn

Ruby: a == b
来源：http://kv.hnjuh.cn


<!-- 参考信息 -->