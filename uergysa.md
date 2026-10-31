代发 wailian999

================================================================================
来源：http://im.bjjhwx.cn

[M01] 读取命令行参数
来源：http://gt.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://fk.asd995.cn

PHP:  $argv;  $argc;
来源：http://dz.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://wd.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://bj.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://gm.bjjhwx.cn

Go:   os.Args[1:]
来源：http://lv.asd995.cn

Ruby: ARGV
来源：http://ny.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://nb.bookmarksfly.cn

[M02] 读取环境变量
来源：http://zx.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://dt.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://as.gzmigu.cn

JS:   process.env.HOME
来源：http://ar.szsharing.cn

TS:   process.env.HOME
来源：http://id.lnxyls.cn

Java: System.getenv("HOME")
来源：http://zm.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://is.newstarts.cn

Ruby: ENV["HOME"]
来源：http://sv.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lm.lnxyls.cn

[M03] 执行外部命令
来源：http://mr.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vf.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wk.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ii.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oq.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aw.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ww.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qr.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://mr.shxzskj.cn

[M04] 获取当前工作目录
来源：http://et.szxytkj.cn

Py:   os.getcwd()
来源：http://do.muxihuayi.cn

PHP:  getcwd();
来源：http://gb.lnxyls.cn

JS:   process.cwd()
来源：http://qm.shtwfgs.cn

TS:   process.cwd()
来源：http://lj.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://xl.newstarts.cn

Go:   os.Getwd()
来源：http://ii.9csxet.cn

Ruby: Dir.pwd
来源：http://yh.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xk.jctech888.com.cn

[M05] 设置退出码
来源：http://xm.colortex.cn

Py:   sys.exit(1)
来源：http://lu.bjjhwx.cn

PHP:  exit(1);
来源：http://jw.shtwfgs.cn

JS:   process.exit(1)
来源：http://ne.521024.cn

TS:   process.exit(1)
来源：http://gk.nszjky.cn

Java: System.exit(1)
来源：http://tu.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://cv.hnjuh.cn

Ruby: exit 1
来源：http://yx.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xp.jctech888.com.cn

[M06] 向标准错误输出
来源：http://zq.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://id.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lf.bookmarksfly.cn

JS:   console.error("err")
来源：http://fj.nszjky.cn

TS:   console.error("err")
来源：http://sa.huixiangedu.cn

Java: System.err.println("err")
来源：http://ta.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aq.huanxung.cn

Ruby: warn "err"
来源：http://kr.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://kd.nszjky.cn

[M07] 判断是否为主入口
来源：http://vh.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://bp.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dd.wgjwhj.cn

JS:   require.main === module
来源：http://hf.wgjwhj.cn

TS:   require.main === module
来源：http://py.asd995.cn

Java: public static void main(String[] args)
来源：http://ni.huixinmuqiang.cn

Go:   func main()
来源：http://yn.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xx.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://gc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://fo.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://qf.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://vh.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://rs.szxytkj.cn

TS:   process.platform;  process.version
来源：http://vp.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://px.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nd.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nc.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mr.newstarts.cn

================================================================================
来源：http://hj.szsharing.cn

N. 数据结构与算法
来源：http://nj.huixinmuqiang.cn

================================================================================
来源：http://ra.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://iw.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qt.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cd.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qn.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://or.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://js.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://mm.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qf.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://va.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://cm.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://va.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eo.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://th.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zt.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bf.hahajie.cn

Go:   slices.Sort(arr)
来源：http://ch.nicolike.cn

Ruby: arr.sort
来源：http://we.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ha.521024.cn

[N03] 快速排序（分治示例）
来源：http://kh.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ir.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ay.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uz.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kk.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fb.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lc.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ym.lnxyls.cn

[N04] 斐波那契数列
来源：http://lr.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hx.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qo.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hp.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iv.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yy.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nq.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tn.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zs.jianghongdianzi.cn

[N05] 最大公约数
来源：http://tz.colortex.cn

Py:   math.gcd(a, b)
来源：http://jf.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xh.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rt.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qa.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://co.szsharing.cn

Ruby: a.gcd(b)
来源：http://zo.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hs.lnxyls.cn

[N06] 判断回文字符串
来源：http://fe.shtwfgs.cn

