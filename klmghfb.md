代发 wailian999

JS:   process.argv.slice(2)
来源：http://yn.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://nm.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://mg.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://zx.szxytkj.cn

Ruby: ARGV
来源：http://ix.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://iy.nicolike.cn

[M02] 读取环境变量
来源：http://fo.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://yz.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ox.shxzskj.cn

JS:   process.env.HOME
来源：http://eg.huixiangedu.cn

TS:   process.env.HOME
来源：http://ni.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://ix.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ta.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://ol.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ux.nicolike.cn

[M03] 执行外部命令
来源：http://rw.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sq.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fs.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dt.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dv.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ab.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nd.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mh.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://iw.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://bj.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://zu.szsharing.cn

PHP:  getcwd();
来源：http://cs.lnxyls.cn

JS:   process.cwd()
来源：http://ud.lnxyls.cn

TS:   process.cwd()
来源：http://wg.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://mt.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://gq.szxytkj.cn

Ruby: Dir.pwd
来源：http://qd.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xr.colortex.cn

[M05] 设置退出码
来源：http://bb.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://aw.gzmigu.cn

PHP:  exit(1);
来源：http://ym.panjiajie.cn

JS:   process.exit(1)
来源：http://ok.jctech888.com.cn

TS:   process.exit(1)
来源：http://fc.nszjky.cn

Java: System.exit(1)
来源：http://oe.panjiajie.cn

Go:   os.Exit(1)
来源：http://jy.szsharing.cn

Ruby: exit 1
来源：http://zh.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ma.9csxet.cn

[M06] 向标准错误输出
来源：http://ue.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://ci.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://in.huixinmuqiang.cn

JS:   console.error("err")
来源：http://ej.521024.cn

TS:   console.error("err")
来源：http://xl.9csxet.cn

Java: System.err.println("err")
来源：http://vu.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hy.haigaiapp.cn

Ruby: warn "err"
来源：http://sq.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://gs.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://dy.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://xv.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xl.nicolike.cn

JS:   require.main === module
来源：http://tf.shxzukj.cn

TS:   require.main === module
来源：http://st.colortex.cn

Java: public static void main(String[] args)
来源：http://wg.lnxyls.cn

Go:   func main()
来源：http://hv.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vv.colortex.cn

C#:   static void Main(string[] args)
来源：http://ox.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://mi.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://op.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://kz.9csxet.cn

JS:   process.platform;  process.version
来源：http://ik.asd995.cn

TS:   process.platform;  process.version
来源：http://ww.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nr.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pf.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qo.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dh.asd995.cn

================================================================================
来源：http://on.nszjky.cn

N. 数据结构与算法
来源：http://kl.shtwfgs.cn

================================================================================
来源：http://ma.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://lv.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eb.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://op.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://an.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ml.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ad.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://gg.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yo.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jh.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://zx.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ck.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gc.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mm.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yz.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ea.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ex.jianghongdianzi.cn

Ruby: arr.sort
来源：http://yp.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yx.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://ak.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://se.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://fc.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xt.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yq.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ax.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vg.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xd.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ec.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://xa.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bh.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hu.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uf.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bw.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fe.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ui.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vf.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mk.wgjwhj.cn

[N05] 最大公约数
来源：http://uq.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://bh.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mx.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sw.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wb.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yu.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dg.521024.cn

Ruby: a.gcd(b)
来源：http://qa.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ps.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://yb.shxzskj.cn

Py:   s == s[::-1]
来源：http://us.9csxet.cn

PHP:  $s === strrev($s);
来源：http://so.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://js.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://cg.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xa.9csxet.cn

Go:   // 双指针从两端比较
来源：http://mm.lnxyls.cn

Ruby: s == s.reverse
来源：http://vt.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ps.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://xq.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gp.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zd.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://em.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://bk.szxytkj.cn

Java: // 手写 HashMap
来源：http://mp.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://mu.9csxet.cn

Ruby: // 手写 Hash
来源：http://bx.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sy.9csxet.cn

