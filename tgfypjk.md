代发 wailian999

TS:   resp.ok;  resp.status
来源：http://zs.yuexingan06.cn

Java: resp.statusCode()
来源：http://or.colortex.cn

Go:   resp.StatusCode
来源：http://qp.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://xz.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://hx.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://ob.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pf.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ik.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xa.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ox.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lx.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mw.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aw.nicolike.cn

================================================================================
来源：http://rl.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://ow.chemitech.net.cn

================================================================================
来源：http://lc.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://fh.hnjuh.cn

Py:   sys.argv[1:]
来源：http://ok.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://ds.nszjky.cn

JS:   process.argv.slice(2)
来源：http://bz.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://fd.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://fd.asd995.cn

Go:   os.Args[1:]
来源：http://da.chemitech.net.cn

Ruby: ARGV
来源：http://mr.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ht.hnjuh.cn

[M02] 读取环境变量
来源：http://cy.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://kv.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xi.muxihuayi.cn

JS:   process.env.HOME
来源：http://wo.hahajie.cn

TS:   process.env.HOME
来源：http://ym.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ht.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tp.nicolike.cn

Ruby: ENV["HOME"]
来源：http://ts.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ei.hnjuh.cn

[M03] 执行外部命令
来源：http://sm.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vi.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rm.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rk.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ki.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mr.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yn.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xb.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://tl.nszjky.cn

[M04] 获取当前工作目录
来源：http://hr.chemitech.net.cn

Py:   os.getcwd()
来源：http://zf.bjjhwx.cn

PHP:  getcwd();
来源：http://ty.szsharing.cn

JS:   process.cwd()
来源：http://xe.huixinmuqiang.cn

TS:   process.cwd()
来源：http://fy.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://mw.shxzukj.cn

Go:   os.Getwd()
来源：http://sl.colortex.cn

Ruby: Dir.pwd
来源：http://fj.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lz.chemitech.net.cn

[M05] 设置退出码
来源：http://ix.huanxung.cn

Py:   sys.exit(1)
来源：http://nm.huixiangedu.cn

PHP:  exit(1);
来源：http://ud.chemitech.net.cn

JS:   process.exit(1)
来源：http://kc.shtwfgs.cn

TS:   process.exit(1)
来源：http://sh.shtwfgs.cn

Java: System.exit(1)
来源：http://zf.nszjky.cn

Go:   os.Exit(1)
来源：http://uh.yuntaijiaju.cn

Ruby: exit 1
来源：http://lc.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hf.colortex.cn

[M06] 向标准错误输出
来源：http://my.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://iz.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cv.asd995.cn

JS:   console.error("err")
来源：http://pp.lnxyls.cn

TS:   console.error("err")
来源：http://wj.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://ir.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://we.muxihuayi.cn

Ruby: warn "err"
来源：http://qe.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.panjiajie.cn

[M07] 判断是否为主入口
来源：http://rr.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://cv.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ww.huixinmuqiang.cn

JS:   require.main === module
来源：http://hf.yuntaijiaju.cn

TS:   require.main === module
来源：http://rh.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://tu.asd995.cn

Go:   func main()
来源：http://ja.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hf.newstarts.cn

C#:   static void Main(string[] args)
来源：http://oe.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://dg.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://gs.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ee.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://dr.panjiajie.cn

TS:   process.platform;  process.version
来源：http://kk.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vh.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bb.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jd.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pd.szsharing.cn

================================================================================
来源：http://uu.panjiajie.cn

N. 数据结构与算法
来源：http://xb.szxytkj.cn

================================================================================
来源：http://we.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://tz.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hh.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vs.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ql.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hj.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://va.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://la.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sp.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dg.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://zj.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://gl.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qs.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xm.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jb.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fu.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://hw.bjjhwx.cn

Ruby: arr.sort
来源：http://yw.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ce.asd995.cn

[N03] 快速排序（分治示例）
来源：http://wx.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://is.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://tf.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qi.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dj.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pl.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pr.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rr.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jj.521024.cn

[N04] 斐波那契数列
来源：http://am.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kw.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zy.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://np.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yk.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ez.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qa.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cj.9csxet.cn

[N05] 最大公约数
来源：http://xp.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://qx.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mq.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fd.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uz.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ia.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vr.521024.cn

