代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://rx.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yu.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gl.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ye.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://zy.nicolike.cn

Java: resp.statusCode()
来源：http://ip.chemitech.net.cn

Go:   resp.StatusCode
来源：http://ce.nicolike.cn

Ruby: resp.code.to_i
来源：http://hd.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://lw.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ja.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eo.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://bd.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sw.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yp.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ui.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zn.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sx.huanxung.cn

================================================================================
来源：http://ep.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://uh.shtwfgs.cn

================================================================================
来源：http://rb.panjiajie.cn

[M01] 读取命令行参数
来源：http://sv.hnjuh.cn

Py:   sys.argv[1:]
来源：http://ja.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://gu.nicolike.cn

JS:   process.argv.slice(2)
来源：http://eg.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://sp.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://wx.521024.cn

Go:   os.Args[1:]
来源：http://el.bookmarksfly.cn

Ruby: ARGV
来源：http://bi.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://fo.shxzskj.cn

[M02] 读取环境变量
来源：http://mw.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://oa.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://em.huixiangedu.cn

JS:   process.env.HOME
来源：http://sj.colortex.cn

TS:   process.env.HOME
来源：http://jo.szxytkj.cn

Java: System.getenv("HOME")
来源：http://df.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cc.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ct.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ox.bjjhwx.cn

[M03] 执行外部命令
来源：http://rh.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ev.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zc.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cr.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kz.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vs.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ty.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hj.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://it.hnjuh.cn

[M04] 获取当前工作目录
来源：http://yg.szsharing.cn

Py:   os.getcwd()
来源：http://do.nszjky.cn

PHP:  getcwd();
来源：http://cf.nszjky.cn

JS:   process.cwd()
来源：http://cl.asd995.cn

TS:   process.cwd()
来源：http://au.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://od.wgjwhj.cn

Go:   os.Getwd()
来源：http://qj.shxzukj.cn

Ruby: Dir.pwd
来源：http://pc.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.shtwfgs.cn

[M05] 设置退出码
来源：http://pe.9csxet.cn

Py:   sys.exit(1)
来源：http://yy.jianghongdianzi.cn

PHP:  exit(1);
来源：http://dm.nicolike.cn

JS:   process.exit(1)
来源：http://si.shtwfgs.cn

TS:   process.exit(1)
来源：http://wd.gzmigu.cn

Java: System.exit(1)
来源：http://nn.hnjuh.cn

Go:   os.Exit(1)
来源：http://ck.bjjhwx.cn

Ruby: exit 1
来源：http://jx.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kc.nszjky.cn

[M06] 向标准错误输出
来源：http://bx.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://xq.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sl.9csxet.cn

JS:   console.error("err")
来源：http://po.521024.cn

TS:   console.error("err")
来源：http://zp.szxytkj.cn

Java: System.err.println("err")
来源：http://wu.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ir.shxzskj.cn

Ruby: warn "err"
来源：http://eu.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://lw.nicolike.cn

[M07] 判断是否为主入口
来源：http://no.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://ze.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://to.chemitech.net.cn

JS:   require.main === module
来源：http://gd.muxihuayi.cn

TS:   require.main === module
来源：http://ho.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://uv.shxzskj.cn

Go:   func main()
来源：http://yi.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://he.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://nw.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://go.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://bj.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://ck.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://xh.shxzskj.cn

TS:   process.platform;  process.version
来源：http://dq.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://is.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uc.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ba.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ig.shxzskj.cn

================================================================================
来源：http://gt.newstarts.cn

N. 数据结构与算法
来源：http://sr.szxytkj.cn

================================================================================
来源：http://yz.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://in.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xc.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rf.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rn.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nx.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ae.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ph.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rt.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xw.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://yb.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ej.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ny.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jx.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qy.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mf.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://uo.shxzukj.cn

Ruby: arr.sort
来源：http://cy.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qn.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://yk.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cl.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://kl.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vc.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pc.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://at.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ph.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rh.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vo.hahajie.cn

[N04] 斐波那契数列
来源：http://ry.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xx.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rj.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tp.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ab.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mw.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cu.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bs.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sl.bookmarksfly.cn

