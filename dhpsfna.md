代发 wailian999

================================================================================
来源：http://gu.asd995.cn

[M01] 读取命令行参数
来源：http://ql.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://lv.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://aw.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://mh.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://mt.asd995.cn

Java: args 数组（main 方法参数）
来源：http://cu.panjiajie.cn

Go:   os.Args[1:]
来源：http://bg.hahajie.cn

Ruby: ARGV
来源：http://rr.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://qz.hnjuh.cn

[M02] 读取环境变量
来源：http://up.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://mg.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xx.gzmigu.cn

JS:   process.env.HOME
来源：http://hu.nicolike.cn

TS:   process.env.HOME
来源：http://db.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://nw.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uz.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://cq.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ul.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://cd.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nv.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ai.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dc.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pg.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://za.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ph.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://en.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://wv.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://qi.haigaiapp.cn

Py:   os.getcwd()
来源：http://vv.hnjuh.cn

PHP:  getcwd();
来源：http://ok.521024.cn

JS:   process.cwd()
来源：http://vi.shxzukj.cn

TS:   process.cwd()
来源：http://dv.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qw.colortex.cn

Go:   os.Getwd()
来源：http://vg.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://xl.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gz.yuntaijiaju.cn

[M05] 设置退出码
来源：http://mt.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://bj.bookmarksfly.cn

PHP:  exit(1);
来源：http://cz.szxytkj.cn

JS:   process.exit(1)
来源：http://qf.shtwfgs.cn

TS:   process.exit(1)
来源：http://ng.newstarts.cn

Java: System.exit(1)
来源：http://kk.lnxyls.cn

Go:   os.Exit(1)
来源：http://gy.shxzskj.cn

Ruby: exit 1
来源：http://wr.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dc.yuexingan06.cn

[M06] 向标准错误输出
来源：http://oq.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://xe.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wk.9csxet.cn

JS:   console.error("err")
来源：http://xu.hnjuh.cn

TS:   console.error("err")
来源：http://nh.asd995.cn

Java: System.err.println("err")
来源：http://jq.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ms.gzmigu.cn

Ruby: warn "err"
来源：http://rx.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://dt.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://wk.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://do.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mr.muxihuayi.cn

JS:   require.main === module
来源：http://rk.shxzskj.cn

TS:   require.main === module
来源：http://tp.hnjuh.cn

Java: public static void main(String[] args)
来源：http://wn.nicolike.cn

Go:   func main()
来源：http://dw.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://on.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://xo.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://yy.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://xb.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://cj.nszjky.cn

JS:   process.platform;  process.version
来源：http://ve.colortex.cn

TS:   process.platform;  process.version
来源：http://qg.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jk.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sr.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vw.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tq.huixinmuqiang.cn

================================================================================
来源：http://ej.gzmigu.cn

N. 数据结构与算法
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://nm.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://xi.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vp.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tz.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jx.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://je.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://cr.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lk.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qs.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://mh.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://wv.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bt.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ga.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dd.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vx.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://aq.huixiangedu.cn

Ruby: arr.sort
来源：http://xq.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://im.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://xz.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aa.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://cc.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hy.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zq.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nx.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pz.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fc.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bc.nicolike.cn

[N04] 斐波那契数列
来源：http://fl.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jm.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rk.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pp.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xf.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uk.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jg.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cs.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ky.shtwfgs.cn

[N05] 最大公约数
来源：http://ai.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://rs.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pb.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cw.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yj.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ps.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://kn.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tv.nszjky.cn

[N06] 判断回文字符串
来源：http://us.yuexingan06.cn

Py:   s == s[::-1]
来源：http://yf.huanxung.cn

PHP:  $s === strrev($s);
来源：http://fm.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://vi.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://tv.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ip.9csxet.cn

Go:   // 双指针从两端比较
来源：http://hh.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://fh.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xc.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://bz.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ku.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ug.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ui.521024.cn

TS:   // 手写 Map<string, number>
来源：http://ib.hnjuh.cn

Java: // 手写 HashMap
来源：http://qv.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://bn.szsharing.cn

Ruby: // 手写 Hash
来源：http://ob.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pe.szxytkj.cn

