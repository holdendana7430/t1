代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vr.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rt.shxzukj.cn

================================================================================
来源：http://hz.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://py.szxytkj.cn

================================================================================
来源：http://mk.bjjhwx.cn

[M01] 读取命令行参数
来源：http://yf.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://bd.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://lz.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://ci.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://bo.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://bp.yuexingan06.cn

Go:   os.Args[1:]
来源：http://oy.nicolike.cn

Ruby: ARGV
来源：http://lm.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://uj.asd995.cn

[M02] 读取环境变量
来源：http://fi.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://rv.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://br.szxytkj.cn

JS:   process.env.HOME
来源：http://po.asd995.cn

TS:   process.env.HOME
来源：http://jb.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://bx.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bg.nszjky.cn

Ruby: ENV["HOME"]
来源：http://kh.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mw.nszjky.cn

[M03] 执行外部命令
来源：http://rs.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://du.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sa.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jz.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xl.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mh.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bt.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://im.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://nn.colortex.cn

[M04] 获取当前工作目录
来源：http://sq.9csxet.cn

Py:   os.getcwd()
来源：http://en.9csxet.cn

PHP:  getcwd();
来源：http://rv.shxzukj.cn

JS:   process.cwd()
来源：http://ut.shxzukj.cn

TS:   process.cwd()
来源：http://cc.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://os.jctech888.com.cn

Go:   os.Getwd()
来源：http://pk.colortex.cn

Ruby: Dir.pwd
来源：http://hw.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ef.hnjuh.cn

[M05] 设置退出码
来源：http://jp.huanxung.cn

Py:   sys.exit(1)
来源：http://jh.panjiajie.cn

PHP:  exit(1);
来源：http://sd.hahajie.cn

JS:   process.exit(1)
来源：http://nf.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://gw.9csxet.cn

Java: System.exit(1)
来源：http://wb.huanxung.cn

Go:   os.Exit(1)
来源：http://ic.nicolike.cn

Ruby: exit 1
来源：http://ge.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nw.muxihuayi.cn

[M06] 向标准错误输出
来源：http://pu.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://yy.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://md.huixinmuqiang.cn

JS:   console.error("err")
来源：http://rk.haigaiapp.cn

TS:   console.error("err")
来源：http://tf.newstarts.cn

Java: System.err.println("err")
来源：http://il.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://no.huanxung.cn

Ruby: warn "err"
来源：http://uz.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://lk.szsharing.cn

[M07] 判断是否为主入口
来源：http://mo.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://xm.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xg.hnjuh.cn

JS:   require.main === module
来源：http://ga.jianghongdianzi.cn

TS:   require.main === module
来源：http://qb.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://sx.newstarts.cn

Go:   func main()
来源：http://hl.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wi.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://pl.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://wo.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://iu.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xe.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://qd.shxzukj.cn

TS:   process.platform;  process.version
来源：http://em.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pb.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qb.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rv.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yj.yuexingan06.cn

================================================================================
来源：http://go.lnxyls.cn

N. 数据结构与算法
来源：http://ri.nszjky.cn

================================================================================
来源：http://dc.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://xs.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wu.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sn.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vv.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mr.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://st.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://qa.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ul.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ev.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://og.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://kn.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gc.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://la.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uq.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qs.colortex.cn

Go:   slices.Sort(arr)
来源：http://je.chemitech.net.cn

Ruby: arr.sort
来源：http://iz.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fv.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://cm.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bp.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://nd.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nm.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ja.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bt.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tm.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fx.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://um.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://lu.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oz.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zi.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vh.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xs.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wb.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fs.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ci.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aj.shxzskj.cn

[N05] 最大公约数
来源：http://nl.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://jb.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yr.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ig.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ln.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lj.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fr.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://jl.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ob.lnxyls.cn

[N06] 判断回文字符串
来源：http://sj.jctech888.com.cn

Py:   s == s[::-1]
来源：http://sv.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://nl.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://gz.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://qh.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mw.521024.cn

