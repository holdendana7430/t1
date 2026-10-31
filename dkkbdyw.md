代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uw.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nd.hahajie.cn

================================================================================
来源：http://pi.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://rz.colortex.cn

================================================================================
来源：http://bn.hahajie.cn

[M01] 读取命令行参数
来源：http://jo.nicolike.cn

Py:   sys.argv[1:]
来源：http://my.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://ch.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://zt.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://vo.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://gm.chemitech.net.cn

Go:   os.Args[1:]
来源：http://ju.wgjwhj.cn

Ruby: ARGV
来源：http://pi.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://bi.szsharing.cn

[M02] 读取环境变量
来源：http://nu.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://ze.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dj.nszjky.cn

JS:   process.env.HOME
来源：http://mq.haigaiapp.cn

TS:   process.env.HOME
来源：http://zx.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://li.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yi.hahajie.cn

Ruby: ENV["HOME"]
来源：http://qr.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xt.yuexingan06.cn

[M03] 执行外部命令
来源：http://dm.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hd.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://id.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ct.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ul.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://md.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://er.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kn.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://jt.hahajie.cn

[M04] 获取当前工作目录
来源：http://yq.huanxung.cn

Py:   os.getcwd()
来源：http://tr.nicolike.cn

PHP:  getcwd();
来源：http://mq.szxytkj.cn

JS:   process.cwd()
来源：http://zz.nicolike.cn

TS:   process.cwd()
来源：http://nn.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://mi.bookmarksfly.cn

Go:   os.Getwd()
来源：http://hv.colortex.cn

Ruby: Dir.pwd
来源：http://gw.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hv.yuntaijiaju.cn

[M05] 设置退出码
来源：http://km.lnxyls.cn

Py:   sys.exit(1)
来源：http://kl.newstarts.cn

PHP:  exit(1);
来源：http://du.gzmigu.cn

JS:   process.exit(1)
来源：http://mx.gzmigu.cn

TS:   process.exit(1)
来源：http://id.gzmigu.cn

Java: System.exit(1)
来源：http://ph.hahajie.cn

Go:   os.Exit(1)
来源：http://uw.wgjwhj.cn

Ruby: exit 1
来源：http://mw.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pu.gzmigu.cn

[M06] 向标准错误输出
来源：http://zx.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://la.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pt.shtwfgs.cn

JS:   console.error("err")
来源：http://yd.bjjhwx.cn

TS:   console.error("err")
来源：http://cd.bookmarksfly.cn

Java: System.err.println("err")
来源：http://dx.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vj.jianghongdianzi.cn

Ruby: warn "err"
来源：http://tt.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://eo.hahajie.cn

[M07] 判断是否为主入口
来源：http://ev.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://vi.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ls.hahajie.cn

JS:   require.main === module
来源：http://pt.szxytkj.cn

TS:   require.main === module
来源：http://tv.hahajie.cn

Java: public static void main(String[] args)
来源：http://lx.jctech888.com.cn

Go:   func main()
来源：http://as.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hr.9csxet.cn

C#:   static void Main(string[] args)
来源：http://og.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://fq.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ym.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://pu.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://fz.hahajie.cn

TS:   process.platform;  process.version
来源：http://qt.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pw.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://da.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uo.huixiangedu.cn

================================================================================
来源：http://rh.jctech888.com.cn

N. 数据结构与算法
来源：http://gf.yuntaijiaju.cn

================================================================================
来源：http://hs.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://jr.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zt.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xf.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uf.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bn.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fn.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://vf.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ba.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pd.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://tf.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ri.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vr.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ky.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jz.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.asd995.cn

Go:   slices.Sort(arr)
来源：http://dd.muxihuayi.cn

Ruby: arr.sort
来源：http://lh.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xq.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://jk.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ev.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://rz.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fw.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ea.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xo.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zs.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://br.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fn.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://te.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mp.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://em.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fl.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iu.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ad.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pl.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://th.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nk.chemitech.net.cn

[N05] 最大公约数
来源：http://sn.asd995.cn

Py:   math.gcd(a, b)
来源：http://tc.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cc.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pm.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jh.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kk.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yv.panjiajie.cn

Ruby: a.gcd(b)
来源：http://dh.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aq.colortex.cn

[N06] 判断回文字符串
来源：http://dl.haigaiapp.cn

Py:   s == s[::-1]
来源：http://lw.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ve.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://sa.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://cm.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jk.521024.cn

