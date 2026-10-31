代发 wailian999

================================================================================
来源：http://my.hnjuh.cn

[M01] 读取命令行参数
来源：http://qj.9csxet.cn

Py:   sys.argv[1:]
来源：http://mm.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://dy.9csxet.cn

JS:   process.argv.slice(2)
来源：http://yu.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://pj.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://fa.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://vj.nicolike.cn

Ruby: ARGV
来源：http://so.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://rw.panjiajie.cn

[M02] 读取环境变量
来源：http://yk.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://uc.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hh.wgjwhj.cn

JS:   process.env.HOME
来源：http://ro.yuexingan06.cn

TS:   process.env.HOME
来源：http://xy.nicolike.cn

Java: System.getenv("HOME")
来源：http://gr.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gx.huanxung.cn

Ruby: ENV["HOME"]
来源：http://oy.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sk.muxihuayi.cn

[M03] 执行外部命令
来源：http://dw.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ze.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eq.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hm.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ss.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gz.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sm.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dh.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://je.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://pn.521024.cn

Py:   os.getcwd()
来源：http://bq.yuexingan06.cn

PHP:  getcwd();
来源：http://yw.huanxung.cn

JS:   process.cwd()
来源：http://au.shtwfgs.cn

TS:   process.cwd()
来源：http://my.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://lc.panjiajie.cn

Go:   os.Getwd()
来源：http://ql.szxytkj.cn

Ruby: Dir.pwd
来源：http://jm.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ri.colortex.cn

[M05] 设置退出码
来源：http://gi.lnxyls.cn

Py:   sys.exit(1)
来源：http://hs.yuexingan06.cn

PHP:  exit(1);
来源：http://hx.colortex.cn

JS:   process.exit(1)
来源：http://ot.gzmigu.cn

TS:   process.exit(1)
来源：http://qd.panjiajie.cn

Java: System.exit(1)
来源：http://vr.huixiangedu.cn

Go:   os.Exit(1)
来源：http://yw.yuexingan06.cn

Ruby: exit 1
来源：http://th.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ax.hnjuh.cn

[M06] 向标准错误输出
来源：http://zl.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://mg.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pd.lnxyls.cn

JS:   console.error("err")
来源：http://sx.panjiajie.cn

TS:   console.error("err")
来源：http://la.yuexingan06.cn

Java: System.err.println("err")
来源：http://hk.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kl.nszjky.cn

Ruby: warn "err"
来源：http://vw.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://zz.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://rn.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://qb.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fl.shxzukj.cn

JS:   require.main === module
来源：http://uk.shxzukj.cn

TS:   require.main === module
来源：http://aa.colortex.cn

Java: public static void main(String[] args)
来源：http://bg.szxytkj.cn

Go:   func main()
来源：http://ta.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cc.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://jm.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://qv.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://rx.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://bu.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://pv.shxzskj.cn

TS:   process.platform;  process.version
来源：http://un.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bz.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wu.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mf.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ye.jctech888.com.cn

================================================================================
来源：http://ov.9csxet.cn

N. 数据结构与算法
来源：http://nx.521024.cn

================================================================================
来源：http://zt.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://ys.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qy.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ho.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ib.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kh.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wl.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ek.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jz.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gh.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://ce.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://rh.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ty.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ss.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nt.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://md.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://wd.huixinmuqiang.cn

Ruby: arr.sort
来源：http://md.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dz.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://wp.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://si.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://gl.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fk.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://em.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fs.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bm.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qq.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ld.huixiangedu.cn

[N04] 斐波那契数列
来源：http://er.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bm.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fe.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hr.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://he.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ed.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rc.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lo.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://du.nszjky.cn

[N05] 最大公约数
来源：http://ag.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://uz.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pk.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://re.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gf.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sx.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://se.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://gj.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yn.muxihuayi.cn

[N06] 判断回文字符串
来源：http://vo.shxzukj.cn

Py:   s == s[::-1]
来源：http://pm.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://ly.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://qh.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://rn.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ex.nicolike.cn

Go:   // 双指针从两端比较
来源：http://nw.szxytkj.cn

Ruby: s == s.reverse
来源：http://nm.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tq.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://ut.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hx.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fg.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sp.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://qm.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://xg.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://bm.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://mh.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uq.nicolike.cn

