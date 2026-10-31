代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://fv.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pj.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kw.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://qm.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://qc.panjiajie.cn

Java: resp.statusCode()
来源：http://sl.colortex.cn

Go:   resp.StatusCode
来源：http://hq.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://th.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://mo.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ye.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wt.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://xf.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://di.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jt.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://of.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://ul.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://jp.huanxung.cn

================================================================================
来源：http://gg.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://km.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://nn.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://pa.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://kl.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://as.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://qp.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ln.szsharing.cn

Ruby: ARGV
来源：http://hb.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://ue.huixiangedu.cn

[M02] 读取环境变量
来源：http://lt.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://jc.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qg.panjiajie.cn

JS:   process.env.HOME
来源：http://rl.colortex.cn

TS:   process.env.HOME
来源：http://nm.hnjuh.cn

Java: System.getenv("HOME")
来源：http://le.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.asd995.cn

Ruby: ENV["HOME"]
来源：http://nu.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wt.jctech888.com.cn

[M03] 执行外部命令
来源：http://bm.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lx.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tp.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hr.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mq.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://py.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jr.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lf.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://vg.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://cs.muxihuayi.cn

Py:   os.getcwd()
来源：http://hc.huixiangedu.cn

PHP:  getcwd();
来源：http://bu.521024.cn

JS:   process.cwd()
来源：http://zu.wgjwhj.cn

TS:   process.cwd()
来源：http://hy.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://xc.nicolike.cn

Go:   os.Getwd()
来源：http://nv.muxihuayi.cn

Ruby: Dir.pwd
来源：http://tt.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sk.shxzukj.cn

[M05] 设置退出码
来源：http://px.9csxet.cn

Py:   sys.exit(1)
来源：http://la.shtwfgs.cn

PHP:  exit(1);
来源：http://zo.muxihuayi.cn

JS:   process.exit(1)
来源：http://jr.huixiangedu.cn

TS:   process.exit(1)
来源：http://wu.lnxyls.cn

Java: System.exit(1)
来源：http://yi.muxihuayi.cn

Go:   os.Exit(1)
来源：http://xt.bjjhwx.cn

Ruby: exit 1
来源：http://tr.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nn.shxzukj.cn

[M06] 向标准错误输出
来源：http://zf.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://db.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bw.jctech888.com.cn

JS:   console.error("err")
来源：http://dy.chemitech.net.cn

TS:   console.error("err")
来源：http://ur.nszjky.cn

Java: System.err.println("err")
来源：http://eg.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ny.521024.cn

Ruby: warn "err"
来源：http://rd.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ch.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://lw.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://za.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wh.muxihuayi.cn

JS:   require.main === module
来源：http://vv.bjjhwx.cn

TS:   require.main === module
来源：http://dy.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://dn.newstarts.cn

Go:   func main()
来源：http://tr.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://om.asd995.cn

C#:   static void Main(string[] args)
来源：http://tp.521024.cn

[M08] 获取系统与运行时信息
来源：http://qm.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://io.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://cy.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://yd.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://pb.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://px.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dp.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rt.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://es.lnxyls.cn

================================================================================
来源：http://le.9csxet.cn

N. 数据结构与算法
来源：http://ki.jctech888.com.cn

================================================================================
来源：http://xh.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://cv.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cq.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vu.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hd.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oa.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jz.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://yu.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fk.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kr.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://cj.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://gd.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://du.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oa.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iw.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hu.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://vk.hnjuh.cn

Ruby: arr.sort
来源：http://je.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xf.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://tj.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://sl.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zv.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xd.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jp.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://de.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dg.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ka.asd995.cn

[N04] 斐波那契数列
来源：http://ri.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gu.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fo.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ac.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eu.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jx.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ap.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sm.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ny.muxihuayi.cn

[N05] 最大公约数
来源：http://sl.nszjky.cn

Py:   math.gcd(a, b)
来源：http://zw.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yk.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fn.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hq.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sj.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ph.521024.cn

Ruby: a.gcd(b)
来源：http://rg.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://re.muxihuayi.cn

