代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cf.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://si.shxzukj.cn

================================================================================
来源：http://dl.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://sg.bookmarksfly.cn

================================================================================
来源：http://ws.521024.cn

[M01] 读取命令行参数
来源：http://ej.gzmigu.cn

Py:   sys.argv[1:]
来源：http://op.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://mh.nszjky.cn

JS:   process.argv.slice(2)
来源：http://vl.9csxet.cn

TS:   process.argv.slice(2)
来源：http://zc.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://ab.hnjuh.cn

Go:   os.Args[1:]
来源：http://ov.jctech888.com.cn

Ruby: ARGV
来源：http://ru.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://es.jctech888.com.cn

[M02] 读取环境变量
来源：http://xd.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://bb.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cu.chemitech.net.cn

JS:   process.env.HOME
来源：http://rv.bjjhwx.cn

TS:   process.env.HOME
来源：http://ia.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ul.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oo.9csxet.cn

Ruby: ENV["HOME"]
来源：http://wc.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://md.huixiangedu.cn

[M03] 执行外部命令
来源：http://ak.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zc.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ep.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pq.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ds.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xa.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cy.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://av.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://yn.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ot.nicolike.cn

Py:   os.getcwd()
来源：http://fn.huixiangedu.cn

PHP:  getcwd();
来源：http://wk.nszjky.cn

JS:   process.cwd()
来源：http://is.shxzukj.cn

TS:   process.cwd()
来源：http://vj.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://fp.chemitech.net.cn

Go:   os.Getwd()
来源：http://pg.9csxet.cn

Ruby: Dir.pwd
来源：http://hs.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ha.szsharing.cn

[M05] 设置退出码
来源：http://ce.9csxet.cn

Py:   sys.exit(1)
来源：http://hp.panjiajie.cn

PHP:  exit(1);
来源：http://nd.shxzskj.cn

JS:   process.exit(1)
来源：http://kn.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://vd.bjjhwx.cn

Java: System.exit(1)
来源：http://qa.9csxet.cn

Go:   os.Exit(1)
来源：http://qa.szsharing.cn

Ruby: exit 1
来源：http://ml.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://st.szxytkj.cn

[M06] 向标准错误输出
来源：http://rs.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://um.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mb.huixinmuqiang.cn

JS:   console.error("err")
来源：http://xn.gzmigu.cn

TS:   console.error("err")
来源：http://va.521024.cn

Java: System.err.println("err")
来源：http://vq.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nr.hahajie.cn

Ruby: warn "err"
来源：http://li.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ls.9csxet.cn

[M07] 判断是否为主入口
来源：http://wr.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://xh.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uz.shtwfgs.cn

JS:   require.main === module
来源：http://gf.wgjwhj.cn

TS:   require.main === module
来源：http://bc.nicolike.cn

Java: public static void main(String[] args)
来源：http://hu.nicolike.cn

Go:   func main()
来源：http://lm.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zy.newstarts.cn

C#:   static void Main(string[] args)
来源：http://wt.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://kl.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://we.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://xn.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://zx.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://cq.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mx.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://da.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hh.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mh.yuexingan06.cn

================================================================================
来源：http://vk.shxzskj.cn

N. 数据结构与算法
来源：http://jk.huanxung.cn

================================================================================
来源：http://pr.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://yp.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uv.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vz.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kc.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qa.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ms.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://ge.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rr.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ah.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://ck.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ub.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aa.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hf.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oy.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ch.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ec.colortex.cn

Ruby: arr.sort
来源：http://ya.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yk.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://yx.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lw.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://gf.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pe.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gv.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://se.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://it.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uv.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ea.muxihuayi.cn

[N04] 斐波那契数列
来源：http://eo.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://al.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jp.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bv.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ia.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zc.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uf.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fo.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vn.hahajie.cn

[N05] 最大公约数
来源：http://tx.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://dc.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ym.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pi.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://st.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hj.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ms.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://vq.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cj.shxzskj.cn

[N06] 判断回文字符串
来源：http://gm.wgjwhj.cn

