代发 wailian999

JS:   process.argv.slice(2)
来源：http://xg.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://mh.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://vq.muxihuayi.cn

Go:   os.Args[1:]
来源：http://td.9csxet.cn

Ruby: ARGV
来源：http://yb.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://nk.shxzukj.cn

[M02] 读取环境变量
来源：http://yd.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://wp.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gk.szsharing.cn

JS:   process.env.HOME
来源：http://mv.9csxet.cn

TS:   process.env.HOME
来源：http://fs.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://im.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tk.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ad.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fb.521024.cn

[M03] 执行外部命令
来源：http://uj.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://he.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lc.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zf.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://au.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cq.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://we.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cb.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://cb.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://ef.shtwfgs.cn

Py:   os.getcwd()
来源：http://hu.panjiajie.cn

PHP:  getcwd();
来源：http://zd.huixinmuqiang.cn

JS:   process.cwd()
来源：http://ft.huixiangedu.cn

TS:   process.cwd()
来源：http://pi.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://vd.nicolike.cn

Go:   os.Getwd()
来源：http://er.shxzukj.cn

Ruby: Dir.pwd
来源：http://on.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://on.szxytkj.cn

[M05] 设置退出码
来源：http://kn.huanxung.cn

Py:   sys.exit(1)
来源：http://kx.lnxyls.cn

PHP:  exit(1);
来源：http://xn.shxzukj.cn

JS:   process.exit(1)
来源：http://xn.muxihuayi.cn

TS:   process.exit(1)
来源：http://bf.9csxet.cn

Java: System.exit(1)
来源：http://fe.panjiajie.cn

Go:   os.Exit(1)
来源：http://fp.muxihuayi.cn

Ruby: exit 1
来源：http://ap.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kt.huanxung.cn

[M06] 向标准错误输出
来源：http://wz.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ga.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gu.szsharing.cn

JS:   console.error("err")
来源：http://lr.szxytkj.cn

TS:   console.error("err")
来源：http://jl.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://cd.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ex.jctech888.com.cn

Ruby: warn "err"
来源：http://nu.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ht.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://jp.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://di.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sb.jctech888.com.cn

JS:   require.main === module
来源：http://wb.haigaiapp.cn

TS:   require.main === module
来源：http://tg.huanxung.cn

Java: public static void main(String[] args)
来源：http://kw.jctech888.com.cn

Go:   func main()
来源：http://rn.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ej.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://mk.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://hf.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://rk.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://vn.colortex.cn

JS:   process.platform;  process.version
来源：http://zh.nszjky.cn

TS:   process.platform;  process.version
来源：http://nv.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uq.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gt.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dg.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ng.hahajie.cn

================================================================================
来源：http://vw.wgjwhj.cn

N. 数据结构与算法
来源：http://ag.hahajie.cn

================================================================================
来源：http://hd.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://kk.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sy.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://np.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yj.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qj.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://io.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ef.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fc.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://oj.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://di.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lr.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bz.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hy.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jp.hahajie.cn

Go:   slices.Sort(arr)
来源：http://bs.shtwfgs.cn

Ruby: arr.sort
来源：http://ay.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lm.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://xs.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nj.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://hq.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rk.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ty.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jh.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hq.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fl.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sd.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://me.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://do.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ou.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ln.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zu.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tr.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dc.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bg.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fl.jctech888.com.cn

[N05] 最大公约数
来源：http://vq.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://wm.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dz.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://et.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://id.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hu.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ji.newstarts.cn

Ruby: a.gcd(b)
来源：http://tr.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xm.chemitech.net.cn

[N06] 判断回文字符串
来源：http://lt.huixiangedu.cn

Py:   s == s[::-1]
来源：http://gp.nszjky.cn

PHP:  $s === strrev($s);
来源：http://jj.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://sk.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://dj.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wi.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://ax.chemitech.net.cn

Ruby: s == s.reverse
来源：http://lj.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pj.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://kx.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ef.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wx.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://fq.yuexingan06.cn

Java: // 手写 HashMap
来源：http://mc.colortex.cn

