代发 wailian999

================================================================================
来源：http://rv.colortex.cn

[M01] 读取命令行参数
来源：http://kk.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://jr.hahajie.cn

PHP:  $argv;  $argc;
来源：http://lz.asd995.cn

JS:   process.argv.slice(2)
来源：http://fu.colortex.cn

TS:   process.argv.slice(2)
来源：http://er.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://cn.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://os.jctech888.com.cn

Ruby: ARGV
来源：http://ak.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://pm.gzmigu.cn

[M02] 读取环境变量
来源：http://yj.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://mc.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zg.hnjuh.cn

JS:   process.env.HOME
来源：http://gn.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://dx.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://gz.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xb.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ow.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ay.nicolike.cn

[M03] 执行外部命令
来源：http://yf.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jj.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://le.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://il.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jp.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://su.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aw.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://ne.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://gj.gzmigu.cn

Py:   os.getcwd()
来源：http://pa.shxzskj.cn

PHP:  getcwd();
来源：http://nd.bjjhwx.cn

JS:   process.cwd()
来源：http://go.bjjhwx.cn

TS:   process.cwd()
来源：http://sb.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://wf.521024.cn

Go:   os.Getwd()
来源：http://up.lnxyls.cn

Ruby: Dir.pwd
来源：http://db.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jg.chemitech.net.cn

[M05] 设置退出码
来源：http://uv.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://rr.yuexingan06.cn

PHP:  exit(1);
来源：http://eb.9csxet.cn

JS:   process.exit(1)
来源：http://pn.521024.cn

TS:   process.exit(1)
来源：http://gd.yuntaijiaju.cn

Java: System.exit(1)
来源：http://mt.szxytkj.cn

Go:   os.Exit(1)
来源：http://vb.haigaiapp.cn

Ruby: exit 1
来源：http://jk.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gx.colortex.cn

[M06] 向标准错误输出
来源：http://jy.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://se.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gi.shxzukj.cn

JS:   console.error("err")
来源：http://ul.hahajie.cn

TS:   console.error("err")
来源：http://cf.bjjhwx.cn

Java: System.err.println("err")
来源：http://xn.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cx.newstarts.cn

Ruby: warn "err"
来源：http://ar.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ib.hnjuh.cn

[M07] 判断是否为主入口
来源：http://mi.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://ks.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://td.gzmigu.cn

JS:   require.main === module
来源：http://ky.newstarts.cn

TS:   require.main === module
来源：http://xn.colortex.cn

Java: public static void main(String[] args)
来源：http://zk.bjjhwx.cn

Go:   func main()
来源：http://bx.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vx.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://tj.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://pb.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://yd.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://hq.hahajie.cn

JS:   process.platform;  process.version
来源：http://fb.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://ut.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kb.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ai.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vy.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fu.hnjuh.cn

================================================================================
来源：http://fn.szsharing.cn

N. 数据结构与算法
来源：http://fe.huanxung.cn

================================================================================
来源：http://xr.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://vz.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xh.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pf.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iy.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wv.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yh.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://sj.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fp.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nf.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://ho.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rv.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ny.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gx.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://md.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://da.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://cl.asd995.cn

Ruby: arr.sort
来源：http://ww.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://um.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://vo.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ks.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ys.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yj.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tc.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sn.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qe.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cy.nszjky.cn

[N04] 斐波那契数列
来源：http://vp.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pb.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gu.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gs.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pe.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yw.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tq.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zp.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lk.lnxyls.cn

[N05] 最大公约数
来源：http://ar.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://xw.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://na.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uh.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xv.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uq.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zw.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://md.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://va.shtwfgs.cn

[N06] 判断回文字符串
来源：http://tn.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://oy.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ek.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://wn.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ug.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qu.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://dh.9csxet.cn

Ruby: s == s.reverse
来源：http://lg.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ue.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://gg.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ss.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sn.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mj.521024.cn

TS:   // 手写 Map<string, number>
来源：http://so.asd995.cn

