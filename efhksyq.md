代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hi.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qy.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hw.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://us.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://nv.lnxyls.cn

Java: resp.statusCode()
来源：http://ji.bjjhwx.cn

Go:   resp.StatusCode
来源：http://wc.gzmigu.cn

Ruby: resp.code.to_i
来源：http://xu.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://zr.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://zy.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vc.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://uc.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nu.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yt.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nn.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xi.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rx.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tr.asd995.cn

================================================================================
来源：http://fn.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://rv.colortex.cn

================================================================================
来源：http://pp.haigaiapp.cn

[M01] 读取命令行参数
来源：http://yy.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://zl.9csxet.cn

PHP:  $argv;  $argc;
来源：http://fb.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://cm.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://vr.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://xq.shxzukj.cn

Go:   os.Args[1:]
来源：http://jc.asd995.cn

Ruby: ARGV
来源：http://gg.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://zt.nicolike.cn

[M02] 读取环境变量
来源：http://nt.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://op.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://io.szxytkj.cn

JS:   process.env.HOME
来源：http://mo.wgjwhj.cn

TS:   process.env.HOME
来源：http://tl.szxytkj.cn

Java: System.getenv("HOME")
来源：http://vi.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ej.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://rm.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vo.lnxyls.cn

[M03] 执行外部命令
来源：http://yj.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xx.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://am.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eu.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wx.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dl.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ae.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tf.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://fl.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ny.shtwfgs.cn

Py:   os.getcwd()
来源：http://kw.panjiajie.cn

PHP:  getcwd();
来源：http://vp.chemitech.net.cn

JS:   process.cwd()
来源：http://cd.shtwfgs.cn

TS:   process.cwd()
来源：http://op.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://fw.huanxung.cn

Go:   os.Getwd()
来源：http://lk.shxzskj.cn

Ruby: Dir.pwd
来源：http://gi.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bo.szsharing.cn

[M05] 设置退出码
来源：http://as.muxihuayi.cn

Py:   sys.exit(1)
来源：http://xn.jctech888.com.cn

PHP:  exit(1);
来源：http://vc.newstarts.cn

JS:   process.exit(1)
来源：http://kb.panjiajie.cn

TS:   process.exit(1)
来源：http://jm.bjjhwx.cn

Java: System.exit(1)
来源：http://ls.asd995.cn

Go:   os.Exit(1)
来源：http://yv.colortex.cn

Ruby: exit 1
来源：http://wu.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nu.521024.cn

[M06] 向标准错误输出
来源：http://mu.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://zh.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://be.wgjwhj.cn

JS:   console.error("err")
来源：http://zs.colortex.cn

TS:   console.error("err")
来源：http://ug.shtwfgs.cn

Java: System.err.println("err")
来源：http://cl.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ai.bookmarksfly.cn

Ruby: warn "err"
来源：http://aj.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.521024.cn

[M07] 判断是否为主入口
来源：http://cp.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://km.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.newstarts.cn

JS:   require.main === module
来源：http://qj.szsharing.cn

TS:   require.main === module
来源：http://tr.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://ge.newstarts.cn

Go:   func main()
来源：http://xf.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yn.hahajie.cn

C#:   static void Main(string[] args)
来源：http://lf.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://gl.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://td.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://tk.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://bi.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://sq.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jr.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eq.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pm.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hv.gzmigu.cn

================================================================================
来源：http://bm.521024.cn

N. 数据结构与算法
来源：http://if.colortex.cn

================================================================================
来源：http://pz.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://ba.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ce.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bz.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qi.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zz.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lj.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://cc.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ed.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bh.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://xt.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://uv.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ga.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://je.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zm.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tl.nicolike.cn

Go:   slices.Sort(arr)
来源：http://kz.shtwfgs.cn

Ruby: arr.sort
来源：http://ph.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ez.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://ft.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tb.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://qb.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gk.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qg.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ui.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sb.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uv.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mb.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://eu.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ul.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bn.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xs.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vv.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fs.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sj.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://db.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jh.bjjhwx.cn

[N05] 最大公约数
来源：http://ey.colortex.cn