Go:   // 双指针从两端比较
来源：http://mn.bjjhwx.cn

Ruby: s == s.reverse
来源：http://fl.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wz.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://ta.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cs.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jo.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mz.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://uh.shxzukj.cn

Java: // 手写 HashMap
来源：http://an.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://pz.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://ws.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sl.bookmarksfly.cn

[N08] 生成全排列
来源：http://vv.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ma.szxytkj.cn

PHP:  // 手写递归交换
来源：http://ml.nicolike.cn

JS:   // 手写回溯递归
来源：http://ct.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://xo.hnjuh.cn

Java: // 手写回溯递归
来源：http://wg.panjiajie.cn

Go:   // 手写回溯递归
来源：http://ag.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://gh.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://vq.shtwfgs.cn

[N09] 栈与队列
来源：http://dg.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hm.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cr.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mj.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xb.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://md.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mf.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://di.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://um.chemitech.net.cn

[N10] 链表节点定义
来源：http://vl.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jd.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hk.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ww.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ks.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://sk.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ac.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mx.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rv.521024.cn

[N11] 二叉树中序遍历
来源：http://fm.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rq.shxzukj.cn

PHP:  // 手写递归函数
来源：http://wk.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kg.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pv.szsharing.cn

Java: // 手写递归
来源：http://yy.huanxung.cn

Go:   // 手写递归
来源：http://wk.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ne.bookmarksfly.cn

C#:   // 手写递归
来源：http://yh.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sg.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gc.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mf.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cd.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cg.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iy.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vp.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cb.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qi.gzmigu.cn

================================================================================
来源：http://nl.hahajie.cn

O. 并发与异步
来源：http://zr.asd995.cn

================================================================================
来源：http://ga.colortex.cn

[O01] 启动一个线程
来源：http://jm.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ws.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://di.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dv.521024.cn

TS:   // 同 JS
来源：http://so.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://ii.shxzukj.cn

Go:   go f()
来源：http://im.lnxyls.cn

Ruby: Thread.new { f }
来源：http://xx.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://vu.szsharing.cn

[O02] 使用线程池
来源：http://eh.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qw.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://af.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://mm.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://nt.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hu.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fj.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nd.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yg.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://kt.szxytkj.cn

Py:   with lock: shared += 1
来源：http://uc.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://cj.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aa.bjjhwx.cn

TS:   // 同 JS
来源：http://ac.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://cy.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sk.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ud.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://ly.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://ef.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://tw.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ut.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://ry.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hu.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hs.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mj.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aa.colortex.cn

C#:   async Task F() { await G(); }
来源：http://ey.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://ck.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://ph.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nm.521024.cn

JS:   await Promise.all(tasks)
来源：http://ib.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://dv.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bh.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ez.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ka.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://od.szsharing.cn

[O06] 使用进程池
来源：http://tw.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nt.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zc.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://cl.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://rz.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fr.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eb.szxytkj.cn

Ruby: // fork 块
来源：http://em.lnxyls.cn

C#:   Parallel.For
来源：http://pm.muxihuayi.cn

================================================================================
来源：http://uz.jianghongdianzi.cn

P. 常用工具函数
来源：http://qn.asd995.cn

================================================================================
来源：http://ik.colortex.cn

[P01] 生成 UUID
来源：http://cn.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://hj.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://za.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://fj.newstarts.cn

TS:   crypto.randomUUID()
来源：http://zp.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://oa.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://ki.521024.cn

Ruby: SecureRandom.uuid
来源：http://td.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://py.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://go.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uc.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nz.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uv.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nt.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dg.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pm.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yh.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yt.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://xj.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vv.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wb.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://li.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lq.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jd.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nn.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ef.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qm.nicolike.cn

[P04] 求长度
来源：http://ci.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://es.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sg.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cf.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kt.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://cc.newstarts.cn

Go:   len(arr);  len(m)
来源：http://dl.hnjuh.cn

Ruby: x.length;  x.size
来源：http://jv.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pe.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://ym.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kc.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iz.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ze.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jy.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qe.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vu.colortex.cn

Ruby: a == b
来源：http://nn.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lp.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ie.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yk.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://ag.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://py.hnjuh.cn

TS:   if (x == null) {}
来源：http://da.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ie.jctech888.com.cn

Go:   if x == nil {}
来源：http://bb.newstarts.cn


<!-- 参考信息 -->