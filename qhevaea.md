代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://em.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lf.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vf.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://qq.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://dd.jctech888.com.cn

Java: resp.statusCode()
来源：http://cs.szxytkj.cn

Go:   resp.StatusCode
来源：http://bn.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://jn.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://kp.9csxet.cn

[L08] 并发请求多个地址
来源：http://kp.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kj.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ww.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mk.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gc.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fx.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ii.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ew.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lb.huanxung.cn

================================================================================
来源：http://az.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://vp.shtwfgs.cn

================================================================================
来源：http://by.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ho.shxzskj.cn

Py:   sys.argv[1:]
来源：http://pv.521024.cn

PHP:  $argv;  $argc;
来源：http://pk.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://qg.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://gl.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://nu.nicolike.cn

Go:   os.Args[1:]
来源：http://po.bookmarksfly.cn

Ruby: ARGV
来源：http://zs.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://ix.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://xg.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://su.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eu.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://yc.hahajie.cn

TS:   process.env.HOME
来源：http://zu.newstarts.cn

Java: System.getenv("HOME")
来源：http://jr.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://co.huanxung.cn

Ruby: ENV["HOME"]
来源：http://zr.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fx.shxzukj.cn

[M03] 执行外部命令
来源：http://fl.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gx.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kj.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nm.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uu.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zx.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qh.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sq.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://fu.gzmigu.cn

[M04] 获取当前工作目录
来源：http://ar.asd995.cn

Py:   os.getcwd()
来源：http://dw.lnxyls.cn

PHP:  getcwd();
来源：http://vc.521024.cn

JS:   process.cwd()
来源：http://vk.9csxet.cn

TS:   process.cwd()
来源：http://sx.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://hd.9csxet.cn

Go:   os.Getwd()
来源：http://dm.nszjky.cn

Ruby: Dir.pwd
来源：http://ph.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gt.szsharing.cn

[M05] 设置退出码
来源：http://xd.shxzskj.cn

Py:   sys.exit(1)
来源：http://tv.hnjuh.cn

PHP:  exit(1);
来源：http://ih.9csxet.cn

JS:   process.exit(1)
来源：http://lg.yuexingan06.cn

TS:   process.exit(1)
来源：http://pg.jianghongdianzi.cn

Java: System.exit(1)
来源：http://fg.lnxyls.cn

Go:   os.Exit(1)
来源：http://dn.yuexingan06.cn

Ruby: exit 1
来源：http://ap.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bl.hnjuh.cn

[M06] 向标准错误输出
来源：http://pz.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://vh.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://la.nicolike.cn

JS:   console.error("err")
来源：http://qz.huixiangedu.cn

TS:   console.error("err")
来源：http://ci.muxihuayi.cn

Java: System.err.println("err")
来源：http://ri.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ew.lnxyls.cn

Ruby: warn "err"
来源：http://kb.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ql.shxzukj.cn

[M07] 判断是否为主入口
来源：http://oh.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://xn.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cr.yuexingan06.cn

JS:   require.main === module
来源：http://yh.asd995.cn

TS:   require.main === module
来源：http://xg.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://th.bjjhwx.cn

Go:   func main()
来源：http://au.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yh.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://sr.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://xy.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://nm.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://as.shxzukj.cn

JS:   process.platform;  process.version
来源：http://wm.nicolike.cn

TS:   process.platform;  process.version
来源：http://tz.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://en.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jt.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hf.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://te.jianghongdianzi.cn

================================================================================
来源：http://rf.huanxung.cn

N. 数据结构与算法
来源：http://jk.jianghongdianzi.cn

================================================================================
来源：http://qa.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://io.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ei.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mp.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vs.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jy.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zf.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://xt.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vm.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aq.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://na.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ya.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://st.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pd.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nd.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wa.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://wt.nszjky.cn

Ruby: arr.sort
来源：http://nj.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vi.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://pc.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kk.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://qu.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xh.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wf.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ze.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cw.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vm.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://lc.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://af.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ba.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gj.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://li.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://df.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kp.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://at.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oy.jctech888.com.cn