[N08] 生成全排列
来源：http://wa.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://jp.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://eb.panjiajie.cn

JS:   // 手写回溯递归
来源：http://za.asd995.cn

TS:   // 手写回溯递归
来源：http://ic.lnxyls.cn

Java: // 手写回溯递归
来源：http://gm.huanxung.cn

Go:   // 手写回溯递归
来源：http://sh.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://af.shxzskj.cn

C#:   // 手写回溯递归
来源：http://uh.chemitech.net.cn

[N09] 栈与队列
来源：http://jo.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://co.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gx.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ar.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://js.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lb.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bu.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dd.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dk.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://tx.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cr.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mp.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nr.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kx.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://cc.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rf.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://so.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yi.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://gg.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ac.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://pj.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zc.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uf.lnxyls.cn

Java: // 手写递归
来源：http://oh.asd995.cn

Go:   // 手写递归
来源：http://vu.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://px.hahajie.cn

C#:   // 手写递归
来源：http://in.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hx.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bp.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fq.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vu.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sc.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bp.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sd.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wz.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ub.bookmarksfly.cn

================================================================================
来源：http://lc.jianghongdianzi.cn

O. 并发与异步
来源：http://kt.haigaiapp.cn

================================================================================
来源：http://lv.nicolike.cn

[O01] 启动一个线程
来源：http://hi.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rh.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wa.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bl.lnxyls.cn

TS:   // 同 JS
来源：http://bl.521024.cn

Java: new Thread(() -> f()).start()
来源：http://uq.muxihuayi.cn

Go:   go f()
来源：http://mp.colortex.cn

Ruby: Thread.new { f }
来源：http://yi.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://rc.muxihuayi.cn

[O02] 使用线程池
来源：http://yj.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ns.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://go.521024.cn

JS:   // worker_threads 线程池
来源：http://eu.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://uw.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hk.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://se.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zg.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lz.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://pa.szsharing.cn

Py:   with lock: shared += 1
来源：http://qg.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://hy.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pw.yuexingan06.cn

TS:   // 同 JS
来源：http://zb.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://ck.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jv.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mr.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://eo.hahajie.cn

[O04] 定义异步函数并等待
来源：http://np.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://aq.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vv.nicolike.cn

JS:   async function f() { await g(); }
来源：http://ai.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jg.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ij.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://or.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lb.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://yp.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://jx.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://xb.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cy.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://tb.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://cx.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fm.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ld.hahajie.cn

Ruby: threads.map(&:join)
来源：http://fr.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://za.colortex.cn

[O06] 使用进程池
来源：http://gp.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fs.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mn.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://il.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://oh.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tp.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uh.hahajie.cn

Ruby: // fork 块
来源：http://cn.yuexingan06.cn

C#:   Parallel.For
来源：http://eg.asd995.cn

================================================================================
来源：http://he.nszjky.cn

P. 常用工具函数
来源：http://nn.hnjuh.cn

================================================================================
来源：http://dl.9csxet.cn

[P01] 生成 UUID
来源：http://tw.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://mh.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vw.colortex.cn

JS:   crypto.randomUUID()
来源：http://tr.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://nn.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://if.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://kw.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://dp.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://md.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://tw.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mv.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zk.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pe.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kb.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bx.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sh.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bc.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ux.hnjuh.cn

[P03] 生成短随机字符串
来源：http://oe.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://se.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mx.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yz.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fd.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ai.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oa.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zh.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hp.bookmarksfly.cn

[P04] 求长度
来源：http://qr.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pw.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yn.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bq.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ek.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://qw.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://uj.huanxung.cn

Ruby: x.length;  x.size
来源：http://he.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qh.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://oj.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://if.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fn.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fj.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bs.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ym.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yo.bjjhwx.cn

Ruby: a == b
来源：http://nx.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xk.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nn.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fp.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://mw.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ur.hnjuh.cn

TS:   if (x == null) {}
来源：http://wx.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://id.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://an.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vc.wgjwhj.cn

C#:   if (x is null) {}
来源：http://zh.szsharing.cn

[P07] 防抖与节流
来源：http://ar.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://un.chemitech.net.cn


<!-- 参考信息 -->