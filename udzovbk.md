代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://uj.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aj.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xk.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://me.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ui.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://ux.haigaiapp.cn

Go:   resp.StatusCode
来源：http://fh.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://tv.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://sc.panjiajie.cn

[L08] 并发请求多个地址
来源：http://qy.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xf.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://ng.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rm.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cd.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yd.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zw.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ia.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hh.szxytkj.cn

================================================================================
来源：http://ch.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ij.jctech888.com.cn

================================================================================
来源：http://os.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://rd.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://pt.9csxet.cn

PHP:  $argv;  $argc;
来源：http://mr.521024.cn

JS:   process.argv.slice(2)
来源：http://lt.9csxet.cn

TS:   process.argv.slice(2)
来源：http://tx.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://ur.521024.cn

Go:   os.Args[1:]
来源：http://wb.colortex.cn

Ruby: ARGV
来源：http://vc.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://mf.shxzukj.cn

[M02] 读取环境变量
来源：http://gf.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://yv.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vl.bjjhwx.cn

JS:   process.env.HOME
来源：http://xt.szxytkj.cn

TS:   process.env.HOME
来源：http://kd.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://nu.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rq.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://yq.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wo.bjjhwx.cn

[M03] 执行外部命令
来源：http://os.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rk.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ze.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://px.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lh.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vs.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pb.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://be.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://xb.521024.cn

[M04] 获取当前工作目录
来源：http://af.521024.cn

Py:   os.getcwd()
来源：http://rw.shxzskj.cn

PHP:  getcwd();
来源：http://os.hahajie.cn

JS:   process.cwd()
来源：http://vr.bjjhwx.cn

TS:   process.cwd()
来源：http://iw.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://eb.9csxet.cn

Go:   os.Getwd()
来源：http://la.haigaiapp.cn

Ruby: Dir.pwd
来源：http://ex.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.szsharing.cn

[M05] 设置退出码
来源：http://ng.wgjwhj.cn

Py:   sys.exit(1)
来源：http://ag.chemitech.net.cn

PHP:  exit(1);
来源：http://ag.shtwfgs.cn

JS:   process.exit(1)
来源：http://dx.panjiajie.cn

TS:   process.exit(1)
来源：http://ej.asd995.cn

Java: System.exit(1)
来源：http://gl.muxihuayi.cn

Go:   os.Exit(1)
来源：http://lm.shxzukj.cn

Ruby: exit 1
来源：http://np.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ok.huanxung.cn

[M06] 向标准错误输出
来源：http://bn.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://ya.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rd.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ye.asd995.cn

TS:   console.error("err")
来源：http://vx.szxytkj.cn

Java: System.err.println("err")
来源：http://ro.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ut.chemitech.net.cn

Ruby: warn "err"
来源：http://kb.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://at.huanxung.cn

[M07] 判断是否为主入口
来源：http://ls.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://qt.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vg.hnjuh.cn

JS:   require.main === module
来源：http://dh.chemitech.net.cn

TS:   require.main === module
来源：http://tw.shxzukj.cn

Java: public static void main(String[] args)
来源：http://lg.wgjwhj.cn

Go:   func main()
来源：http://ni.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zw.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://ap.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://bo.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://fw.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://tf.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://sq.hahajie.cn

TS:   process.platform;  process.version
来源：http://xi.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wx.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mp.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nr.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wk.jctech888.com.cn

================================================================================
来源：http://up.lnxyls.cn

N. 数据结构与算法
来源：http://ml.shtwfgs.cn

================================================================================
来源：http://nc.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://zl.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gp.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bv.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yw.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rp.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dx.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://ca.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ee.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rc.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ea.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://ct.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://og.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ba.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qk.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ur.newstarts.cn

Go:   slices.Sort(arr)
来源：http://jy.wgjwhj.cn

Ruby: arr.sort
来源：http://zz.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uc.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://rg.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ng.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://gc.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ol.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tm.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ef.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jb.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bg.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bz.shxzskj.cn

[N04] 斐波那契数列
来源：http://fm.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zm.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qd.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xw.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jw.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kp.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pc.hnjuh.cn