[N05] 最大公约数
来源：http://qc.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://za.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bz.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yu.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://im.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mx.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zg.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://en.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rf.huanxung.cn

[N06] 判断回文字符串
来源：http://ob.szxytkj.cn

Py:   s == s[::-1]
来源：http://pm.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://uu.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://jx.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://oq.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mg.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://rd.bjjhwx.cn

Ruby: s == s.reverse
来源：http://sm.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pu.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://rv.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ai.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fj.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bk.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://iu.shtwfgs.cn

Java: // 手写 HashMap
来源：http://ku.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://yv.hahajie.cn

Ruby: // 手写 Hash
来源：http://vf.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ob.huixiangedu.cn

[N08] 生成全排列
来源：http://pm.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://wc.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://jv.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://bg.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://cf.shxzskj.cn

Java: // 手写回溯递归
来源：http://wp.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://zl.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://xq.panjiajie.cn

C#:   // 手写回溯递归
来源：http://vd.colortex.cn

[N09] 栈与队列
来源：http://rn.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xu.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wd.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jf.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qk.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aj.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lf.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nj.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nx.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ma.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nm.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gc.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wu.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pk.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://yc.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qc.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dr.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://az.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://au.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oi.gzmigu.cn

PHP:  // 手写递归函数
来源：http://jj.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sx.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.panjiajie.cn

Java: // 手写递归
来源：http://sd.szxytkj.cn

Go:   // 手写递归
来源：http://ql.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vp.nszjky.cn

C#:   // 手写递归
来源：http://ro.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ml.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fh.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nm.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kg.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mh.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pz.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bz.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yo.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dy.nszjky.cn

================================================================================
来源：http://ez.yuexingan06.cn

O. 并发与异步
来源：http://ps.nszjky.cn

================================================================================
来源：http://rw.newstarts.cn

[O01] 启动一个线程
来源：http://lk.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iq.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oy.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rd.yuntaijiaju.cn

TS:   // 同 JS
来源：http://an.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://ml.haigaiapp.cn

Go:   go f()
来源：http://lm.521024.cn

Ruby: Thread.new { f }
来源：http://su.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://hx.hahajie.cn

[O02] 使用线程池
来源：http://qc.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://da.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qx.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://ef.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://tr.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://na.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://br.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vg.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cs.asd995.cn

[O03] 加锁保护共享数据
来源：http://nr.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://wx.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://ub.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iz.panjiajie.cn

TS:   // 同 JS
来源：http://nn.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://ba.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ov.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ea.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://zt.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://hj.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://lx.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uy.colortex.cn

JS:   async function f() { await g(); }
来源：http://du.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pz.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kw.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jk.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cy.colortex.cn

C#:   async Task F() { await G(); }
来源：http://qs.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://dd.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://vw.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yr.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://lx.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://zl.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yr.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ks.nicolike.cn

Ruby: threads.map(&:join)
来源：http://ra.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bp.gzmigu.cn

[O06] 使用进程池
来源：http://hq.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ba.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kx.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://gv.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://em.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hr.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dq.wgjwhj.cn

Ruby: // fork 块
来源：http://xx.haigaiapp.cn

C#:   Parallel.For
来源：http://rt.wgjwhj.cn

================================================================================
来源：http://ny.colortex.cn

P. 常用工具函数
来源：http://sc.chemitech.net.cn

================================================================================
来源：http://wj.yuexingan06.cn

[P01] 生成 UUID
来源：http://yg.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://bq.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zk.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://ya.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://uq.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://um.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://rb.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://do.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://fg.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://qa.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mv.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ph.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wi.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vm.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xc.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qx.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kh.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qi.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://oz.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fu.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cj.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zb.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bp.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ft.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gk.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ce.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ly.chemitech.net.cn

[P04] 求长度
来源：http://qk.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bl.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://so.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ul.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zh.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://zh.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://he.hahajie.cn

Ruby: x.length;  x.size
来源：http://pv.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zq.jctech888.com.cn


<!-- 参考信息 -->