[N08] 生成全排列
来源：http://ex.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://fw.asd995.cn

PHP:  // 手写递归交换
来源：http://aw.szsharing.cn

JS:   // 手写回溯递归
来源：http://gl.521024.cn

TS:   // 手写回溯递归
来源：http://ma.nszjky.cn

Java: // 手写回溯递归
来源：http://ky.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://xz.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://pi.hnjuh.cn

C#:   // 手写回溯递归
来源：http://mz.panjiajie.cn

[N09] 栈与队列
来源：http://tp.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lr.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ji.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mh.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fp.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://av.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rf.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fg.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vs.chemitech.net.cn

[N10] 链表节点定义
来源：http://uq.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uz.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qz.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bj.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gr.colortex.cn

Java: class Node { int v; Node next; }
来源：http://hg.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fd.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lb.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ic.hahajie.cn

[N11] 二叉树中序遍历
来源：http://pp.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vl.gzmigu.cn

PHP:  // 手写递归函数
来源：http://rv.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wv.nicolike.cn

Java: // 手写递归
来源：http://sm.shtwfgs.cn

Go:   // 手写递归
来源：http://cd.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pa.huanxung.cn

C#:   // 手写递归
来源：http://ad.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xk.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pj.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jz.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kv.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vp.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yw.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ea.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xk.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pk.chemitech.net.cn

================================================================================
来源：http://uc.gzmigu.cn

O. 并发与异步
来源：http://qf.hahajie.cn

================================================================================
来源：http://rn.yuexingan06.cn

[O01] 启动一个线程
来源：http://yb.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://el.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ml.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ww.panjiajie.cn

TS:   // 同 JS
来源：http://oi.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://cf.asd995.cn

Go:   go f()
来源：http://rr.shxzukj.cn

Ruby: Thread.new { f }
来源：http://nb.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://oj.jianghongdianzi.cn

[O02] 使用线程池
来源：http://kf.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kv.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oi.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://bz.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://et.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yr.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hv.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qq.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fe.colortex.cn

[O03] 加锁保护共享数据
来源：http://aa.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://xm.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ad.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yz.shtwfgs.cn

TS:   // 同 JS
来源：http://lc.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://oq.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lk.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wr.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://ot.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://oy.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://zl.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ja.colortex.cn

JS:   async function f() { await g(); }
来源：http://hg.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vg.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xk.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mn.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cg.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://es.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://vp.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://cf.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dm.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://mt.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://xj.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qt.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xw.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://zx.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vs.hahajie.cn

[O06] 使用进程池
来源：http://xf.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ey.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cj.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://yb.521024.cn

TS:   // child_process / cluster 模块
来源：http://kv.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ot.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wu.shxzukj.cn

Ruby: // fork 块
来源：http://dm.yuntaijiaju.cn

C#:   Parallel.For
来源：http://vk.nszjky.cn

================================================================================
来源：http://cx.9csxet.cn

P. 常用工具函数
来源：http://rg.lnxyls.cn

================================================================================
来源：http://pf.jctech888.com.cn

[P01] 生成 UUID
来源：http://wv.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://yi.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xc.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://rb.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://vu.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://vc.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://kv.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://xi.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://qp.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://rx.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ny.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vt.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wa.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wc.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nj.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jg.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bs.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zt.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://qm.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://om.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uq.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bq.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yz.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jh.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ma.wgjwhj.cn

[P04] 求长度
来源：http://kc.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zr.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://au.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rh.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ew.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://dr.colortex.cn

Go:   len(arr);  len(m)
来源：http://ob.9csxet.cn

Ruby: x.length;  x.size
来源：http://rq.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xp.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://hn.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xt.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lz.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qo.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ha.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gr.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ve.szxytkj.cn

Ruby: a == b
来源：http://dz.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cy.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gr.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gk.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://os.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mf.wgjwhj.cn

TS:   if (x == null) {}
来源：http://po.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bn.shtwfgs.cn

Go:   if x == nil {}
来源：http://dh.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fu.shxzskj.cn

C#:   if (x is null) {}
来源：http://ch.gzmigu.cn

[P07] 防抖与节流
来源：http://ui.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wu.newstarts.cn


<!-- 参考信息 -->