Go:   // 双指针从两端比较
来源：http://ew.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ni.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gx.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://zj.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uc.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gg.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kd.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://xp.gzmigu.cn

Java: // 手写 HashMap
来源：http://xq.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://tc.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ar.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nc.nszjky.cn

[N08] 生成全排列
来源：http://pz.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://fs.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://hy.szsharing.cn

JS:   // 手写回溯递归
来源：http://hv.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://mk.szsharing.cn

Java: // 手写回溯递归
来源：http://fb.szxytkj.cn

Go:   // 手写回溯递归
来源：http://gv.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://wf.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://xi.haigaiapp.cn

[N09] 栈与队列
来源：http://qh.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jm.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tz.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qe.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uh.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sl.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zq.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ot.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tw.wgjwhj.cn

[N10] 链表节点定义
来源：http://be.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hr.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pj.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://km.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xk.asd995.cn

Java: class Node { int v; Node next; }
来源：http://cy.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fg.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://al.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qu.9csxet.cn

[N11] 二叉树中序遍历
来源：http://kh.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sb.newstarts.cn

PHP:  // 手写递归函数
来源：http://dd.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vh.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cg.shxzskj.cn

Java: // 手写递归
来源：http://zj.shxzskj.cn

Go:   // 手写递归
来源：http://xs.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://td.newstarts.cn

C#:   // 手写递归
来源：http://ot.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ie.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ne.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kk.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qk.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ul.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ys.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yi.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ue.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pe.bjjhwx.cn

================================================================================
来源：http://bj.wgjwhj.cn

O. 并发与异步
来源：http://op.yuexingan06.cn

================================================================================
来源：http://qb.szsharing.cn

[O01] 启动一个线程
来源：http://lx.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ih.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uf.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cy.chemitech.net.cn

TS:   // 同 JS
来源：http://kq.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://kg.jianghongdianzi.cn

Go:   go f()
来源：http://rs.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://gq.szsharing.cn

C#:   Task.Run(() => F());
来源：http://sc.521024.cn

[O02] 使用线程池
来源：http://lz.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dh.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sh.9csxet.cn

JS:   // worker_threads 线程池
来源：http://cs.colortex.cn

TS:   // worker_threads 线程池
来源：http://he.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bl.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bf.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hf.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pg.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://dv.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://ty.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://ou.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ol.huanxung.cn

TS:   // 同 JS
来源：http://wy.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://cz.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://za.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iz.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://xc.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://cr.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://qn.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gj.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://bk.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rt.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ko.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qx.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ng.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://wf.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://mk.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://sk.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rx.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://st.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://yr.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aw.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gc.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ob.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://di.huixinmuqiang.cn

[O06] 使用进程池
来源：http://jq.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oq.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qv.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://ty.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://cv.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pa.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://go.bjjhwx.cn

Ruby: // fork 块
来源：http://kz.nicolike.cn

C#:   Parallel.For
来源：http://jv.bjjhwx.cn

================================================================================
来源：http://nc.muxihuayi.cn

P. 常用工具函数
来源：http://ga.huanxung.cn

================================================================================
来源：http://sa.szxytkj.cn

[P01] 生成 UUID
来源：http://iz.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://za.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kg.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://up.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://sx.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://lu.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://dy.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://pb.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://cl.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://sl.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pf.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uw.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qn.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aj.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qk.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pw.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bf.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mv.asd995.cn

[P03] 生成短随机字符串
来源：http://hd.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nf.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uv.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wu.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rc.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cv.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hm.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bb.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qa.asd995.cn

[P04] 求长度
来源：http://bp.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ki.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bo.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dr.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mp.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://sf.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://bs.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://tp.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nf.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://gk.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wr.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://un.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ao.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rz.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vn.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fa.9csxet.cn

Ruby: a == b
来源：http://cq.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cf.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rs.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ux.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://qf.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cy.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ul.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ru.colortex.cn

Go:   if x == nil {}
来源：http://og.szxytkj.cn


<!-- 参考信息 -->