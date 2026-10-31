代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://uy.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yc.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xo.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://oy.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://cx.gzmigu.cn

Java: resp.statusCode()
来源：http://bc.szsharing.cn

Go:   resp.StatusCode
来源：http://ne.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://lq.asd995.cn

C#:   (int)resp.StatusCode
来源：http://no.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://gp.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cz.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://eq.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hu.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://do.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ac.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uo.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vf.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jh.shxzukj.cn

================================================================================
来源：http://ef.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://ui.gzmigu.cn

================================================================================
来源：http://qq.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://ld.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://zs.huanxung.cn

PHP:  $argv;  $argc;
来源：http://rf.newstarts.cn

JS:   process.argv.slice(2)
来源：http://vg.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://tu.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://mm.gzmigu.cn

Go:   os.Args[1:]
来源：http://ww.nicolike.cn

Ruby: ARGV
来源：http://fh.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://gg.colortex.cn

[M02] 读取环境变量
来源：http://ky.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://qo.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uj.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://kl.muxihuayi.cn

TS:   process.env.HOME
来源：http://bo.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://kr.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qd.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://us.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ya.colortex.cn

[M03] 执行外部命令
来源：http://xl.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vm.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cp.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zn.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fw.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fp.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rs.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hv.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://mj.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://df.shtwfgs.cn

Py:   os.getcwd()
来源：http://cr.asd995.cn

PHP:  getcwd();
来源：http://db.bookmarksfly.cn

JS:   process.cwd()
来源：http://md.hnjuh.cn

TS:   process.cwd()
来源：http://qz.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://rd.521024.cn

Go:   os.Getwd()
来源：http://yy.9csxet.cn

Ruby: Dir.pwd
来源：http://ix.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kk.yuntaijiaju.cn

[M05] 设置退出码
来源：http://xo.muxihuayi.cn

Py:   sys.exit(1)
来源：http://sc.huixiangedu.cn

PHP:  exit(1);
来源：http://py.asd995.cn

JS:   process.exit(1)
来源：http://xm.asd995.cn

TS:   process.exit(1)
来源：http://st.nicolike.cn

Java: System.exit(1)
来源：http://ob.shxzukj.cn

Go:   os.Exit(1)
来源：http://ks.muxihuayi.cn

Ruby: exit 1
来源：http://hh.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xi.yuexingan06.cn

[M06] 向标准错误输出
来源：http://qj.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://is.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://an.lnxyls.cn

JS:   console.error("err")
来源：http://fa.huixiangedu.cn

TS:   console.error("err")
来源：http://jo.shtwfgs.cn

Java: System.err.println("err")
来源：http://ap.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ji.shxzukj.cn

Ruby: warn "err"
来源：http://vo.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://fe.hahajie.cn

[M07] 判断是否为主入口
来源：http://je.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://xn.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mh.huanxung.cn

JS:   require.main === module
来源：http://wn.9csxet.cn

TS:   require.main === module
来源：http://sn.nicolike.cn

Java: public static void main(String[] args)
来源：http://kd.colortex.cn

Go:   func main()
来源：http://ga.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nq.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://jy.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://pi.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://di.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://ti.asd995.cn

JS:   process.platform;  process.version
来源：http://zj.9csxet.cn

TS:   process.platform;  process.version
来源：http://cb.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wv.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xx.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zr.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.bjjhwx.cn

================================================================================
来源：http://ip.gzmigu.cn

N. 数据结构与算法
来源：http://zi.521024.cn

================================================================================
来源：http://lv.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://jm.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://de.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://di.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qo.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://im.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ae.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://tk.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iz.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ez.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://ec.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://rw.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://as.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bv.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zh.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hb.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://ok.nszjky.cn

Ruby: arr.sort
来源：http://tf.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yz.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://yb.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://js.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://wj.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ix.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hv.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cv.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://km.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wp.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oc.newstarts.cn

[N04] 斐波那契数列
来源：http://yu.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ft.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bl.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hv.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nn.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ya.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dr.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xu.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dk.jianghongdianzi.cn

[N05] 最大公约数
来源：http://fn.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://gl.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lj.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kt.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://co.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lb.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fh.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://zr.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gi.hnjuh.cn