Go:   // 手写 map[int]int
来源：http://ag.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://gi.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vq.lnxyls.cn

[N08] 生成全排列
来源：http://pq.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://rn.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://gc.newstarts.cn

JS:   // 手写回溯递归
来源：http://hk.hahajie.cn

TS:   // 手写回溯递归
来源：http://iw.wgjwhj.cn

Java: // 手写回溯递归
来源：http://kt.shxzukj.cn

Go:   // 手写回溯递归
来源：http://nr.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://xz.asd995.cn

C#:   // 手写回溯递归
来源：http://pt.bjjhwx.cn

[N09] 栈与队列
来源：http://lz.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ev.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ox.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vh.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hb.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qe.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qk.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zg.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://en.chemitech.net.cn

[N10] 链表节点定义
来源：http://jn.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://be.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cg.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ye.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hp.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://zc.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ak.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cq.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jd.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://pr.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ly.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://xb.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sn.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ri.shxzskj.cn

Java: // 手写递归
来源：http://ge.521024.cn

Go:   // 手写递归
来源：http://oe.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zw.gzmigu.cn

C#:   // 手写递归
来源：http://iz.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://so.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nq.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://on.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pt.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fq.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://az.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yx.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oh.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kr.nszjky.cn

================================================================================
来源：http://ql.yuexingan06.cn

O. 并发与异步
来源：http://io.asd995.cn

================================================================================
来源：http://cv.yuexingan06.cn

[O01] 启动一个线程
来源：http://ht.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://va.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eh.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yd.shtwfgs.cn

TS:   // 同 JS
来源：http://lc.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://td.lnxyls.cn

Go:   go f()
来源：http://yz.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://kx.asd995.cn

C#:   Task.Run(() => F());
来源：http://fz.haigaiapp.cn

[O02] 使用线程池
来源：http://ip.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cc.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gu.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://qt.szsharing.cn

TS:   // worker_threads 线程池
来源：http://yv.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://up.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gq.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jx.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gr.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://fh.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://yw.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://pw.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ly.muxihuayi.cn

TS:   // 同 JS
来源：http://bc.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://ys.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dh.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mg.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://kp.9csxet.cn

[O04] 定义异步函数并等待
来源：http://yi.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://by.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gl.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://mi.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wa.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mj.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mi.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zn.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://qy.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://yy.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://kh.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yx.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://os.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://qu.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oa.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wa.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://pg.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uc.bjjhwx.cn

[O06] 使用进程池
来源：http://qd.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://od.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sf.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://pr.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://qv.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gv.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vi.newstarts.cn

Ruby: // fork 块
来源：http://ka.jianghongdianzi.cn

C#:   Parallel.For
来源：http://ud.asd995.cn

================================================================================
来源：http://vh.huixinmuqiang.cn

P. 常用工具函数
来源：http://sw.bjjhwx.cn

================================================================================
来源：http://jp.szsharing.cn

[P01] 生成 UUID
来源：http://qn.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://wi.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uk.szsharing.cn

JS:   crypto.randomUUID()
来源：http://br.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://sw.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://im.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://zn.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://ta.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://bd.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://oj.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lv.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xr.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ik.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xl.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gk.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wv.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gb.nicolike.cn

[P03] 生成短随机字符串
来源：http://zi.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zo.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qs.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wx.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cf.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ql.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oa.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iu.hahajie.cn

[P04] 求长度
来源：http://zl.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wy.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ld.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wx.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://xp.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://tc.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://bg.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uy.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://ry.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wy.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://de.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fy.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://om.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sw.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://or.haigaiapp.cn

Ruby: a == b
来源：http://yd.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jw.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jh.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kc.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://tt.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xw.yuexingan06.cn

TS:   if (x == null) {}
来源：http://ae.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cz.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://kv.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eq.9csxet.cn

C#:   if (x is null) {}
来源：http://os.hahajie.cn

[P07] 防抖与节流
来源：http://qg.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://na.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://rz.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ux.muxihuayi.cn


<!-- 参考信息 -->