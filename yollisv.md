代发 wailian999

TS:   resp.ok;  resp.status
来源：http://ym.wgjwhj.cn

Java: resp.statusCode()
来源：http://nf.wgjwhj.cn

Go:   resp.StatusCode
来源：http://lg.shxzskj.cn

Ruby: resp.code.to_i
来源：http://kt.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://ux.szxytkj.cn

[L08] 并发请求多个地址
来源：http://cq.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fo.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://cb.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://md.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iq.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dh.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gm.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gw.hnjuh.cn

================================================================================
来源：http://tb.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://gz.asd995.cn

================================================================================
来源：http://lz.nszjky.cn

[M01] 读取命令行参数
来源：http://mw.huanxung.cn

Py:   sys.argv[1:]
来源：http://mr.szsharing.cn

PHP:  $argv;  $argc;
来源：http://ow.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://dm.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://sw.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://as.huanxung.cn

Go:   os.Args[1:]
来源：http://xi.asd995.cn

Ruby: ARGV
来源：http://yz.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://dq.shxzskj.cn

[M02] 读取环境变量
来源：http://no.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://si.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rv.szxytkj.cn

JS:   process.env.HOME
来源：http://pe.chemitech.net.cn

TS:   process.env.HOME
来源：http://pr.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://ez.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pa.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://gk.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gh.nszjky.cn

[M03] 执行外部命令
来源：http://na.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nl.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pf.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://my.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mv.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eu.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nt.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ne.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://hq.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://uc.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://kr.bookmarksfly.cn

PHP:  getcwd();
来源：http://md.colortex.cn

JS:   process.cwd()
来源：http://zr.nicolike.cn

TS:   process.cwd()
来源：http://eq.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ns.gzmigu.cn

Go:   os.Getwd()
来源：http://wp.chemitech.net.cn

Ruby: Dir.pwd
来源：http://ri.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.huixiangedu.cn

[M05] 设置退出码
来源：http://pk.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://sa.szxytkj.cn

PHP:  exit(1);
来源：http://nm.jctech888.com.cn

JS:   process.exit(1)
来源：http://ww.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ny.jianghongdianzi.cn

Java: System.exit(1)
来源：http://wt.wgjwhj.cn

Go:   os.Exit(1)
来源：http://dl.jctech888.com.cn

Ruby: exit 1
来源：http://zy.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wl.muxihuayi.cn

[M06] 向标准错误输出
来源：http://yt.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://mx.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bt.lnxyls.cn

JS:   console.error("err")
来源：http://tu.huixiangedu.cn

TS:   console.error("err")
来源：http://dl.nszjky.cn

Java: System.err.println("err")
来源：http://zb.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hr.newstarts.cn

Ruby: warn "err"
来源：http://bm.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://ku.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://ok.colortex.cn

Py:   if __name__ == "__main__":
来源：http://zt.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oh.hahajie.cn

JS:   require.main === module
来源：http://zn.haigaiapp.cn

TS:   require.main === module
来源：http://bb.shxzskj.cn

Java: public static void main(String[] args)
来源：http://wh.gzmigu.cn

Go:   func main()
来源：http://tw.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zk.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://gq.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://wg.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://va.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://aq.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://mo.gzmigu.cn

TS:   process.platform;  process.version
来源：http://we.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iu.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hl.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yx.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rz.9csxet.cn

================================================================================
来源：http://zn.huanxung.cn

N. 数据结构与算法
来源：http://pd.521024.cn

================================================================================
来源：http://yt.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://ro.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hj.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ao.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zh.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ld.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xg.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://dk.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fe.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ol.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://bl.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://tj.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kr.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ej.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cj.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hi.nicolike.cn

Go:   slices.Sort(arr)
来源：http://xb.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ol.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fj.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://sr.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pw.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://wa.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pw.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vo.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tc.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yg.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ku.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hh.huanxung.cn

[N04] 斐波那契数列
来源：http://ze.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://av.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sb.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eo.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xh.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fk.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qu.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xn.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zu.szsharing.cn

[N05] 最大公约数
来源：http://wc.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://ns.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zw.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lg.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ut.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hh.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rz.shxzukj.cn

Ruby: a.gcd(b)
来源：http://cg.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vd.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://xq.nicolike.cn

