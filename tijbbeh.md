代发 wailian999

================================================================================
来源：http://iq.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://fj.lnxyls.cn

Py:   sys.argv[1:]
来源：http://fu.szsharing.cn

PHP:  $argv;  $argc;
来源：http://fw.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://tk.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://xx.521024.cn

Java: args 数组（main 方法参数）
来源：http://nb.szxytkj.cn

Go:   os.Args[1:]
来源：http://ur.bookmarksfly.cn

Ruby: ARGV
来源：http://rs.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://nf.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://xs.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://iq.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jb.yuexingan06.cn

JS:   process.env.HOME
来源：http://ig.huanxung.cn

TS:   process.env.HOME
来源：http://sb.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://gg.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xc.521024.cn

Ruby: ENV["HOME"]
来源：http://jz.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jh.shtwfgs.cn

[M03] 执行外部命令
来源：http://ti.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ww.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ed.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tj.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sr.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yj.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hm.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://wp.shxzskj.cn

[M04] 获取当前工作目录
来源：http://hm.chemitech.net.cn

Py:   os.getcwd()
来源：http://in.huixinmuqiang.cn

PHP:  getcwd();
来源：http://km.muxihuayi.cn

JS:   process.cwd()
来源：http://wr.bjjhwx.cn

TS:   process.cwd()
来源：http://oh.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://am.chemitech.net.cn

Go:   os.Getwd()
来源：http://ny.szxytkj.cn

Ruby: Dir.pwd
来源：http://ni.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oj.gzmigu.cn

[M05] 设置退出码
来源：http://dv.521024.cn

Py:   sys.exit(1)
来源：http://fa.wgjwhj.cn

PHP:  exit(1);
来源：http://wc.shxzskj.cn

JS:   process.exit(1)
来源：http://zp.huanxung.cn

TS:   process.exit(1)
来源：http://kv.chemitech.net.cn

Java: System.exit(1)
来源：http://zt.huanxung.cn

Go:   os.Exit(1)
来源：http://xb.muxihuayi.cn

Ruby: exit 1
来源：http://pz.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wy.shxzukj.cn

[M06] 向标准错误输出
来源：http://hq.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://jl.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ny.newstarts.cn

JS:   console.error("err")
来源：http://vo.yuntaijiaju.cn

TS:   console.error("err")
来源：http://oq.jctech888.com.cn

Java: System.err.println("err")
来源：http://gp.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gg.asd995.cn

Ruby: warn "err"
来源：http://cu.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://bo.nszjky.cn

[M07] 判断是否为主入口
来源：http://as.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://tv.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mh.hahajie.cn

JS:   require.main === module
来源：http://uf.haigaiapp.cn

TS:   require.main === module
来源：http://dg.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://rw.shtwfgs.cn

Go:   func main()
来源：http://ua.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xu.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://if.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://pg.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://ip.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://cf.521024.cn

JS:   process.platform;  process.version
来源：http://pl.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://xl.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yo.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ce.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dh.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hv.huixinmuqiang.cn

================================================================================
来源：http://lr.lnxyls.cn

N. 数据结构与算法
来源：http://ql.lnxyls.cn

================================================================================
来源：http://wz.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://ve.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ci.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ov.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://no.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yn.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://is.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ws.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vi.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dh.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://xm.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wl.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ng.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ks.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fd.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qo.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://ik.szxytkj.cn

Ruby: arr.sort
来源：http://pm.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fb.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://bk.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eo.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ny.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dp.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://or.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fq.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qf.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mn.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vh.haigaiapp.cn

[N04] 斐波那契数列
来源：http://dc.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aa.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ou.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rv.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rf.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://su.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zw.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tj.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wy.gzmigu.cn

[N05] 最大公约数
来源：http://vh.newstarts.cn

Py:   math.gcd(a, b)
来源：http://la.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vl.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kr.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cg.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gb.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nf.asd995.cn

Ruby: a.gcd(b)
来源：http://he.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ij.asd995.cn

[N06] 判断回文字符串
来源：http://mt.shxzskj.cn

Py:   s == s[::-1]
来源：http://kw.521024.cn

PHP:  $s === strrev($s);
来源：http://xw.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ra.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://bo.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ng.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://ec.muxihuayi.cn

