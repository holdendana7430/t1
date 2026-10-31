代发 wailian999

C#:   (int)resp.StatusCode
来源：http://oz.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://az.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qr.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ey.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cq.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lr.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ck.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yd.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tr.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ks.gzmigu.cn

================================================================================
来源：http://bs.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://aa.lnxyls.cn

================================================================================
来源：http://qg.muxihuayi.cn

[M01] 读取命令行参数
来源：http://mh.panjiajie.cn

Py:   sys.argv[1:]
来源：http://dd.szsharing.cn

PHP:  $argv;  $argc;
来源：http://df.colortex.cn

JS:   process.argv.slice(2)
来源：http://qv.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://qp.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://ks.jctech888.com.cn

Go:   os.Args[1:]
来源：http://uk.nicolike.cn

Ruby: ARGV
来源：http://ei.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://gb.colortex.cn

[M02] 读取环境变量
来源：http://we.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://ng.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://su.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://yf.szsharing.cn

TS:   process.env.HOME
来源：http://hj.szsharing.cn

Java: System.getenv("HOME")
来源：http://sy.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://om.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://wt.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pv.nszjky.cn

[M03] 执行外部命令
来源：http://ta.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://am.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://od.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zy.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tr.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mb.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ar.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bl.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://yy.panjiajie.cn

[M04] 获取当前工作目录
来源：http://ly.asd995.cn

Py:   os.getcwd()
来源：http://nu.gzmigu.cn

PHP:  getcwd();
来源：http://cd.nszjky.cn

JS:   process.cwd()
来源：http://ch.huixiangedu.cn

TS:   process.cwd()
来源：http://pj.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://sh.newstarts.cn

Go:   os.Getwd()
来源：http://fm.asd995.cn

Ruby: Dir.pwd
来源：http://wc.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qn.jctech888.com.cn

[M05] 设置退出码
来源：http://xq.9csxet.cn

Py:   sys.exit(1)
来源：http://be.lnxyls.cn

PHP:  exit(1);
来源：http://zm.panjiajie.cn

JS:   process.exit(1)
来源：http://qp.bjjhwx.cn

TS:   process.exit(1)
来源：http://rf.bjjhwx.cn

Java: System.exit(1)
来源：http://ce.nszjky.cn

Go:   os.Exit(1)
来源：http://ar.lnxyls.cn

Ruby: exit 1
来源：http://zo.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qa.haigaiapp.cn

[M06] 向标准错误输出
来源：http://ea.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ap.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jf.huixiangedu.cn

JS:   console.error("err")
来源：http://ey.jianghongdianzi.cn

TS:   console.error("err")
来源：http://fe.asd995.cn

Java: System.err.println("err")
来源：http://la.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rr.bjjhwx.cn

Ruby: warn "err"
来源：http://ry.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://we.shxzukj.cn

[M07] 判断是否为主入口
来源：http://id.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://xy.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kw.9csxet.cn

JS:   require.main === module
来源：http://db.bjjhwx.cn

TS:   require.main === module
来源：http://wp.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://bm.shtwfgs.cn

Go:   func main()
来源：http://ro.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cu.9csxet.cn

C#:   static void Main(string[] args)
来源：http://wa.521024.cn

[M08] 获取系统与运行时信息
来源：http://vv.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://zk.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vx.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://wz.lnxyls.cn

TS:   process.platform;  process.version
来源：http://jt.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wy.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ow.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ws.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ja.yuexingan06.cn

================================================================================
来源：http://yc.panjiajie.cn

N. 数据结构与算法
来源：http://kh.hnjuh.cn

================================================================================
来源：http://ts.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://oc.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://op.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jj.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nk.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gu.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bu.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://tq.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rr.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yd.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://nu.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ok.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uw.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ju.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ct.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://du.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://jw.nszjky.cn

Ruby: arr.sort
来源：http://td.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yh.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://dm.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rn.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://sm.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tb.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ce.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qa.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xq.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nr.hnjuh.cn

[N04] 斐波那契数列
来源：http://cu.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tb.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bz.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dv.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ni.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://on.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yt.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hw.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gt.shxzskj.cn

[N05] 最大公约数
来源：http://xn.nszjky.cn

Py:   math.gcd(a, b)
来源：http://ro.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://en.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rk.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zm.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mu.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ya.lnxyls.cn

