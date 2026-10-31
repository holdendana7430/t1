代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://sv.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eb.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gk.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://vl.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://rp.521024.cn

Java: resp.statusCode()
来源：http://iv.gzmigu.cn

Go:   resp.StatusCode
来源：http://cn.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://tf.521024.cn

C#:   (int)resp.StatusCode
来源：http://ya.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://lr.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://da.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://oi.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xf.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dw.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ib.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pl.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sq.nicolike.cn

================================================================================
来源：http://zc.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ly.hahajie.cn

================================================================================
来源：http://ht.gzmigu.cn

[M01] 读取命令行参数
来源：http://tu.szsharing.cn

Py:   sys.argv[1:]
来源：http://mj.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ol.nszjky.cn

JS:   process.argv.slice(2)
来源：http://ei.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://mg.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://tw.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://bi.muxihuayi.cn

Ruby: ARGV
来源：http://au.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://yd.gzmigu.cn

[M02] 读取环境变量
来源：http://jw.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://nm.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aw.9csxet.cn

JS:   process.env.HOME
来源：http://tl.shtwfgs.cn

TS:   process.env.HOME
来源：http://fq.9csxet.cn

Java: System.getenv("HOME")
来源：http://fq.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dm.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://wz.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vd.gzmigu.cn

[M03] 执行外部命令
来源：http://da.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://et.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tw.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gy.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yo.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rs.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mz.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hk.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://vg.huanxung.cn

[M04] 获取当前工作目录
来源：http://zo.colortex.cn

Py:   os.getcwd()
来源：http://mc.jctech888.com.cn

PHP:  getcwd();
来源：http://tx.nicolike.cn

JS:   process.cwd()
来源：http://fd.9csxet.cn

TS:   process.cwd()
来源：http://ir.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://cs.muxihuayi.cn

Go:   os.Getwd()
来源：http://cg.newstarts.cn

Ruby: Dir.pwd
来源：http://yf.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yj.yuntaijiaju.cn

[M05] 设置退出码
来源：http://ny.huanxung.cn

Py:   sys.exit(1)
来源：http://vn.huixiangedu.cn

PHP:  exit(1);
来源：http://dn.gzmigu.cn

JS:   process.exit(1)
来源：http://yl.wgjwhj.cn

TS:   process.exit(1)
来源：http://sw.chemitech.net.cn

Java: System.exit(1)
来源：http://ag.hahajie.cn

Go:   os.Exit(1)
来源：http://li.shxzukj.cn

Ruby: exit 1
来源：http://mm.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ex.hahajie.cn

[M06] 向标准错误输出
来源：http://pl.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://av.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ha.huanxung.cn

JS:   console.error("err")
来源：http://ip.haigaiapp.cn

TS:   console.error("err")
来源：http://xi.yuexingan06.cn

Java: System.err.println("err")
来源：http://oo.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ny.muxihuayi.cn

Ruby: warn "err"
来源：http://bh.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://jo.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://ib.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://mo.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uv.newstarts.cn

JS:   require.main === module
来源：http://sq.chemitech.net.cn

TS:   require.main === module
来源：http://il.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ob.asd995.cn

Go:   func main()
来源：http://wa.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oz.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ph.asd995.cn

[M08] 获取系统与运行时信息
来源：http://lr.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://zg.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://vy.shxzskj.cn

JS:   process.platform;  process.version
来源：http://qh.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://oy.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ij.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lx.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wq.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ye.9csxet.cn

================================================================================
来源：http://gq.yuntaijiaju.cn

N. 数据结构与算法
来源：http://up.haigaiapp.cn

================================================================================
来源：http://wp.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://uk.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zt.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wa.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nw.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dr.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jy.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://bl.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cq.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://pf.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://fc.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pc.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zy.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mm.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kl.521024.cn

Go:   slices.Sort(arr)
来源：http://qd.haigaiapp.cn

Ruby: arr.sort
来源：http://ww.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://te.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://mt.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xr.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://eu.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ql.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xt.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oi.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bm.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pz.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://by.shxzskj.cn

[N04] 斐波那契数列
来源：http://jn.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zz.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pl.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mr.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zt.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vn.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dk.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xy.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ze.huixiangedu.cn

[N05] 最大公约数
来源：http://qm.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://sn.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vc.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ab.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xo.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yp.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ss.hnjuh.cn

