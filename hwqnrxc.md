代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://iv.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qb.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qh.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://cj.colortex.cn

TS:   resp.ok;  resp.status
来源：http://rd.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://nr.newstarts.cn

Go:   resp.StatusCode
来源：http://mu.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://yv.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://lc.nicolike.cn

[L08] 并发请求多个地址
来源：http://fm.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ht.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://sc.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xa.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bb.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hh.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ah.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kg.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://re.muxihuayi.cn

================================================================================
来源：http://lf.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://bh.szsharing.cn

================================================================================
来源：http://gf.szsharing.cn

[M01] 读取命令行参数
来源：http://mw.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://oa.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://fz.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://yx.nicolike.cn

TS:   process.argv.slice(2)
来源：http://ms.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://uy.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://ww.nszjky.cn

Ruby: ARGV
来源：http://td.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://rj.szsharing.cn

[M02] 读取环境变量
来源：http://lq.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://af.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rh.asd995.cn

JS:   process.env.HOME
来源：http://ah.muxihuayi.cn

TS:   process.env.HOME
来源：http://ke.panjiajie.cn

Java: System.getenv("HOME")
来源：http://ht.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ee.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://to.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://de.nicolike.cn

[M03] 执行外部命令
来源：http://xd.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://on.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ec.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zh.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nz.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xy.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gd.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ov.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ic.nszjky.cn

[M04] 获取当前工作目录
来源：http://ah.huixiangedu.cn

Py:   os.getcwd()
来源：http://qc.szsharing.cn

PHP:  getcwd();
来源：http://fv.szsharing.cn

JS:   process.cwd()
来源：http://ur.lnxyls.cn

TS:   process.cwd()
来源：http://kg.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://rm.shxzukj.cn

Go:   os.Getwd()
来源：http://sb.hahajie.cn

Ruby: Dir.pwd
来源：http://xy.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bn.bjjhwx.cn

[M05] 设置退出码
来源：http://bk.szxytkj.cn

Py:   sys.exit(1)
来源：http://hh.nszjky.cn

PHP:  exit(1);
来源：http://dc.chemitech.net.cn

JS:   process.exit(1)
来源：http://bt.nicolike.cn

TS:   process.exit(1)
来源：http://cl.jianghongdianzi.cn

Java: System.exit(1)
来源：http://sd.shxzskj.cn

Go:   os.Exit(1)
来源：http://qi.haigaiapp.cn

Ruby: exit 1
来源：http://ov.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jh.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://hn.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://sg.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://em.panjiajie.cn

JS:   console.error("err")
来源：http://dx.asd995.cn

TS:   console.error("err")
来源：http://cw.yuexingan06.cn

Java: System.err.println("err")
来源：http://fx.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tm.huixiangedu.cn

Ruby: warn "err"
来源：http://ra.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://ot.asd995.cn

[M07] 判断是否为主入口
来源：http://gi.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://rw.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://at.yuntaijiaju.cn

JS:   require.main === module
来源：http://tw.asd995.cn

TS:   require.main === module
来源：http://xx.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://jv.jctech888.com.cn

Go:   func main()
来源：http://kq.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rm.hahajie.cn

C#:   static void Main(string[] args)
来源：http://ab.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://ac.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ml.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://kk.newstarts.cn

JS:   process.platform;  process.version
来源：http://io.shxzukj.cn

TS:   process.platform;  process.version
来源：http://bf.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://be.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vb.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gi.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tr.shtwfgs.cn

================================================================================
来源：http://kg.lnxyls.cn

N. 数据结构与算法
来源：http://bn.gzmigu.cn

================================================================================
来源：http://pb.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://bl.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sg.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tl.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yr.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yo.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dh.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://wi.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kk.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sf.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://hv.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://rg.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jy.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ob.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://om.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nb.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://sc.muxihuayi.cn

Ruby: arr.sort
来源：http://uh.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fk.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://ce.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lt.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://jw.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fw.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bt.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://er.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bb.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tk.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tx.nszjky.cn