[N05] 最大公约数
来源：http://hr.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://oo.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lt.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mg.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cz.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mj.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cg.szxytkj.cn

Ruby: a.gcd(b)
来源：http://ws.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://od.hahajie.cn

[N06] 判断回文字符串
来源：http://gl.lnxyls.cn

Py:   s == s[::-1]
来源：http://ke.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://ne.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://fh.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://ro.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xk.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://wp.wgjwhj.cn

Ruby: s == s.reverse
来源：http://ny.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kb.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://or.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fw.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qr.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fa.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://jx.muxihuayi.cn

Java: // 手写 HashMap
来源：http://av.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://eq.shxzukj.cn

Ruby: // 手写 Hash
来源：http://zi.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zq.panjiajie.cn

[N08] 生成全排列
来源：http://ln.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://fd.nszjky.cn

PHP:  // 手写递归交换
来源：http://sr.9csxet.cn

JS:   // 手写回溯递归
来源：http://bw.asd995.cn

TS:   // 手写回溯递归
来源：http://uo.shtwfgs.cn

Java: // 手写回溯递归
来源：http://il.nszjky.cn

Go:   // 手写回溯递归
来源：http://pp.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://ou.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ua.lnxyls.cn

[N09] 栈与队列
来源：http://nl.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rt.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ja.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fo.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cg.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mk.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gg.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zs.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kq.yuexingan06.cn

[N10] 链表节点定义
来源：http://ix.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qx.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qw.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fs.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vy.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://xg.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ys.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ik.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qm.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://mj.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://is.521024.cn

PHP:  // 手写递归函数
来源：http://ej.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xn.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://my.szxytkj.cn

Java: // 手写递归
来源：http://sr.hnjuh.cn

Go:   // 手写递归
来源：http://qv.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xk.yuntaijiaju.cn

C#:   // 手写递归
来源：http://tw.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ye.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gi.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gn.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gz.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://go.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yp.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wd.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://br.szsharing.cn

================================================================================
来源：http://xu.gzmigu.cn

O. 并发与异步
来源：http://qp.panjiajie.cn

================================================================================
来源：http://oc.bjjhwx.cn

[O01] 启动一个线程
来源：http://uq.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mx.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lr.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zb.jctech888.com.cn

TS:   // 同 JS
来源：http://in.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://hi.panjiajie.cn

Go:   go f()
来源：http://jp.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://ba.9csxet.cn

C#:   Task.Run(() => F());
来源：http://hb.szsharing.cn

[O02] 使用线程池
来源：http://yo.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lj.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ar.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://zo.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://ti.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://js.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tx.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sy.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://np.colortex.cn

[O03] 加锁保护共享数据
来源：http://mc.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://yl.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://zs.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ao.szxytkj.cn

TS:   // 同 JS
来源：http://vh.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://mc.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hr.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ft.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://kk.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://fn.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://dm.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ww.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://qd.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yp.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lk.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mp.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ba.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://vg.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://uj.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://pb.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rh.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://di.521024.cn

TS:   await Promise.all(tasks)
来源：http://wl.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://li.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sa.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://xw.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jo.521024.cn

[O06] 使用进程池
来源：http://uw.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rj.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nc.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://da.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://ic.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://js.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wc.huixiangedu.cn

Ruby: // fork 块
来源：http://ms.huixinmuqiang.cn

C#:   Parallel.For
来源：http://cm.colortex.cn

================================================================================
来源：http://pn.yuexingan06.cn

P. 常用工具函数
来源：http://jk.nszjky.cn

================================================================================
来源：http://mb.haigaiapp.cn

[P01] 生成 UUID
来源：http://ln.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://cl.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nq.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://of.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://xx.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://zt.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://rk.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://yp.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://ge.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://dl.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qn.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mk.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vp.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sb.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lb.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lg.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nk.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rm.colortex.cn

[P03] 生成短随机字符串
来源：http://qi.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qz.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cv.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sd.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ef.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nc.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ub.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://py.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://he.yuntaijiaju.cn

[P04] 求长度
来源：http://kv.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qw.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zr.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zh.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jf.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://kr.hahajie.cn

Go:   len(arr);  len(m)
来源：http://bl.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://vj.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bv.shxzukj.cn


<!-- 参考信息 -->