Ruby: a.gcd(b)
来源：http://in.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bt.nicolike.cn

[N06] 判断回文字符串
来源：http://vu.szxytkj.cn

Py:   s == s[::-1]
来源：http://ov.asd995.cn

PHP:  $s === strrev($s);
来源：http://oo.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://fh.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://eb.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mw.521024.cn

Go:   // 双指针从两端比较
来源：http://lq.nicolike.cn

Ruby: s == s.reverse
来源：http://el.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lu.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://xb.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lj.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sk.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yc.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ud.asd995.cn

Java: // 手写 HashMap
来源：http://yv.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://kw.newstarts.cn

Ruby: // 手写 Hash
来源：http://wl.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xe.asd995.cn

[N08] 生成全排列
来源：http://zk.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://gd.asd995.cn

PHP:  // 手写递归交换
来源：http://bj.asd995.cn

JS:   // 手写回溯递归
来源：http://km.asd995.cn

TS:   // 手写回溯递归
来源：http://pf.nszjky.cn

Java: // 手写回溯递归
来源：http://cl.nszjky.cn

Go:   // 手写回溯递归
来源：http://hl.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://nk.newstarts.cn

C#:   // 手写回溯递归
来源：http://gi.wgjwhj.cn

[N09] 栈与队列
来源：http://ci.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gs.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lv.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ro.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ne.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lv.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ii.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uf.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rh.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://bc.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://za.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gz.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ba.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://le.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://er.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pi.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vl.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ld.nicolike.cn

[N11] 二叉树中序遍历
来源：http://jn.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://re.newstarts.cn

PHP:  // 手写递归函数
来源：http://wz.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ju.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mz.huixinmuqiang.cn

Java: // 手写递归
来源：http://mv.huixiangedu.cn

Go:   // 手写递归
来源：http://vd.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nh.bookmarksfly.cn

C#:   // 手写递归
来源：http://uy.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oz.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sb.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gg.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ru.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wh.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gc.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jb.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cg.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tj.chemitech.net.cn

================================================================================
来源：http://wo.shxzukj.cn

O. 并发与异步
来源：http://cy.hnjuh.cn

================================================================================
来源：http://bg.nicolike.cn

[O01] 启动一个线程
来源：http://ae.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jy.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hq.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xu.gzmigu.cn

TS:   // 同 JS
来源：http://sn.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://nh.szxytkj.cn

Go:   go f()
来源：http://sl.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://dw.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://on.szxytkj.cn

[O02] 使用线程池
来源：http://qs.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fr.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://om.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://ti.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://he.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ov.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lp.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pd.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kx.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://vq.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://jn.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://dx.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ud.bjjhwx.cn

TS:   // 同 JS
来源：http://dt.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://wc.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pm.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iv.521024.cn

C#:   lock (gate) { shared++; }
来源：http://ad.newstarts.cn

[O04] 定义异步函数并等待
来源：http://cd.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://rs.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vi.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://fn.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tq.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yn.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uc.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uj.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://lp.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://oc.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://bb.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dz.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://sx.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://ca.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fr.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ly.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ir.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ip.jctech888.com.cn

[O06] 使用进程池
来源：http://ml.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gl.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qh.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://zo.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://lq.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iv.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xu.nszjky.cn

Ruby: // fork 块
来源：http://cm.yuntaijiaju.cn

C#:   Parallel.For
来源：http://gb.szsharing.cn

================================================================================
来源：http://ta.shtwfgs.cn

P. 常用工具函数
来源：http://it.colortex.cn

================================================================================
来源：http://us.chemitech.net.cn

[P01] 生成 UUID
来源：http://gm.colortex.cn

Py:   str(uuid.uuid4())
来源：http://jq.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fn.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ng.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://xp.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://ch.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://hl.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://yg.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://cg.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://wq.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uo.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gz.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pl.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wj.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qm.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ex.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kx.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yn.szsharing.cn

[P03] 生成短随机字符串
来源：http://qi.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xe.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ln.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tf.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iv.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ya.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rp.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ye.haigaiapp.cn

[P04] 求长度
来源：http://vq.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ca.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://td.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sb.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zd.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://gs.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://wx.nszjky.cn

Ruby: x.length;  x.size
来源：http://es.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hb.shtwfgs.cn


<!-- 参考信息 -->