代发 wailian999

TS:   resp.ok;  resp.status
来源：http://rt.shtwfgs.cn

Java: resp.statusCode()
来源：http://bk.hahajie.cn

Go:   resp.StatusCode
来源：http://ey.lnxyls.cn

Ruby: resp.code.to_i
来源：http://ei.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://gp.huanxung.cn

[L08] 并发请求多个地址
来源：http://rn.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fp.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://bq.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://um.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://si.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gd.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://br.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yg.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mc.chemitech.net.cn

================================================================================
来源：http://eu.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://dy.shxzskj.cn

================================================================================
来源：http://rm.huanxung.cn

[M01] 读取命令行参数
来源：http://tj.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ns.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://is.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://jl.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://si.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://rj.hahajie.cn

Go:   os.Args[1:]
来源：http://sl.yuexingan06.cn

Ruby: ARGV
来源：http://go.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://dj.colortex.cn

[M02] 读取环境变量
来源：http://yn.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://kr.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hy.haigaiapp.cn

JS:   process.env.HOME
来源：http://ly.newstarts.cn

TS:   process.env.HOME
来源：http://ua.hahajie.cn

Java: System.getenv("HOME")
来源：http://pt.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zc.9csxet.cn

Ruby: ENV["HOME"]
来源：http://sn.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zu.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://lm.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ao.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ek.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dv.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wp.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iq.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fl.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zz.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://qm.521024.cn

[M04] 获取当前工作目录
来源：http://nk.colortex.cn

Py:   os.getcwd()
来源：http://nv.yuntaijiaju.cn

PHP:  getcwd();
来源：http://wj.nszjky.cn

JS:   process.cwd()
来源：http://gg.nicolike.cn

TS:   process.cwd()
来源：http://ib.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://qy.hahajie.cn

Go:   os.Getwd()
来源：http://ie.newstarts.cn

Ruby: Dir.pwd
来源：http://rx.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://og.hnjuh.cn

[M05] 设置退出码
来源：http://nv.lnxyls.cn

Py:   sys.exit(1)
来源：http://nu.asd995.cn

PHP:  exit(1);
来源：http://da.jctech888.com.cn

JS:   process.exit(1)
来源：http://yy.shxzskj.cn

TS:   process.exit(1)
来源：http://ej.lnxyls.cn

Java: System.exit(1)
来源：http://zn.nicolike.cn

Go:   os.Exit(1)
来源：http://pj.521024.cn

Ruby: exit 1
来源：http://it.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rr.nszjky.cn

[M06] 向标准错误输出
来源：http://sa.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://im.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rz.colortex.cn

JS:   console.error("err")
来源：http://tf.yuexingan06.cn

TS:   console.error("err")
来源：http://hg.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ln.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ia.chemitech.net.cn

Ruby: warn "err"
来源：http://hk.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://jv.szsharing.cn

[M07] 判断是否为主入口
来源：http://fj.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://lf.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mv.huixiangedu.cn

JS:   require.main === module
来源：http://cn.muxihuayi.cn

TS:   require.main === module
来源：http://gi.hnjuh.cn

Java: public static void main(String[] args)
来源：http://nx.chemitech.net.cn

Go:   func main()
来源：http://rx.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hh.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://ty.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://le.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://sl.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://wf.szsharing.cn

JS:   process.platform;  process.version
来源：http://rt.szxytkj.cn

TS:   process.platform;  process.version
来源：http://xl.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aq.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vc.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ek.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bz.jianghongdianzi.cn

================================================================================
来源：http://pz.gzmigu.cn

N. 数据结构与算法
来源：http://iq.szxytkj.cn

================================================================================
来源：http://zb.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://cf.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://el.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mi.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://va.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uh.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yl.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://mv.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fm.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mp.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://mk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://mx.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://en.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fc.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nk.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zl.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://sc.shtwfgs.cn

Ruby: arr.sort
来源：http://uc.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mw.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://xp.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qx.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://ox.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xw.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pc.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ca.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ro.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ad.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://le.szsharing.cn

[N04] 斐波那契数列
来源：http://lc.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sh.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mq.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://px.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bw.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sa.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dz.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xr.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xw.nicolike.cn