Ruby: a.gcd(b)
来源：http://ld.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yw.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ig.shxzskj.cn

Py:   s == s[::-1]
来源：http://iz.nicolike.cn

PHP:  $s === strrev($s);
来源：http://vd.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://xi.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://rk.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vj.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://nb.wgjwhj.cn

Ruby: s == s.reverse
来源：http://np.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sb.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://zh.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://np.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pb.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uk.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ea.newstarts.cn

Java: // 手写 HashMap
来源：http://vp.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://vb.asd995.cn

Ruby: // 手写 Hash
来源：http://jk.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gk.asd995.cn

[N08] 生成全排列
来源：http://pm.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://gb.panjiajie.cn

PHP:  // 手写递归交换
来源：http://zo.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://xz.lnxyls.cn

TS:   // 手写回溯递归
来源：http://vu.yuexingan06.cn

Java: // 手写回溯递归
来源：http://hn.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://cg.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://qt.szsharing.cn

C#:   // 手写回溯递归
来源：http://aj.521024.cn

[N09] 栈与队列
来源：http://se.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hk.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://id.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ro.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tj.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ze.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uk.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lw.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xk.huanxung.cn

[N10] 链表节点定义
来源：http://lt.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://et.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ri.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xx.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aj.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://bh.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hm.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ux.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qb.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://eh.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jp.asd995.cn

PHP:  // 手写递归函数
来源：http://st.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kw.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ic.chemitech.net.cn

Java: // 手写递归
来源：http://zc.colortex.cn

Go:   // 手写递归
来源：http://bf.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ue.lnxyls.cn

C#:   // 手写递归
来源：http://bt.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ft.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lv.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nh.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://al.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jx.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://py.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ke.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ow.shxzskj.cn

================================================================================
来源：http://qa.jctech888.com.cn

O. 并发与异步
来源：http://nh.gzmigu.cn

================================================================================
来源：http://uh.chemitech.net.cn

[O01] 启动一个线程
来源：http://kd.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dc.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yv.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://no.yuntaijiaju.cn

TS:   // 同 JS
来源：http://fr.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://nl.huixiangedu.cn

Go:   go f()
来源：http://fp.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://kc.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ug.shxzskj.cn

[O02] 使用线程池
来源：http://fk.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cc.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ho.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://oh.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://ll.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pz.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lm.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qo.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lq.9csxet.cn

[O03] 加锁保护共享数据
来源：http://ug.521024.cn

Py:   with lock: shared += 1
来源：http://qu.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://vo.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ck.yuexingan06.cn

TS:   // 同 JS
来源：http://ya.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://dg.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yq.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tj.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://kj.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://og.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://uj.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nq.nicolike.cn

JS:   async function f() { await g(); }
来源：http://du.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hw.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fu.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tm.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pz.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://ku.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://dl.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://aa.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iz.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://pu.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://yg.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rt.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qv.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://xr.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ik.jctech888.com.cn

[O06] 使用进程池
来源：http://oh.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://id.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://su.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://pf.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://xa.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://so.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fb.bjjhwx.cn

Ruby: // fork 块
来源：http://kb.shxzskj.cn

C#:   Parallel.For
来源：http://ru.521024.cn

================================================================================
来源：http://sp.bookmarksfly.cn

P. 常用工具函数
来源：http://qs.yuntaijiaju.cn

================================================================================
来源：http://jp.nicolike.cn

[P01] 生成 UUID
来源：http://qc.asd995.cn

Py:   str(uuid.uuid4())
来源：http://mt.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sq.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://qb.nicolike.cn

TS:   crypto.randomUUID()
来源：http://qu.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://mc.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://ja.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://co.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://gg.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://ln.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mh.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ol.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hc.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ot.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fi.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qn.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ua.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pk.szxytkj.cn

[P03] 生成短随机字符串
来源：http://gl.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wf.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qe.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://me.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ei.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iy.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cb.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gv.muxihuayi.cn

[P04] 求长度
来源：http://bj.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nt.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lg.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uo.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xp.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ha.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://gn.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://xy.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qv.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://uu.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bh.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hl.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ww.huixiangedu.cn


<!-- 参考信息 -->