Py:   s == s[::-1]
来源：http://se.asd995.cn

PHP:  $s === strrev($s);
来源：http://mn.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://sm.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ce.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bw.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://dv.shtwfgs.cn

Ruby: s == s.reverse
来源：http://jh.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pi.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://pn.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jp.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gl.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ah.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ea.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://on.huanxung.cn

Go:   // 手写 map[int]int
来源：http://vd.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://gy.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bs.shxzskj.cn

[N08] 生成全排列
来源：http://gv.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://pn.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ac.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://tj.colortex.cn

TS:   // 手写回溯递归
来源：http://kq.haigaiapp.cn

Java: // 手写回溯递归
来源：http://zi.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://pc.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://dd.9csxet.cn

C#:   // 手写回溯递归
来源：http://od.521024.cn

[N09] 栈与队列
来源：http://sa.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://me.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zx.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aa.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://au.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://um.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ho.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://te.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vr.gzmigu.cn

[N10] 链表节点定义
来源：http://ob.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qr.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gf.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fr.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kr.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://cf.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://og.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qr.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hj.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ep.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mt.gzmigu.cn

PHP:  // 手写递归函数
来源：http://uc.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://au.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iv.shxzukj.cn

Java: // 手写递归
来源：http://iy.hnjuh.cn

Go:   // 手写递归
来源：http://uq.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qa.bjjhwx.cn

C#:   // 手写递归
来源：http://sg.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ue.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sw.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gw.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fb.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ao.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rw.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zn.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gc.nicolike.cn

================================================================================
来源：http://dt.jianghongdianzi.cn

O. 并发与异步
来源：http://cf.wgjwhj.cn

================================================================================
来源：http://xt.szsharing.cn

[O01] 启动一个线程
来源：http://ej.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ch.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nb.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kk.jianghongdianzi.cn

TS:   // 同 JS
来源：http://jp.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://ws.shxzskj.cn

Go:   go f()
来源：http://ot.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://mx.newstarts.cn

C#:   Task.Run(() => F());
来源：http://yo.asd995.cn

[O02] 使用线程池
来源：http://rq.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rf.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cx.nszjky.cn

JS:   // worker_threads 线程池
来源：http://fr.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://xz.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://py.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zm.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qv.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://py.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://nt.521024.cn

Py:   with lock: shared += 1
来源：http://uc.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://rt.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dy.huanxung.cn

TS:   // 同 JS
来源：http://pi.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://ko.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xv.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://he.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://qe.szsharing.cn

[O04] 定义异步函数并等待
来源：http://cv.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ne.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yz.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://un.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jk.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wb.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hl.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tq.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://pt.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://mn.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://jd.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bk.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ih.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://qp.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iy.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ih.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://xz.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cg.huanxung.cn

[O06] 使用进程池
来源：http://ku.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://is.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qs.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://sr.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://js.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ik.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ic.huixinmuqiang.cn

Ruby: // fork 块
来源：http://nr.wgjwhj.cn

C#:   Parallel.For
来源：http://jo.szxytkj.cn

================================================================================
来源：http://fc.jianghongdianzi.cn

P. 常用工具函数
来源：http://pt.chemitech.net.cn

================================================================================
来源：http://zf.nicolike.cn

[P01] 生成 UUID
来源：http://hr.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://yc.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jb.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://eb.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://pm.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://ud.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://yu.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://nb.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ty.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://jv.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mz.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ky.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://za.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kk.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://am.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cc.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://he.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zi.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://tp.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lp.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fm.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yg.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mv.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oq.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ig.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://so.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tz.9csxet.cn

[P04] 求长度
来源：http://nz.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cn.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fk.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ko.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kq.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://iv.newstarts.cn

Go:   len(arr);  len(m)
来源：http://vx.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://cf.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lw.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://tm.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rz.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ot.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mx.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kg.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dc.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uz.gzmigu.cn

Ruby: a == b
来源：http://ax.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ia.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yk.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jd.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://ap.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iy.muxihuayi.cn

TS:   if (x == null) {}
来源：http://hy.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nn.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://sf.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lx.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ud.asd995.cn

[P07] 防抖与节流
来源：http://dt.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ve.shtwfgs.cn


<!-- 参考信息 -->