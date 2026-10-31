代发 wailian999

C#:   (int)resp.StatusCode
来源：http://qh.panjiajie.cn

[L08] 并发请求多个地址
来源：http://mh.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ly.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://zz.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kj.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://je.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ww.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kh.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tg.wgjwhj.cn

================================================================================
来源：http://bc.521024.cn

M. 命令行 / 进程 / 环境
来源：http://pg.szsharing.cn

================================================================================
来源：http://mn.shxzskj.cn

[M01] 读取命令行参数
来源：http://ow.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://zn.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://aw.colortex.cn

JS:   process.argv.slice(2)
来源：http://zc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://gd.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://va.shxzskj.cn

Go:   os.Args[1:]
来源：http://sp.nicolike.cn

Ruby: ARGV
来源：http://qd.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ec.yuexingan06.cn

[M02] 读取环境变量
来源：http://wx.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://gz.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jo.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://xe.hnjuh.cn

TS:   process.env.HOME
来源：http://ik.521024.cn

Java: System.getenv("HOME")
来源：http://dq.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rq.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://zs.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kx.shtwfgs.cn

[M03] 执行外部命令
来源：http://ge.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yt.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mp.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vc.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yc.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ua.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oo.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kk.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://nl.nszjky.cn

[M04] 获取当前工作目录
来源：http://ni.shxzukj.cn

Py:   os.getcwd()
来源：http://pk.szxytkj.cn

PHP:  getcwd();
来源：http://kq.chemitech.net.cn

JS:   process.cwd()
来源：http://ek.yuexingan06.cn

TS:   process.cwd()
来源：http://br.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ak.shxzukj.cn

Go:   os.Getwd()
来源：http://fg.9csxet.cn

Ruby: Dir.pwd
来源：http://go.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wt.asd995.cn

[M05] 设置退出码
来源：http://no.shxzskj.cn

Py:   sys.exit(1)
来源：http://xz.yuexingan06.cn

PHP:  exit(1);
来源：http://ah.bookmarksfly.cn

JS:   process.exit(1)
来源：http://ta.gzmigu.cn

TS:   process.exit(1)
来源：http://fe.panjiajie.cn

Java: System.exit(1)
来源：http://ma.shxzskj.cn

Go:   os.Exit(1)
来源：http://ue.muxihuayi.cn

Ruby: exit 1
来源：http://wj.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dl.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ha.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://qk.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fj.colortex.cn

JS:   console.error("err")
来源：http://mx.huixinmuqiang.cn

TS:   console.error("err")
来源：http://ae.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://sh.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kd.jianghongdianzi.cn

Ruby: warn "err"
来源：http://iz.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://kq.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://so.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://zc.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ww.colortex.cn

JS:   require.main === module
来源：http://wm.colortex.cn

TS:   require.main === module
来源：http://ca.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://op.nszjky.cn

Go:   func main()
来源：http://ix.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zc.szsharing.cn

C#:   static void Main(string[] args)
来源：http://tn.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://zs.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://mz.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://mg.shxzukj.cn

JS:   process.platform;  process.version
来源：http://lh.shxzukj.cn

TS:   process.platform;  process.version
来源：http://sd.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kl.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xw.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bb.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pc.wgjwhj.cn

================================================================================
来源：http://fb.9csxet.cn

N. 数据结构与算法
来源：http://jb.huixiangedu.cn

================================================================================
来源：http://pv.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://qa.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iq.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://is.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bd.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wb.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fp.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://np.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yd.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cr.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://mv.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://af.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rt.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://il.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eh.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vw.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://pl.gzmigu.cn

Ruby: arr.sort
来源：http://kb.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gc.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://de.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pf.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ik.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rf.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rh.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://za.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ub.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dw.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pm.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://av.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qm.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://de.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ln.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://on.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vp.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bz.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wx.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xb.shtwfgs.cn

[N05] 最大公约数
来源：http://nf.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://ch.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hw.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tc.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ml.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xn.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dy.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://je.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kh.hnjuh.cn

[N06] 判断回文字符串
来源：http://sw.bjjhwx.cn