[N04] 斐波那契数列
来源：http://is.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oi.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rt.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wi.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sq.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yr.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tk.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kr.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://au.521024.cn

[N05] 最大公约数
来源：http://ou.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://vm.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oz.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xn.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xk.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cu.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zt.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://rb.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ml.chemitech.net.cn

[N06] 判断回文字符串
来源：http://mi.9csxet.cn

Py:   s == s[::-1]
来源：http://aa.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://mo.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://lr.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://zg.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ot.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://jq.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://rv.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zf.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://og.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mx.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fk.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vv.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://na.newstarts.cn

Java: // 手写 HashMap
来源：http://dx.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://mg.nicolike.cn

Ruby: // 手写 Hash
来源：http://dh.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xp.hnjuh.cn

[N08] 生成全排列
来源：http://lb.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://kp.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://el.szsharing.cn

JS:   // 手写回溯递归
来源：http://wh.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://hx.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://te.lnxyls.cn

Go:   // 手写回溯递归
来源：http://sb.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://jh.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://nu.shxzukj.cn

[N09] 栈与队列
来源：http://tw.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nz.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gw.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ce.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://df.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eo.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qj.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qh.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://du.haigaiapp.cn

[N10] 链表节点定义
来源：http://aj.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yz.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cy.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tw.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bq.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://xg.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jn.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yf.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fm.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://mb.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kc.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://jm.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tc.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ws.szxytkj.cn

Java: // 手写递归
来源：http://gr.shxzukj.cn

Go:   // 手写递归
来源：http://sy.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dd.521024.cn

C#:   // 手写递归
来源：http://jy.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://at.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hr.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ci.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://el.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gp.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vt.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bs.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sp.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://et.hahajie.cn

================================================================================
来源：http://uo.szsharing.cn

O. 并发与异步
来源：http://fn.wgjwhj.cn

================================================================================
来源：http://mh.9csxet.cn

[O01] 启动一个线程
来源：http://bt.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bh.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dt.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wk.szsharing.cn

TS:   // 同 JS
来源：http://gw.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://iz.szxytkj.cn

Go:   go f()
来源：http://lh.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://js.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://qe.nszjky.cn

[O02] 使用线程池
来源：http://is.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zx.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ja.521024.cn

JS:   // worker_threads 线程池
来源：http://cv.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://bk.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kp.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ig.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xj.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zw.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://bj.szxytkj.cn

Py:   with lock: shared += 1
来源：http://fg.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://my.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ga.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ud.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://ir.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ow.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fe.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://ey.newstarts.cn

[O04] 定义异步函数并等待
来源：http://yf.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://kt.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://za.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://hk.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dj.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kk.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lx.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gr.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://dm.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://un.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://bt.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gm.asd995.cn

JS:   await Promise.all(tasks)
来源：http://jd.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://fo.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wz.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fe.asd995.cn

Ruby: threads.map(&:join)
来源：http://me.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sg.szsharing.cn

[O06] 使用进程池
来源：http://gi.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bu.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ab.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://qi.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://le.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xy.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ce.chemitech.net.cn

Ruby: // fork 块
来源：http://mn.jctech888.com.cn

C#:   Parallel.For
来源：http://jr.colortex.cn

================================================================================
来源：http://yq.9csxet.cn

P. 常用工具函数
来源：http://wq.panjiajie.cn

================================================================================
来源：http://mb.chemitech.net.cn

[P01] 生成 UUID
来源：http://se.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://uv.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yv.newstarts.cn

JS:   crypto.randomUUID()
来源：http://gx.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://km.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://sn.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://ps.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://ud.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://cg.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://di.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nx.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nl.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ml.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iz.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cl.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://il.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fm.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zo.szsharing.cn

[P03] 生成短随机字符串
来源：http://af.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ki.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kf.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ey.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://el.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hj.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jk.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wi.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nl.yuexingan06.cn

[P04] 求长度
来源：http://om.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wz.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ao.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gt.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cn.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://rx.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://yh.colortex.cn

Ruby: x.length;  x.size
来源：http://de.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jl.colortex.cn


<!-- 参考信息 -->