Java: // 手写 HashMap
来源：http://pg.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://zf.huanxung.cn

Ruby: // 手写 Hash
来源：http://iy.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bs.shxzukj.cn

[N08] 生成全排列
来源：http://aa.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://qe.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://ka.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://js.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ij.panjiajie.cn

Java: // 手写回溯递归
来源：http://xk.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://pg.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://qr.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://jq.szsharing.cn

[N09] 栈与队列
来源：http://id.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ge.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iy.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dh.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cu.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gg.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xr.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ne.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nw.huixiangedu.cn

[N10] 链表节点定义
来源：http://dp.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ap.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xa.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tb.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wq.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://ym.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kv.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ny.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oc.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://yy.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://di.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://bw.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vy.gzmigu.cn

Java: // 手写递归
来源：http://kd.szsharing.cn

Go:   // 手写递归
来源：http://qa.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wa.hnjuh.cn

C#:   // 手写递归
来源：http://ai.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ww.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ou.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oi.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dk.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wm.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mf.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ao.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nz.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wd.9csxet.cn

================================================================================
来源：http://bt.yuntaijiaju.cn

O. 并发与异步
来源：http://wk.colortex.cn

================================================================================
来源：http://xw.muxihuayi.cn

[O01] 启动一个线程
来源：http://dt.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ku.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ez.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iu.chemitech.net.cn

TS:   // 同 JS
来源：http://oi.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://rd.nszjky.cn

Go:   go f()
来源：http://ut.nszjky.cn

Ruby: Thread.new { f }
来源：http://ng.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://ge.hnjuh.cn

[O02] 使用线程池
来源：http://ft.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lg.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yt.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://lw.huanxung.cn

TS:   // worker_threads 线程池
来源：http://zr.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dj.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ce.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://me.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ox.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://kw.colortex.cn

Py:   with lock: shared += 1
来源：http://xu.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://od.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sn.shxzskj.cn

TS:   // 同 JS
来源：http://yr.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://xq.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ak.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tf.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://zs.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://kf.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://dk.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sv.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://zv.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bp.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mv.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bz.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uk.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://dz.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://hj.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://ej.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jv.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://hu.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://wz.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pn.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ic.hahajie.cn

Ruby: threads.map(&:join)
来源：http://um.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pr.chemitech.net.cn

[O06] 使用进程池
来源：http://jk.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sc.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nc.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://ns.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://mk.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dl.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yy.szxytkj.cn

Ruby: // fork 块
来源：http://gm.nszjky.cn

C#:   Parallel.For
来源：http://ef.hnjuh.cn

================================================================================
来源：http://pp.colortex.cn

P. 常用工具函数
来源：http://ev.huixinmuqiang.cn

================================================================================
来源：http://ib.hahajie.cn

[P01] 生成 UUID
来源：http://pj.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://sg.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wx.colortex.cn

JS:   crypto.randomUUID()
来源：http://xf.9csxet.cn

TS:   crypto.randomUUID()
来源：http://op.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://mb.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://zo.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://bs.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://vo.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://sx.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ab.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iv.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oe.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kk.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pu.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ag.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tx.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://na.asd995.cn

[P03] 生成短随机字符串
来源：http://xo.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jy.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cq.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pt.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wx.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lf.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xa.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://df.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wh.bjjhwx.cn

[P04] 求长度
来源：http://ts.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://na.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jr.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qg.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://te.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://te.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://ik.panjiajie.cn

Ruby: x.length;  x.size
来源：http://hv.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eq.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://te.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hu.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wa.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://he.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lq.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wy.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eb.521024.cn

Ruby: a == b
来源：http://rh.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ss.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://th.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ym.521024.cn

PHP:  if (empty($x)) {}
来源：http://ye.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://no.9csxet.cn

TS:   if (x == null) {}
来源：http://mm.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cx.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://yt.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ds.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://sf.shtwfgs.cn

[P07] 防抖与节流
来源：http://xq.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gb.jianghongdianzi.cn


<!-- 参考信息 -->