代发 wailian999

================================================================================
来源：http://pu.yuexingan06.cn

[M01] 读取命令行参数
来源：http://tx.521024.cn

Py:   sys.argv[1:]
来源：http://ur.hahajie.cn

PHP:  $argv;  $argc;
来源：http://qf.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://kq.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://jo.asd995.cn

Java: args 数组（main 方法参数）
来源：http://xo.shxzukj.cn

Go:   os.Args[1:]
来源：http://ol.asd995.cn

Ruby: ARGV
来源：http://hc.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://kh.muxihuayi.cn

[M02] 读取环境变量
来源：http://ed.asd995.cn

Py:   os.environ.get("HOME")
来源：http://jp.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lh.huixiangedu.cn

JS:   process.env.HOME
来源：http://mc.gzmigu.cn

TS:   process.env.HOME
来源：http://dw.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ed.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xq.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://vn.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pk.yuexingan06.cn

[M03] 执行外部命令
来源：http://xg.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fg.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://su.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lq.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mj.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rm.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hh.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cj.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://sf.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://vu.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://xz.newstarts.cn

PHP:  getcwd();
来源：http://cz.wgjwhj.cn

JS:   process.cwd()
来源：http://nb.9csxet.cn

TS:   process.cwd()
来源：http://wl.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://sv.wgjwhj.cn

Go:   os.Getwd()
来源：http://nh.bjjhwx.cn

Ruby: Dir.pwd
来源：http://sp.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sr.shtwfgs.cn

[M05] 设置退出码
来源：http://mb.nicolike.cn

Py:   sys.exit(1)
来源：http://jx.huanxung.cn

PHP:  exit(1);
来源：http://kq.hahajie.cn

JS:   process.exit(1)
来源：http://cp.hnjuh.cn

TS:   process.exit(1)
来源：http://zf.huixinmuqiang.cn

Java: System.exit(1)
来源：http://tb.shxzskj.cn

Go:   os.Exit(1)
来源：http://ly.9csxet.cn

Ruby: exit 1
来源：http://pz.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qz.asd995.cn

[M06] 向标准错误输出
来源：http://eh.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://ow.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ff.lnxyls.cn

JS:   console.error("err")
来源：http://xc.shtwfgs.cn

TS:   console.error("err")
来源：http://wo.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://ye.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ni.nicolike.cn

Ruby: warn "err"
来源：http://bd.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://sn.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://qa.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://hb.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ai.gzmigu.cn

JS:   require.main === module
来源：http://ip.yuexingan06.cn

TS:   require.main === module
来源：http://bd.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://le.shxzskj.cn

Go:   func main()
来源：http://ac.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sj.colortex.cn

C#:   static void Main(string[] args)
来源：http://lb.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://ek.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://ah.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://zt.hnjuh.cn

JS:   process.platform;  process.version
来源：http://ri.lnxyls.cn

TS:   process.platform;  process.version
来源：http://rm.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ij.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ky.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://od.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ot.colortex.cn

================================================================================
来源：http://mx.jianghongdianzi.cn

N. 数据结构与算法
来源：http://xa.nicolike.cn

================================================================================
来源：http://vx.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://dc.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nb.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://os.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rk.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ep.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wy.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://iv.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pi.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yv.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://wv.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bi.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ga.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yi.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ft.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://zz.hahajie.cn

Ruby: arr.sort
来源：http://ik.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sx.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://aj.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gu.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://je.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jn.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tx.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rw.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qa.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qf.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ox.chemitech.net.cn

[N04] 斐波那契数列
来源：http://av.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zj.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wc.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mo.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kk.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jo.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bq.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://op.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wi.shtwfgs.cn

[N05] 最大公约数
来源：http://co.huanxung.cn

Py:   math.gcd(a, b)
来源：http://lr.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dn.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bv.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dn.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qc.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oa.hahajie.cn

Ruby: a.gcd(b)
来源：http://vi.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ty.szxytkj.cn

[N06] 判断回文字符串
来源：http://ch.hahajie.cn

Py:   s == s[::-1]
来源：http://nk.newstarts.cn

PHP:  $s === strrev($s);
来源：http://dr.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ft.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://qi.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ih.521024.cn