Py:   math.gcd(a, b)
来源：http://se.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ez.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mb.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ut.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yx.521024.cn

Ruby: a.gcd(b)
来源：http://wq.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oy.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://vf.chemitech.net.cn

Py:   s == s[::-1]
来源：http://tj.huanxung.cn

PHP:  $s === strrev($s);
来源：http://el.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://di.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://eu.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oa.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://zy.panjiajie.cn

Ruby: s == s.reverse
来源：http://ez.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://te.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://ri.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ge.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uy.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zv.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://og.chemitech.net.cn

Java: // 手写 HashMap
来源：http://ss.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://gp.nicolike.cn

Ruby: // 手写 Hash
来源：http://of.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eu.shxzukj.cn

[N08] 生成全排列
来源：http://zm.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://xx.nicolike.cn

PHP:  // 手写递归交换
来源：http://xg.huanxung.cn

JS:   // 手写回溯递归
来源：http://td.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://vf.nicolike.cn

Java: // 手写回溯递归
来源：http://qi.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://hr.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://wc.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://do.shxzukj.cn

[N09] 栈与队列
来源：http://kb.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://et.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kg.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://il.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ye.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ds.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qq.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xm.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sv.nszjky.cn

[N10] 链表节点定义
来源：http://gy.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mk.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kq.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xx.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://gt.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fn.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ux.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sn.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://cr.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cr.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://bj.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pd.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lu.lnxyls.cn

Java: // 手写递归
来源：http://dx.521024.cn

Go:   // 手写递归
来源：http://fq.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lt.muxihuayi.cn

C#:   // 手写递归
来源：http://md.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://om.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ng.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rm.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ah.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fx.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://io.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gi.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ey.huixiangedu.cn

================================================================================
来源：http://zt.yuntaijiaju.cn

O. 并发与异步
来源：http://ks.colortex.cn

================================================================================
来源：http://go.colortex.cn

[O01] 启动一个线程
来源：http://hv.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vf.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hk.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nr.yuntaijiaju.cn

TS:   // 同 JS
来源：http://wh.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://kl.jianghongdianzi.cn

Go:   go f()
来源：http://ql.newstarts.cn

Ruby: Thread.new { f }
来源：http://za.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://nl.szxytkj.cn

[O02] 使用线程池
来源：http://wa.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lp.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qu.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://cf.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://kf.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xs.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hm.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qn.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lk.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://ge.521024.cn

Py:   with lock: shared += 1
来源：http://ur.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://di.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ay.lnxyls.cn

TS:   // 同 JS
来源：http://lw.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://uq.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tn.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ov.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://vo.521024.cn

[O04] 定义异步函数并等待
来源：http://yj.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://mz.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wd.nszjky.cn

JS:   async function f() { await g(); }
来源：http://em.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fy.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zz.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nm.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xc.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://mc.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://sf.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://au.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fc.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://fd.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://xj.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kc.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ue.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://tf.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kb.shxzskj.cn

[O06] 使用进程池
来源：http://lf.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bu.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pk.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://ub.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://mk.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oo.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uh.wgjwhj.cn

Ruby: // fork 块
来源：http://gh.huanxung.cn

C#:   Parallel.For
来源：http://sy.shxzskj.cn

================================================================================
来源：http://nr.9csxet.cn

P. 常用工具函数
来源：http://dn.newstarts.cn

================================================================================
来源：http://lt.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://km.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://vq.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ez.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://eo.521024.cn

TS:   crypto.randomUUID()
来源：http://oz.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://lq.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://np.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://wm.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://sk.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://gc.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zb.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ue.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gv.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://by.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rr.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tk.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vd.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bj.shxzukj.cn

[P03] 生成短随机字符串
来源：http://kz.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ve.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lh.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ct.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gh.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sz.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dc.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ay.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ma.gzmigu.cn

[P04] 求长度
来源：http://jx.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xb.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jh.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kr.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://im.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://ju.521024.cn

Go:   len(arr);  len(m)
来源：http://st.szxytkj.cn

Ruby: x.length;  x.size
来源：http://wl.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://au.shxzskj.cn


<!-- 参考信息 -->