[N06] 判断回文字符串
来源：http://fk.panjiajie.cn

Py:   s == s[::-1]
来源：http://py.521024.cn

PHP:  $s === strrev($s);
来源：http://ym.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://nu.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://dl.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oq.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://pz.jctech888.com.cn

Ruby: s == s.reverse
来源：http://qa.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xs.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://os.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mx.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ot.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://ya.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://kg.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://xz.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://us.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://os.newstarts.cn

[N08] 生成全排列
来源：http://eq.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://kq.asd995.cn

PHP:  // 手写递归交换
来源：http://al.shxzukj.cn

JS:   // 手写回溯递归
来源：http://xe.szsharing.cn

TS:   // 手写回溯递归
来源：http://xu.hnjuh.cn

Java: // 手写回溯递归
来源：http://sj.hnjuh.cn

Go:   // 手写回溯递归
来源：http://al.asd995.cn

Ruby: arr.permutation.to_a
来源：http://lp.gzmigu.cn

C#:   // 手写回溯递归
来源：http://xz.huixinmuqiang.cn

[N09] 栈与队列
来源：http://ih.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pt.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tr.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fv.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ka.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hm.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ns.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xb.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yf.shxzukj.cn

[N10] 链表节点定义
来源：http://wn.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cv.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ol.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uz.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nl.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://xb.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qr.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bd.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kl.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://le.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ol.colortex.cn

PHP:  // 手写递归函数
来源：http://hv.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lp.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wr.haigaiapp.cn

Java: // 手写递归
来源：http://zv.hahajie.cn

Go:   // 手写递归
来源：http://xg.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://an.colortex.cn

C#:   // 手写递归
来源：http://ab.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ql.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jx.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pt.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://du.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mm.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pr.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mo.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ey.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.nszjky.cn

================================================================================
来源：http://ix.huixinmuqiang.cn

O. 并发与异步
来源：http://me.panjiajie.cn

================================================================================
来源：http://yx.panjiajie.cn

[O01] 启动一个线程
来源：http://pu.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hs.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gb.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bv.wgjwhj.cn

TS:   // 同 JS
来源：http://lw.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://xi.newstarts.cn

Go:   go f()
来源：http://ew.shxzukj.cn

Ruby: Thread.new { f }
来源：http://xh.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://nq.yuntaijiaju.cn

[O02] 使用线程池
来源：http://wr.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iu.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://es.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://tx.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://xe.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qn.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ul.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dc.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://st.nicolike.cn

[O03] 加锁保护共享数据
来源：http://rc.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://jw.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://jt.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cz.huixinmuqiang.cn

TS:   // 同 JS
来源：http://sf.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://go.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lf.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uu.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://bk.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://zc.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://ei.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kh.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://dh.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nd.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zg.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iv.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pl.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://sl.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://zh.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://tq.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lg.asd995.cn

JS:   await Promise.all(tasks)
来源：http://wt.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://zs.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cb.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ue.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://rq.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gu.szsharing.cn

[O06] 使用进程池
来源：http://zd.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yg.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://os.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://il.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://wg.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tx.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yr.jianghongdianzi.cn

Ruby: // fork 块
来源：http://qi.nicolike.cn

C#:   Parallel.For
来源：http://wv.huixiangedu.cn

================================================================================
来源：http://jr.gzmigu.cn

P. 常用工具函数
来源：http://ck.wgjwhj.cn

================================================================================
来源：http://ge.szsharing.cn

[P01] 生成 UUID
来源：http://at.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://wi.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iq.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://yw.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://pu.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://og.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://wg.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://wu.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://wx.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ps.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rg.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vi.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qt.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ck.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fr.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eg.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://au.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aq.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://za.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hu.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gf.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zh.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://in.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pu.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fz.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oo.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yf.szsharing.cn

[P04] 求长度
来源：http://sa.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cl.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lr.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dn.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qt.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://cr.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://iu.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://hl.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zp.shtwfgs.cn


<!-- 参考信息 -->