代发 wailian999

C#:   (int)resp.StatusCode
来源：http://tg.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://kb.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vw.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://rm.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ky.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rm.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ey.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lw.huixinmuqiang.cn

================================================================================
来源：http://en.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://ts.hnjuh.cn

================================================================================
来源：http://mb.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://sl.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://ei.szsharing.cn

PHP:  $argv;  $argc;
来源：http://na.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://kd.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://lz.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://qg.panjiajie.cn

Go:   os.Args[1:]
来源：http://ir.wgjwhj.cn

Ruby: ARGV
来源：http://gl.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ch.muxihuayi.cn

[M02] 读取环境变量
来源：http://jf.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://am.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fz.newstarts.cn

JS:   process.env.HOME
来源：http://jk.colortex.cn

TS:   process.env.HOME
来源：http://bx.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://rg.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vt.9csxet.cn

Ruby: ENV["HOME"]
来源：http://tc.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yv.nszjky.cn

[M03] 执行外部命令
来源：http://ex.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kw.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ts.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jm.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ho.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ar.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uk.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wm.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://qi.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://cq.nicolike.cn

Py:   os.getcwd()
来源：http://hh.chemitech.net.cn

PHP:  getcwd();
来源：http://ij.huanxung.cn

JS:   process.cwd()
来源：http://rq.yuntaijiaju.cn

TS:   process.cwd()
来源：http://kx.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://lx.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ue.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ly.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qi.jianghongdianzi.cn

[M05] 设置退出码
来源：http://el.gzmigu.cn

Py:   sys.exit(1)
来源：http://wc.hnjuh.cn

PHP:  exit(1);
来源：http://or.hahajie.cn

JS:   process.exit(1)
来源：http://tu.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://vx.hahajie.cn

Java: System.exit(1)
来源：http://ns.nszjky.cn

Go:   os.Exit(1)
来源：http://ik.haigaiapp.cn

Ruby: exit 1
来源：http://vo.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kc.shxzskj.cn

[M06] 向标准错误输出
来源：http://rx.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://np.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xu.panjiajie.cn

JS:   console.error("err")
来源：http://wy.lnxyls.cn

TS:   console.error("err")
来源：http://fv.bjjhwx.cn

Java: System.err.println("err")
来源：http://en.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vw.hahajie.cn

Ruby: warn "err"
来源：http://tw.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://dl.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://ba.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://pr.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wq.shxzskj.cn

JS:   require.main === module
来源：http://nh.yuntaijiaju.cn

TS:   require.main === module
来源：http://am.colortex.cn

Java: public static void main(String[] args)
来源：http://uj.huixiangedu.cn

Go:   func main()
来源：http://vc.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vv.huanxung.cn

C#:   static void Main(string[] args)
来源：http://au.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://ev.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://fr.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://az.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://vv.gzmigu.cn

TS:   process.platform;  process.version
来源：http://dm.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vn.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nz.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gs.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ar.bookmarksfly.cn

================================================================================
来源：http://bx.szsharing.cn

N. 数据结构与算法
来源：http://zl.hahajie.cn

================================================================================
来源：http://dr.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://ou.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mi.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jv.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mx.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zr.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vv.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tw.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rq.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://up.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://dc.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ak.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pf.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qc.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tp.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://iy.colortex.cn

Ruby: arr.sort
来源：http://og.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dn.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://cs.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ub.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://hs.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://by.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://co.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cr.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://al.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rh.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://je.521024.cn

[N04] 斐波那契数列
来源：http://ek.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pt.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rw.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tx.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jx.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tb.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xy.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tt.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lm.gzmigu.cn

[N05] 最大公约数
来源：http://aj.nszjky.cn

Py:   math.gcd(a, b)
来源：http://cz.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ae.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lm.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ef.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rs.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lo.shxzskj.cn

Ruby: a.gcd(b)
来源：http://be.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wn.panjiajie.cn

[N06] 判断回文字符串
来源：http://vv.9csxet.cn

Py:   s == s[::-1]
来源：http://uv.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://ry.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://iu.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://ix.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rr.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://yt.wgjwhj.cn