Py:   s == s[::-1]
来源：http://tg.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://xn.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ko.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://fd.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://na.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://wq.yuexingan06.cn

Ruby: s == s.reverse
来源：http://uu.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://na.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://vk.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ix.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xv.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yv.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://ul.yuexingan06.cn

Java: // 手写 HashMap
来源：http://cm.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://lz.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ew.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oh.asd995.cn

[N08] 生成全排列
来源：http://wp.colortex.cn

Py:   itertools.permutations(arr)
来源：http://dc.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://xe.hnjuh.cn

JS:   // 手写回溯递归
来源：http://vu.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://ld.wgjwhj.cn

Java: // 手写回溯递归
来源：http://id.9csxet.cn

Go:   // 手写回溯递归
来源：http://nw.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://fn.newstarts.cn

C#:   // 手写回溯递归
来源：http://te.nszjky.cn

[N09] 栈与队列
来源：http://uv.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kd.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://at.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jq.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jq.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jx.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://va.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ec.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gh.szsharing.cn

[N10] 链表节点定义
来源：http://ko.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wq.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mk.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sx.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ey.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://qu.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kl.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jp.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zi.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://zf.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nf.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://zv.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qe.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.wgjwhj.cn

Java: // 手写递归
来源：http://yp.haigaiapp.cn

Go:   // 手写递归
来源：http://am.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kb.panjiajie.cn

C#:   // 手写递归
来源：http://lm.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gf.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qc.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cb.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ap.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yg.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rg.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ht.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ie.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mv.lnxyls.cn

================================================================================
来源：http://kp.shtwfgs.cn

O. 并发与异步
来源：http://ii.szsharing.cn

================================================================================
来源：http://qv.yuexingan06.cn

[O01] 启动一个线程
来源：http://ew.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ek.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ei.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dj.huixinmuqiang.cn

TS:   // 同 JS
来源：http://gd.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://sq.jctech888.com.cn

Go:   go f()
来源：http://oe.nicolike.cn

Ruby: Thread.new { f }
来源：http://el.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://al.521024.cn

[O02] 使用线程池
来源：http://cx.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wg.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xb.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://mc.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://mg.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ko.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zz.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ri.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sg.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://au.nicolike.cn

Py:   with lock: shared += 1
来源：http://ch.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gl.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pe.yuexingan06.cn

TS:   // 同 JS
来源：http://gp.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://vh.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hm.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://us.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://wy.nicolike.cn

[O04] 定义异步函数并等待
来源：http://fk.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://vg.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://av.9csxet.cn

JS:   async function f() { await g(); }
来源：http://fm.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ty.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sv.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ic.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pz.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ex.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://av.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ps.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://or.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ld.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://cm.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://co.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oo.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://ok.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://md.nicolike.cn

[O06] 使用进程池
来源：http://og.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ik.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sb.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://qn.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://xe.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://np.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ub.shtwfgs.cn

Ruby: // fork 块
来源：http://ui.szsharing.cn

C#:   Parallel.For
来源：http://js.muxihuayi.cn

================================================================================
来源：http://mo.yuexingan06.cn

P. 常用工具函数
来源：http://wl.yuexingan06.cn

================================================================================
来源：http://uh.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://cp.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://uf.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://se.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://ee.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://hd.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://et.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://nn.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://yc.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://sz.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://fo.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xd.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fu.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qd.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qn.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qg.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nd.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dd.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rs.szsharing.cn

[P03] 生成短随机字符串
来源：http://uw.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yj.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yg.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yc.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wy.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oc.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oz.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://di.huixinmuqiang.cn

[P04] 求长度
来源：http://us.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ym.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rp.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vn.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://my.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://sb.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://iq.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://nh.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tt.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://lq.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://du.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cv.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ss.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tr.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fm.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mm.wgjwhj.cn

Ruby: a == b
来源：http://rj.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pl.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kc.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ap.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://nj.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://of.gzmigu.cn

TS:   if (x == null) {}
来源：http://dr.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fi.muxihuayi.cn

Go:   if x == nil {}
来源：http://ia.newstarts.cn


<!-- 参考信息 -->