[N08] 生成全排列
来源：http://rb.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ha.panjiajie.cn

PHP:  // 手写递归交换
来源：http://qm.gzmigu.cn

JS:   // 手写回溯递归
来源：http://ow.nicolike.cn

TS:   // 手写回溯递归
来源：http://jc.muxihuayi.cn

Java: // 手写回溯递归
来源：http://th.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://wx.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://kf.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://kt.newstarts.cn

[N09] 栈与队列
来源：http://fx.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jb.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mk.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xp.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gk.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uv.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aw.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ha.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sa.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://sg.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tt.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://il.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nm.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iu.asd995.cn

Java: class Node { int v; Node next; }
来源：http://vh.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nh.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tv.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xz.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://pk.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ba.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ez.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lk.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tc.jianghongdianzi.cn

Java: // 手写递归
来源：http://tc.muxihuayi.cn

Go:   // 手写递归
来源：http://xj.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ah.gzmigu.cn

C#:   // 手写递归
来源：http://kb.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://en.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ww.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bs.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tr.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ij.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qm.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fn.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ga.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hf.haigaiapp.cn

================================================================================
来源：http://ln.muxihuayi.cn

O. 并发与异步
来源：http://cu.haigaiapp.cn

================================================================================
来源：http://uy.nicolike.cn

[O01] 启动一个线程
来源：http://qo.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rs.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://du.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ye.chemitech.net.cn

TS:   // 同 JS
来源：http://bi.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://eb.bookmarksfly.cn

Go:   go f()
来源：http://ba.hnjuh.cn

Ruby: Thread.new { f }
来源：http://qa.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://mi.wgjwhj.cn

[O02] 使用线程池
来源：http://qh.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hx.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://le.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://ox.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://gh.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rm.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://la.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jl.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sa.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://ms.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://na.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://yb.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yp.yuntaijiaju.cn

TS:   // 同 JS
来源：http://vm.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://xr.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ld.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qa.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://bd.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://ew.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://il.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kp.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://ui.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hc.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kn.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zr.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://na.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://mm.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://rt.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://yd.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mj.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://sq.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://il.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hn.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yi.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://xe.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qa.shxzukj.cn

[O06] 使用进程池
来源：http://kk.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pq.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tc.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://af.521024.cn

TS:   // child_process / cluster 模块
来源：http://gr.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hx.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jp.gzmigu.cn

Ruby: // fork 块
来源：http://xi.lnxyls.cn

C#:   Parallel.For
来源：http://da.jctech888.com.cn

================================================================================
来源：http://sd.9csxet.cn

P. 常用工具函数
来源：http://eh.jctech888.com.cn

================================================================================
来源：http://dt.szxytkj.cn

[P01] 生成 UUID
来源：http://ov.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://ad.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rx.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ad.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://rg.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://lo.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://jd.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://kc.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://sg.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://ra.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bh.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ck.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kf.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tg.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xl.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://is.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kt.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zd.szxytkj.cn

[P03] 生成短随机字符串
来源：http://xe.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ag.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eb.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lt.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gj.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mg.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hu.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ak.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ph.9csxet.cn

[P04] 求长度
来源：http://ve.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kh.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ut.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bg.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pk.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://lm.nicolike.cn

Go:   len(arr);  len(m)
来源：http://tw.asd995.cn

Ruby: x.length;  x.size
来源：http://tb.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xj.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://xl.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lu.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qy.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pb.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sb.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wv.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oq.asd995.cn

Ruby: a == b
来源：http://nv.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ts.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wc.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pb.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://nh.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cu.jctech888.com.cn

TS:   if (x == null) {}
来源：http://ta.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ck.shxzukj.cn

Go:   if x == nil {}
来源：http://sr.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rl.shtwfgs.cn

C#:   if (x is null) {}
来源：http://bt.shxzukj.cn

[P07] 防抖与节流
来源：http://vm.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://al.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://ct.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zo.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pa.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jy.newstarts.cn


<!-- 参考信息 -->