Ruby: a.gcd(b)
来源：http://bi.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fk.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://ej.gzmigu.cn

Py:   s == s[::-1]
来源：http://cp.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://em.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ay.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://qx.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sz.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://jv.shxzskj.cn

Ruby: s == s.reverse
来源：http://gl.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vh.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ip.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ju.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iq.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://br.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://vc.panjiajie.cn

Java: // 手写 HashMap
来源：http://gh.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://qy.szsharing.cn

Ruby: // 手写 Hash
来源：http://fy.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yn.huixiangedu.cn

[N08] 生成全排列
来源：http://zz.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://dr.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://st.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://dg.asd995.cn

TS:   // 手写回溯递归
来源：http://nx.shxzukj.cn

Java: // 手写回溯递归
来源：http://ni.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://be.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://os.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://dp.bookmarksfly.cn

[N09] 栈与队列
来源：http://ks.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ds.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lu.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gl.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cy.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iy.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hv.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xp.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pw.nszjky.cn

[N10] 链表节点定义
来源：http://mo.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dn.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gk.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://za.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xl.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://kc.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bb.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yo.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gv.hahajie.cn

[N11] 二叉树中序遍历
来源：http://ot.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wf.hnjuh.cn

PHP:  // 手写递归函数
来源：http://rc.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yw.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yq.haigaiapp.cn

Java: // 手写递归
来源：http://qw.jianghongdianzi.cn

Go:   // 手写递归
来源：http://nl.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ep.newstarts.cn

C#:   // 手写递归
来源：http://ke.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zb.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ao.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lj.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vt.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://le.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hx.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ng.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wc.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zp.colortex.cn

================================================================================
来源：http://az.asd995.cn

O. 并发与异步
来源：http://nj.shxzskj.cn

================================================================================
来源：http://ey.nicolike.cn

[O01] 启动一个线程
来源：http://ib.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ie.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yp.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vg.yuntaijiaju.cn

TS:   // 同 JS
来源：http://zd.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://ma.hahajie.cn

Go:   go f()
来源：http://db.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://al.hahajie.cn

C#:   Task.Run(() => F());
来源：http://qw.gzmigu.cn

[O02] 使用线程池
来源：http://zd.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eg.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hn.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://xb.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://pu.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gh.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ai.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://la.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sb.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://kn.521024.cn

Py:   with lock: shared += 1
来源：http://gu.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ch.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nf.jctech888.com.cn

TS:   // 同 JS
来源：http://li.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://bl.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ta.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pc.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://fj.szsharing.cn

[O04] 定义异步函数并等待
来源：http://vr.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://tr.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cd.hahajie.cn

JS:   async function f() { await g(); }
来源：http://cb.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nr.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ht.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iv.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cs.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://tm.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ms.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://uh.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://re.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://ct.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://lv.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oh.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ja.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://tf.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lw.jctech888.com.cn

[O06] 使用进程池
来源：http://gj.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kg.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gy.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://at.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://cd.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ir.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cc.huanxung.cn

Ruby: // fork 块
来源：http://zo.huixinmuqiang.cn

C#:   Parallel.For
来源：http://mo.jianghongdianzi.cn

================================================================================
来源：http://td.bjjhwx.cn

P. 常用工具函数
来源：http://mo.shtwfgs.cn

================================================================================
来源：http://nl.521024.cn

[P01] 生成 UUID
来源：http://hv.asd995.cn

Py:   str(uuid.uuid4())
来源：http://hw.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ez.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://tr.colortex.cn

TS:   crypto.randomUUID()
来源：http://zu.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://gd.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://ug.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://gg.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://dd.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ga.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kl.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gw.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vg.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kx.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://it.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jh.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yi.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rv.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://yw.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ma.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wl.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kn.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wj.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qx.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pz.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mz.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eo.hnjuh.cn

[P04] 求长度
来源：http://hi.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ew.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tt.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ft.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hc.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://jp.newstarts.cn

Go:   len(arr);  len(m)
来源：http://gb.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://yc.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xq.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://jd.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vt.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hn.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iu.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eu.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wg.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xp.newstarts.cn

Ruby: a == b
来源：http://fc.yuexingan06.cn


<!-- 参考信息 -->