Ruby: s == s.reverse
来源：http://px.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://al.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://nd.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uw.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vm.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wu.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://qq.hnjuh.cn

Java: // 手写 HashMap
来源：http://de.521024.cn

Go:   // 手写 map[int]int
来源：http://qx.nicolike.cn

Ruby: // 手写 Hash
来源：http://jo.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gy.haigaiapp.cn

[N08] 生成全排列
来源：http://hr.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://lr.521024.cn

PHP:  // 手写递归交换
来源：http://iz.nszjky.cn

JS:   // 手写回溯递归
来源：http://bi.szxytkj.cn

TS:   // 手写回溯递归
来源：http://zb.lnxyls.cn

Java: // 手写回溯递归
来源：http://ku.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ko.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://iy.panjiajie.cn

C#:   // 手写回溯递归
来源：http://bs.panjiajie.cn

[N09] 栈与队列
来源：http://sk.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ql.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qc.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oj.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qp.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jy.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eo.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fc.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ey.colortex.cn

[N10] 链表节点定义
来源：http://mr.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ia.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ue.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hi.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xs.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://an.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wk.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wm.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sd.newstarts.cn

[N11] 二叉树中序遍历
来源：http://ob.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zx.colortex.cn

PHP:  // 手写递归函数
来源：http://vs.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bn.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fw.muxihuayi.cn

Java: // 手写递归
来源：http://zf.nszjky.cn

Go:   // 手写递归
来源：http://xo.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rw.lnxyls.cn

C#:   // 手写递归
来源：http://ff.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://am.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dl.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vh.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fu.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sp.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jz.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eh.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wa.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wt.shtwfgs.cn

================================================================================
来源：http://yw.lnxyls.cn

O. 并发与异步
来源：http://ln.szxytkj.cn

================================================================================
来源：http://qs.muxihuayi.cn

[O01] 启动一个线程
来源：http://pq.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ai.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rt.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vs.gzmigu.cn

TS:   // 同 JS
来源：http://gw.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://ot.asd995.cn

Go:   go f()
来源：http://ez.shxzskj.cn

Ruby: Thread.new { f }
来源：http://ix.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ht.gzmigu.cn

[O02] 使用线程池
来源：http://yi.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tk.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nr.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://cj.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://vv.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fv.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ju.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uw.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ub.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://wl.nicolike.cn

Py:   with lock: shared += 1
来源：http://pg.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://kg.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ml.shxzukj.cn

TS:   // 同 JS
来源：http://il.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://ze.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aw.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xu.521024.cn

C#:   lock (gate) { shared++; }
来源：http://qm.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://ix.521024.cn

Py:   async def f():⏎    await g()
来源：http://zt.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bm.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ru.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ps.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://po.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bs.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://es.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://jz.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://zz.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://qr.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xp.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://qe.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://we.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rl.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fx.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://ny.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zj.yuntaijiaju.cn

[O06] 使用进程池
来源：http://pi.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wc.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tf.521024.cn

JS:   // child_process / cluster 模块
来源：http://yb.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://am.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gn.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ud.nicolike.cn

Ruby: // fork 块
来源：http://ht.wgjwhj.cn

C#:   Parallel.For
来源：http://fu.hnjuh.cn

================================================================================
来源：http://gh.szxytkj.cn

P. 常用工具函数
来源：http://ui.jianghongdianzi.cn

================================================================================
来源：http://iy.gzmigu.cn

[P01] 生成 UUID
来源：http://dx.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ew.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oh.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://bl.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ww.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://vz.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://em.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://ik.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://bg.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://zj.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://od.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pq.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ws.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://so.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ys.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jy.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ad.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bl.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://oc.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wh.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dc.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ac.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ld.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hu.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bb.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://of.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jz.bookmarksfly.cn

[P04] 求长度
来源：http://wy.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jf.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xm.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ie.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://he.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://bk.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://kc.521024.cn

Ruby: x.length;  x.size
来源：http://un.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yu.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://uy.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mw.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lf.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ec.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ct.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gk.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gu.bjjhwx.cn

Ruby: a == b
来源：http://yi.chemitech.net.cn


<!-- 参考信息 -->