Py:   s == s[::-1]
来源：http://og.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://ip.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://az.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://wp.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bm.szsharing.cn

Go:   // 双指针从两端比较
来源：http://wj.yuexingan06.cn

Ruby: s == s.reverse
来源：http://yr.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bv.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://zp.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sc.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wj.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jy.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://to.chemitech.net.cn

Java: // 手写 HashMap
来源：http://zb.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://zg.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://mj.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ux.9csxet.cn

[N08] 生成全排列
来源：http://hw.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://zu.shxzskj.cn

PHP:  // 手写递归交换
来源：http://uw.asd995.cn

JS:   // 手写回溯递归
来源：http://vd.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://hb.huixiangedu.cn

Java: // 手写回溯递归
来源：http://xo.hahajie.cn

Go:   // 手写回溯递归
来源：http://pr.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://le.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://pp.panjiajie.cn

[N09] 栈与队列
来源：http://dt.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fc.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gz.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xz.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mj.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yr.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ie.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pz.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oc.bookmarksfly.cn

[N10] 链表节点定义
来源：http://ps.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://al.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oc.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qc.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ec.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://fw.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ko.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ya.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://ww.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pu.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ez.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jk.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ki.9csxet.cn

Java: // 手写递归
来源：http://ll.hnjuh.cn

Go:   // 手写递归
来源：http://yr.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bb.shxzskj.cn

C#:   // 手写递归
来源：http://nm.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hy.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tz.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fj.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://re.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tc.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ch.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://na.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nz.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pz.hahajie.cn

================================================================================
来源：http://ow.chemitech.net.cn

O. 并发与异步
来源：http://sj.yuntaijiaju.cn

================================================================================
来源：http://eu.yuexingan06.cn

[O01] 启动一个线程
来源：http://nv.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pj.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xp.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rh.bookmarksfly.cn

TS:   // 同 JS
来源：http://tq.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://oy.yuexingan06.cn

Go:   go f()
来源：http://ud.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://dr.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://dm.9csxet.cn

[O02] 使用线程池
来源：http://kr.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ea.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lh.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://ch.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://gl.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dr.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cu.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ze.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pt.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://kv.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://eh.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://im.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qf.shtwfgs.cn

TS:   // 同 JS
来源：http://qi.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://li.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cw.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zl.521024.cn

C#:   lock (gate) { shared++; }
来源：http://fh.hahajie.cn

[O04] 定义异步函数并等待
来源：http://pg.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://th.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jk.521024.cn

JS:   async function f() { await g(); }
来源：http://jg.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kt.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://id.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yx.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ha.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ch.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://ep.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://mi.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tv.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://md.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://bp.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fz.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fh.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://wm.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yv.chemitech.net.cn

[O06] 使用进程池
来源：http://jn.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cw.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qy.colortex.cn

JS:   // child_process / cluster 模块
来源：http://xb.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://pl.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://za.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vn.gzmigu.cn

Ruby: // fork 块
来源：http://du.yuntaijiaju.cn

C#:   Parallel.For
来源：http://dq.hnjuh.cn

================================================================================
来源：http://iv.chemitech.net.cn

P. 常用工具函数
来源：http://xv.asd995.cn

================================================================================
来源：http://ly.bjjhwx.cn

[P01] 生成 UUID
来源：http://ix.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://lx.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kl.hahajie.cn

JS:   crypto.randomUUID()
来源：http://po.asd995.cn

TS:   crypto.randomUUID()
来源：http://oj.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://tr.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://zw.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://gs.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://wo.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://fk.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oz.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eg.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nv.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pc.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jx.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ep.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ca.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gj.colortex.cn

[P03] 生成短随机字符串
来源：http://rw.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ps.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vw.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oz.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mw.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ob.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ne.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qb.colortex.cn

[P04] 求长度
来源：http://cs.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ts.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ok.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cd.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nc.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://jt.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://ur.521024.cn

Ruby: x.length;  x.size
来源：http://re.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gw.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://cc.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uu.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lb.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zg.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xe.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://la.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tf.9csxet.cn

Ruby: a == b
来源：http://uw.9csxet.cn


<!-- 参考信息 -->