[N06] 判断回文字符串
来源：http://ag.bjjhwx.cn

Py:   s == s[::-1]
来源：http://bt.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://zl.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://pu.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://vo.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wn.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://rg.shxzskj.cn

Ruby: s == s.reverse
来源：http://fj.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rl.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://ke.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wf.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kx.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gx.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://nh.9csxet.cn

Java: // 手写 HashMap
来源：http://il.szsharing.cn

Go:   // 手写 map[int]int
来源：http://cr.shxzukj.cn

Ruby: // 手写 Hash
来源：http://kq.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hb.szsharing.cn

[N08] 生成全排列
来源：http://wy.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://gn.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://tn.szsharing.cn

JS:   // 手写回溯递归
来源：http://ak.newstarts.cn

TS:   // 手写回溯递归
来源：http://nl.chemitech.net.cn

Java: // 手写回溯递归
来源：http://ww.9csxet.cn

Go:   // 手写回溯递归
来源：http://bw.asd995.cn

Ruby: arr.permutation.to_a
来源：http://tf.szxytkj.cn

C#:   // 手写回溯递归
来源：http://ot.huanxung.cn

[N09] 栈与队列
来源：http://nf.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sb.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ua.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kl.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ub.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nr.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cm.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tt.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jn.bookmarksfly.cn

[N10] 链表节点定义
来源：http://cm.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bb.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ct.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gb.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yp.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://da.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zp.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pq.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wl.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://sx.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://am.newstarts.cn

PHP:  // 手写递归函数
来源：http://qc.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ob.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hp.huanxung.cn

Java: // 手写递归
来源：http://td.huixiangedu.cn

Go:   // 手写递归
来源：http://ey.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://db.bookmarksfly.cn

C#:   // 手写递归
来源：http://ek.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qy.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ii.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ay.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://am.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pb.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fg.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rh.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gj.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tg.szxytkj.cn

================================================================================
来源：http://qy.szxytkj.cn

O. 并发与异步
来源：http://mt.muxihuayi.cn

================================================================================
来源：http://yj.yuexingan06.cn

[O01] 启动一个线程
来源：http://io.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mn.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ws.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bu.bookmarksfly.cn

TS:   // 同 JS
来源：http://ur.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://lj.panjiajie.cn

Go:   go f()
来源：http://st.szxytkj.cn

Ruby: Thread.new { f }
来源：http://kl.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://we.shtwfgs.cn

[O02] 使用线程池
来源：http://qm.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cy.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uy.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://in.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://pn.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ff.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sb.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hc.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qt.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://ya.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://lm.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://wk.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ol.lnxyls.cn

TS:   // 同 JS
来源：http://iu.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://rd.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xh.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cq.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://ow.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://mo.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://uc.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hr.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://wc.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fr.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wq.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fq.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jc.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://eo.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://xf.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://et.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wo.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://xj.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://zj.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dh.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ne.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gr.521024.cn

[O06] 使用进程池
来源：http://mg.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sw.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://po.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://ft.asd995.cn

TS:   // child_process / cluster 模块
来源：http://eg.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://br.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fz.bookmarksfly.cn

Ruby: // fork 块
来源：http://tl.szsharing.cn

C#:   Parallel.For
来源：http://sn.yuexingan06.cn

================================================================================
来源：http://yn.yuexingan06.cn

P. 常用工具函数
来源：http://vu.nszjky.cn

================================================================================
来源：http://ip.521024.cn

[P01] 生成 UUID
来源：http://ij.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://js.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xf.newstarts.cn

JS:   crypto.randomUUID()
来源：http://dv.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://ls.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://vy.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://rj.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://hx.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://fv.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://wa.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://in.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zl.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gn.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rl.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ho.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ar.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://js.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ot.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://yq.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ep.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ao.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ic.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yq.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kp.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fy.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nr.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ey.colortex.cn

[P04] 求长度
来源：http://nl.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ik.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gi.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vj.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cl.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://qq.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://gt.newstarts.cn

Ruby: x.length;  x.size
来源：http://lf.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ld.jctech888.com.cn


<!-- 参考信息 -->