[N05] 最大公约数
来源：http://gh.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ia.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rl.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yq.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tv.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fb.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fz.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://cy.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tn.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://pm.shtwfgs.cn

Py:   s == s[::-1]
来源：http://na.huanxung.cn

PHP:  $s === strrev($s);
来源：http://yw.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://vm.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://re.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ni.nszjky.cn

Go:   // 双指针从两端比较
来源：http://re.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://jz.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ui.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://dt.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oj.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wg.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yk.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://tc.lnxyls.cn

Java: // 手写 HashMap
来源：http://zu.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://zn.nicolike.cn

Ruby: // 手写 Hash
来源：http://fj.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://id.nicolike.cn

[N08] 生成全排列
来源：http://im.colortex.cn

Py:   itertools.permutations(arr)
来源：http://uf.521024.cn

PHP:  // 手写递归交换
来源：http://zj.hahajie.cn

JS:   // 手写回溯递归
来源：http://wj.nszjky.cn

TS:   // 手写回溯递归
来源：http://bl.nicolike.cn

Java: // 手写回溯递归
来源：http://vs.hahajie.cn

Go:   // 手写回溯递归
来源：http://go.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://ep.huanxung.cn

C#:   // 手写回溯递归
来源：http://kc.asd995.cn

[N09] 栈与队列
来源：http://qn.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tr.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ju.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xq.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qd.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pl.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zh.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nk.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://px.bookmarksfly.cn

[N10] 链表节点定义
来源：http://qz.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yc.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yy.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zz.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ga.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://pm.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ib.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://il.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vc.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://yp.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oy.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://vj.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sr.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xo.muxihuayi.cn

Java: // 手写递归
来源：http://nh.nszjky.cn

Go:   // 手写递归
来源：http://wh.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ct.asd995.cn

C#:   // 手写递归
来源：http://dj.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fr.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hf.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cz.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ws.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gc.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qx.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mq.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gj.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iy.gzmigu.cn

================================================================================
来源：http://he.muxihuayi.cn

O. 并发与异步
来源：http://cv.9csxet.cn

================================================================================
来源：http://xr.newstarts.cn

[O01] 启动一个线程
来源：http://jt.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uc.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://of.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ed.newstarts.cn

TS:   // 同 JS
来源：http://uy.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://fb.huixiangedu.cn

Go:   go f()
来源：http://lv.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://jd.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://as.nszjky.cn

[O02] 使用线程池
来源：http://ti.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ah.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cy.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://gf.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://jq.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qe.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://br.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dm.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nk.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://kt.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://ze.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://gb.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wi.szsharing.cn

TS:   // 同 JS
来源：http://vi.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://xh.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ar.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jq.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://sg.huanxung.cn

[O04] 定义异步函数并等待
来源：http://ty.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://qt.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://im.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://im.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ol.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gv.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vk.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jm.asd995.cn

C#:   async Task F() { await G(); }
来源：http://eq.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://kd.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ch.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vt.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://ov.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://jm.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zj.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ka.huanxung.cn

Ruby: threads.map(&:join)
来源：http://oj.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pt.9csxet.cn

[O06] 使用进程池
来源：http://xc.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zg.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://py.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://bc.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://ij.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fo.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fv.hahajie.cn

Ruby: // fork 块
来源：http://ab.shxzukj.cn

C#:   Parallel.For
来源：http://zv.shxzukj.cn

================================================================================
来源：http://dw.panjiajie.cn

P. 常用工具函数
来源：http://ka.muxihuayi.cn

================================================================================
来源：http://ku.asd995.cn

[P01] 生成 UUID
来源：http://cr.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://ep.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lg.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://qm.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://zx.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://jb.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://zs.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://nw.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://qw.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://ef.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sy.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oe.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qe.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wl.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fh.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mc.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rn.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ca.colortex.cn

[P03] 生成短随机字符串
来源：http://vn.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://km.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sz.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pp.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://be.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sm.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rn.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ot.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kf.szxytkj.cn

[P04] 求长度
来源：http://vj.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bj.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gk.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gl.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nv.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://em.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://eg.lnxyls.cn

Ruby: x.length;  x.size
来源：http://uk.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yw.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ik.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ze.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yk.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aq.bjjhwx.cn


<!-- 参考信息 -->