Py:   s == s[::-1]
来源：http://xm.nicolike.cn

PHP:  $s === strrev($s);
来源：http://kq.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ut.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://xv.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nb.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://zh.shxzukj.cn

Ruby: s == s.reverse
来源：http://vt.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://el.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://gf.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lw.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uy.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://be.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://fd.hahajie.cn

Java: // 手写 HashMap
来源：http://vo.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://wi.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ed.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://go.szsharing.cn

[N08] 生成全排列
来源：http://we.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://xj.szxytkj.cn

PHP:  // 手写递归交换
来源：http://tb.521024.cn

JS:   // 手写回溯递归
来源：http://ra.colortex.cn

TS:   // 手写回溯递归
来源：http://sl.bjjhwx.cn

Java: // 手写回溯递归
来源：http://br.nicolike.cn

Go:   // 手写回溯递归
来源：http://qy.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://op.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://hj.szxytkj.cn

[N09] 栈与队列
来源：http://oy.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dw.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dw.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sw.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://it.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eg.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ci.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kl.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tr.wgjwhj.cn

[N10] 链表节点定义
来源：http://oz.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ew.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bf.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gp.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ju.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://pe.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://au.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xq.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cf.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://jp.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rl.hahajie.cn

PHP:  // 手写递归函数
来源：http://qp.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://px.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ex.newstarts.cn

Java: // 手写递归
来源：http://cc.jctech888.com.cn

Go:   // 手写递归
来源：http://di.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uj.szsharing.cn

C#:   // 手写递归
来源：http://ji.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ku.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ch.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://av.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gv.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://er.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ab.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nr.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qo.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vo.521024.cn

================================================================================
来源：http://jz.9csxet.cn

O. 并发与异步
来源：http://ud.bookmarksfly.cn

================================================================================
来源：http://fj.chemitech.net.cn

[O01] 启动一个线程
来源：http://uw.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fw.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bm.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cv.hnjuh.cn

TS:   // 同 JS
来源：http://zu.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://mn.hnjuh.cn

Go:   go f()
来源：http://vq.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://my.nszjky.cn

C#:   Task.Run(() => F());
来源：http://xc.jctech888.com.cn

[O02] 使用线程池
来源：http://bb.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ug.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sq.colortex.cn

JS:   // worker_threads 线程池
来源：http://pm.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://en.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://we.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mu.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rp.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hu.szsharing.cn

[O03] 加锁保护共享数据
来源：http://sm.hnjuh.cn

Py:   with lock: shared += 1
来源：http://tz.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://dd.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rt.szxytkj.cn

TS:   // 同 JS
来源：http://yb.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://tc.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ye.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ck.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://ma.nicolike.cn

[O04] 定义异步函数并等待
来源：http://dt.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://fx.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ht.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://lx.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zt.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pw.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://op.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rt.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://gq.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://hx.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://gg.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wn.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://ca.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ht.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xg.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://me.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://bs.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://td.newstarts.cn

[O06] 使用进程池
来源：http://ya.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fb.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dh.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://cj.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://vy.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wj.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dc.szxytkj.cn

Ruby: // fork 块
来源：http://xp.szsharing.cn

C#:   Parallel.For
来源：http://lj.hahajie.cn

================================================================================
来源：http://nl.hnjuh.cn

P. 常用工具函数
来源：http://et.hahajie.cn

================================================================================
来源：http://tl.bjjhwx.cn

[P01] 生成 UUID
来源：http://wh.521024.cn

Py:   str(uuid.uuid4())
来源：http://lu.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gd.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ks.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://ac.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://kx.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://as.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://uf.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://ah.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://tw.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rd.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jc.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dp.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pa.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://te.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jr.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tb.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nb.nszjky.cn

[P03] 生成短随机字符串
来源：http://nr.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://es.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wf.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sb.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://by.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vm.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ja.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cg.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ye.shxzukj.cn

[P04] 求长度
来源：http://yy.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ho.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kh.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jf.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ve.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://wy.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://dp.shxzskj.cn

Ruby: x.length;  x.size
来源：http://dn.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ix.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://an.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xs.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dw.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ka.yuntaijiaju.cn


<!-- 参考信息 -->