[N05] 最大公约数
来源：http://na.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://bi.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ru.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ph.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zx.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ec.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tn.asd995.cn

Ruby: a.gcd(b)
来源：http://yu.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nf.colortex.cn

[N06] 判断回文字符串
来源：http://fv.yuexingan06.cn

Py:   s == s[::-1]
来源：http://qy.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://iy.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://pl.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://di.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oq.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://pp.hahajie.cn

Ruby: s == s.reverse
来源：http://vf.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ws.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://yh.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zq.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kc.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kv.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://rn.lnxyls.cn

Java: // 手写 HashMap
来源：http://bu.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://uv.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://wl.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nk.haigaiapp.cn

[N08] 生成全排列
来源：http://nv.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://zu.nicolike.cn

PHP:  // 手写递归交换
来源：http://qn.huanxung.cn

JS:   // 手写回溯递归
来源：http://tt.lnxyls.cn

TS:   // 手写回溯递归
来源：http://oc.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://tm.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://fi.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://xn.521024.cn

C#:   // 手写回溯递归
来源：http://yh.lnxyls.cn

[N09] 栈与队列
来源：http://bt.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ct.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hy.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ww.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nc.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uf.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sv.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uj.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rm.gzmigu.cn

[N10] 链表节点定义
来源：http://xx.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ga.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ot.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jd.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xe.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://lp.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dq.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ot.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ey.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://po.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://je.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://lw.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ii.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://va.szsharing.cn

Java: // 手写递归
来源：http://if.yuexingan06.cn

Go:   // 手写递归
来源：http://wt.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pp.hnjuh.cn

C#:   // 手写递归
来源：http://vm.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dh.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://au.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ew.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bh.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ld.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lr.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ys.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iz.nicolike.cn

================================================================================
来源：http://qe.bookmarksfly.cn

O. 并发与异步
来源：http://dy.jianghongdianzi.cn

================================================================================
来源：http://yw.shxzskj.cn

[O01] 启动一个线程
来源：http://yp.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pn.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xs.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xh.shxzskj.cn

TS:   // 同 JS
来源：http://up.521024.cn

Java: new Thread(() -> f()).start()
来源：http://iq.hahajie.cn

Go:   go f()
来源：http://kv.lnxyls.cn

Ruby: Thread.new { f }
来源：http://tc.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://bw.yuntaijiaju.cn

[O02] 使用线程池
来源：http://kh.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fp.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vq.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://vo.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://cy.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ks.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://az.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://za.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nt.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://tg.szsharing.cn

Py:   with lock: shared += 1
来源：http://nd.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://yg.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kb.521024.cn

TS:   // 同 JS
来源：http://mj.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://ok.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qt.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ga.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://mj.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://nu.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://qv.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dx.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://dz.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ye.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fg.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://er.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kc.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://zm.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://pv.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://pm.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://em.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://bh.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://tq.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fb.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uq.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://kx.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ng.muxihuayi.cn

[O06] 使用进程池
来源：http://fc.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mz.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fg.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://rd.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://os.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zo.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hy.yuntaijiaju.cn

Ruby: // fork 块
来源：http://tz.panjiajie.cn

C#:   Parallel.For
来源：http://zu.lnxyls.cn

================================================================================
来源：http://rz.newstarts.cn

P. 常用工具函数
来源：http://qp.hahajie.cn

================================================================================
来源：http://ob.521024.cn

[P01] 生成 UUID
来源：http://ss.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://bq.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ep.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://bk.colortex.cn

TS:   crypto.randomUUID()
来源：http://fe.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://qm.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://aa.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://dy.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://pm.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://sj.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hn.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://df.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://on.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nt.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kv.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ic.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bq.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uo.nicolike.cn

[P03] 生成短随机字符串
来源：http://tb.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ac.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tz.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qm.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vw.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ia.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mc.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nn.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ft.szxytkj.cn

[P04] 求长度
来源：http://ed.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hp.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jj.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ww.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://rs.colortex.cn

Go:   len(arr);  len(m)
来源：http://yj.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://zl.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bl.shxzukj.cn


<!-- 参考信息 -->