Go:   // 双指针从两端比较
来源：http://em.huixiangedu.cn

Ruby: s == s.reverse
来源：http://jz.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://br.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://jq.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://id.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qs.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wr.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://bc.shxzskj.cn

Java: // 手写 HashMap
来源：http://bg.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://xl.szxytkj.cn

Ruby: // 手写 Hash
来源：http://yc.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kj.szsharing.cn

[N08] 生成全排列
来源：http://mf.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://yz.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://ji.newstarts.cn

JS:   // 手写回溯递归
来源：http://ge.hahajie.cn

TS:   // 手写回溯递归
来源：http://lj.szsharing.cn

Java: // 手写回溯递归
来源：http://ko.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://bt.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://dx.lnxyls.cn

C#:   // 手写回溯递归
来源：http://kx.huixinmuqiang.cn

[N09] 栈与队列
来源：http://cs.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vf.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zl.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vt.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ay.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://at.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://id.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://er.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hk.szxytkj.cn

[N10] 链表节点定义
来源：http://zw.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hw.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wj.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ad.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://td.521024.cn

Java: class Node { int v; Node next; }
来源：http://rx.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uw.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sz.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cj.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://pn.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://md.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://zn.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://du.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gk.szxytkj.cn

Java: // 手写递归
来源：http://cj.chemitech.net.cn

Go:   // 手写递归
来源：http://xx.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kt.521024.cn

C#:   // 手写递归
来源：http://dp.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ba.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rl.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iz.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kz.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ol.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tr.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bj.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mf.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vo.asd995.cn

================================================================================
来源：http://si.yuexingan06.cn

O. 并发与异步
来源：http://dv.newstarts.cn

================================================================================
来源：http://px.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://fv.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xo.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rc.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qm.shxzskj.cn

TS:   // 同 JS
来源：http://va.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://ux.muxihuayi.cn

Go:   go f()
来源：http://an.asd995.cn

Ruby: Thread.new { f }
来源：http://xz.colortex.cn

C#:   Task.Run(() => F());
来源：http://wf.shxzskj.cn

[O02] 使用线程池
来源：http://rs.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aw.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zj.9csxet.cn

JS:   // worker_threads 线程池
来源：http://ws.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://uj.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pe.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yk.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vq.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kq.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://pp.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://zp.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://wm.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ob.shtwfgs.cn

TS:   // 同 JS
来源：http://fd.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://dj.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zz.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jw.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://al.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://bd.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://rp.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://te.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://xo.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bh.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hv.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eg.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lz.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://vg.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://kf.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://ju.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eu.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://vx.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://tv.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kq.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yl.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ci.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bm.chemitech.net.cn

[O06] 使用进程池
来源：http://fc.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tz.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dd.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://vt.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://gg.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vk.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://so.colortex.cn

Ruby: // fork 块
来源：http://pb.hahajie.cn

C#:   Parallel.For
来源：http://fd.521024.cn

================================================================================
来源：http://qz.bjjhwx.cn

P. 常用工具函数
来源：http://vu.shxzukj.cn

================================================================================
来源：http://ll.muxihuayi.cn

[P01] 生成 UUID
来源：http://eu.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://hk.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bp.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://dg.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://la.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://hw.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://gq.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://il.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://ue.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://yv.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://in.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eg.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mq.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gi.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ug.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rf.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kz.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xw.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://pb.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ii.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ag.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vi.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ce.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yh.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ck.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zj.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hp.jianghongdianzi.cn

[P04] 求长度
来源：http://hr.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ku.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://si.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qs.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lg.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://cu.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://qw.lnxyls.cn

Ruby: x.length;  x.size
来源：http://rp.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yx.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://mr.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://by.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ve.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://if.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gh.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tu.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pu.shxzskj.cn

Ruby: a == b
来源：http://qh.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eq.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ph.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ij.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://dm.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ox.shxzskj.cn

TS:   if (x == null) {}
来源：http://vn.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gt.bjjhwx.cn

Go:   if x == nil {}
来源：http://va.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nm.huixiangedu.cn

C#:   if (x is null) {}
来源：http://ba.newstarts.cn

[P07] 防抖与节流
来源：http://kc.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ym.gzmigu.cn


<!-- 参考信息 -->