Ruby: s == s.reverse
来源：http://fb.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ic.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://rh.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://la.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eq.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gg.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://ye.hnjuh.cn

Java: // 手写 HashMap
来源：http://ts.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://uq.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ht.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qy.wgjwhj.cn

[N08] 生成全排列
来源：http://bl.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://xy.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://vj.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://vk.shxzskj.cn

TS:   // 手写回溯递归
来源：http://xe.hahajie.cn

Java: // 手写回溯递归
来源：http://vt.521024.cn

Go:   // 手写回溯递归
来源：http://lg.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://re.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://sp.huixiangedu.cn

[N09] 栈与队列
来源：http://qy.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xg.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wo.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gt.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ky.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://if.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pk.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fe.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yr.chemitech.net.cn

[N10] 链表节点定义
来源：http://mp.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xm.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kv.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kr.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rw.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://zv.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://km.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://us.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qg.hahajie.cn

[N11] 二叉树中序遍历
来源：http://pr.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ry.hahajie.cn

PHP:  // 手写递归函数
来源：http://zh.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ma.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vk.521024.cn

Java: // 手写递归
来源：http://xc.nszjky.cn

Go:   // 手写递归
来源：http://ii.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uw.shxzskj.cn

C#:   // 手写递归
来源：http://vb.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gn.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hu.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iv.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yx.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vf.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wy.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ug.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pc.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hr.panjiajie.cn

================================================================================
来源：http://nk.nicolike.cn

O. 并发与异步
来源：http://bi.nicolike.cn

================================================================================
来源：http://pa.wgjwhj.cn

[O01] 启动一个线程
来源：http://ak.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://px.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bj.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dw.shtwfgs.cn

TS:   // 同 JS
来源：http://se.521024.cn

Java: new Thread(() -> f()).start()
来源：http://ev.huanxung.cn

Go:   go f()
来源：http://ns.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://pj.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://rw.shxzukj.cn

[O02] 使用线程池
来源：http://tb.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cv.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cr.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://jb.hahajie.cn

TS:   // worker_threads 线程池
来源：http://de.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uk.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://av.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qh.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yt.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://zn.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://fh.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://vu.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wl.huanxung.cn

TS:   // 同 JS
来源：http://zn.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://pk.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://at.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ce.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://vt.szsharing.cn

[O04] 定义异步函数并等待
来源：http://mk.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://jw.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ui.huanxung.cn

JS:   async function f() { await g(); }
来源：http://lc.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vf.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uj.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ce.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hu.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://pk.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://zk.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://fl.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://be.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://kb.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://fg.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qx.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yq.nszjky.cn

Ruby: threads.map(&:join)
来源：http://at.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ut.colortex.cn

[O06] 使用进程池
来源：http://lv.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sv.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jx.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://qa.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://dz.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oj.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fc.bookmarksfly.cn

Ruby: // fork 块
来源：http://am.bookmarksfly.cn

C#:   Parallel.For
来源：http://oj.lnxyls.cn

================================================================================
来源：http://ur.gzmigu.cn

P. 常用工具函数
来源：http://pm.shtwfgs.cn

================================================================================
来源：http://wi.hahajie.cn

[P01] 生成 UUID
来源：http://pd.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://el.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xr.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://hx.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://zq.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://ln.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://qc.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://ha.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://pb.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://oo.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mg.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fs.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pw.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rj.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xs.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pi.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sx.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://im.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://bu.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fx.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://db.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gp.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yr.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eq.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sg.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tm.wgjwhj.cn

[P04] 求长度
来源：http://ss.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ut.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://np.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cr.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wn.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://ws.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://vj.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://az.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kt.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://mh.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vo.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ov.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ib.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ht.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qa.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lk.lnxyls.cn

Ruby: a == b
来源：http://hm.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zc.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uy.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://td.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://dd.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iz.haigaiapp.cn

TS:   if (x == null) {}
来源：http://rb.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pe.yuexingan06.cn

Go:   if x == nil {}
来源：http://kh.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nn.huanxung.cn

C#:   if (x is null) {}
来源：http://cu.shxzskj.cn

[P07] 防抖与节流
来源：http://hs.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://av.szxytkj.cn


<!-- 参考信息 -->