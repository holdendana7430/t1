代发 wailian999

JS:   process.argv.slice(2)
来源：http://nh.521024.cn

TS:   process.argv.slice(2)
来源：http://mm.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://ey.colortex.cn

Go:   os.Args[1:]
来源：http://mx.szxytkj.cn

Ruby: ARGV
来源：http://ju.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://qs.huixiangedu.cn

[M02] 读取环境变量
来源：http://hi.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://bb.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lk.newstarts.cn

JS:   process.env.HOME
来源：http://gd.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://mr.panjiajie.cn

Java: System.getenv("HOME")
来源：http://bk.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zn.521024.cn

Ruby: ENV["HOME"]
来源：http://lf.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cz.nicolike.cn

[M03] 执行外部命令
来源：http://bx.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lc.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://my.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yj.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mh.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zd.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fz.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uy.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://op.colortex.cn

[M04] 获取当前工作目录
来源：http://pb.lnxyls.cn

Py:   os.getcwd()
来源：http://hh.bjjhwx.cn

PHP:  getcwd();
来源：http://oa.newstarts.cn

JS:   process.cwd()
来源：http://rz.szxytkj.cn

TS:   process.cwd()
来源：http://aa.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://yv.hnjuh.cn

Go:   os.Getwd()
来源：http://zj.szsharing.cn

Ruby: Dir.pwd
来源：http://vd.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rx.szsharing.cn

[M05] 设置退出码
来源：http://el.gzmigu.cn

Py:   sys.exit(1)
来源：http://wg.lnxyls.cn

PHP:  exit(1);
来源：http://gh.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://ap.wgjwhj.cn

TS:   process.exit(1)
来源：http://qz.bookmarksfly.cn

Java: System.exit(1)
来源：http://iy.huanxung.cn

Go:   os.Exit(1)
来源：http://ex.huixinmuqiang.cn

Ruby: exit 1
来源：http://uh.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pj.huanxung.cn

[M06] 向标准错误输出
来源：http://bv.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://zz.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hg.gzmigu.cn

JS:   console.error("err")
来源：http://kf.shxzukj.cn

TS:   console.error("err")
来源：http://ec.wgjwhj.cn

Java: System.err.println("err")
来源：http://on.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mi.jianghongdianzi.cn

Ruby: warn "err"
来源：http://xz.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://od.szsharing.cn

[M07] 判断是否为主入口
来源：http://ii.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://fg.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://md.yuexingan06.cn

JS:   require.main === module
来源：http://js.hnjuh.cn

TS:   require.main === module
来源：http://al.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://ui.jianghongdianzi.cn

Go:   func main()
来源：http://gt.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ye.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://hf.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://fy.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://am.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://xp.newstarts.cn

JS:   process.platform;  process.version
来源：http://fx.shxzskj.cn

TS:   process.platform;  process.version
来源：http://xf.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oc.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kn.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jo.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gu.newstarts.cn

================================================================================
来源：http://gn.newstarts.cn

N. 数据结构与算法
来源：http://ou.szsharing.cn

================================================================================
来源：http://nq.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://pc.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rr.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kd.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qt.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uy.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nt.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://pj.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ea.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yw.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://vr.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ie.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ig.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eh.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pq.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cw.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://eu.colortex.cn

Ruby: arr.sort
来源：http://bh.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zi.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://qe.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gg.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://hv.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mv.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lf.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rn.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uy.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://me.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://re.panjiajie.cn

[N04] 斐波那契数列
来源：http://yo.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ud.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dh.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rr.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://py.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lq.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ma.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ba.huanxung.cn

[N05] 最大公约数
来源：http://in.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://mz.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://df.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dz.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rx.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://la.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pa.hahajie.cn

Ruby: a.gcd(b)
来源：http://jj.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tz.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://zg.haigaiapp.cn

Py:   s == s[::-1]
来源：http://it.szsharing.cn

PHP:  $s === strrev($s);
来源：http://hm.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://yr.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://vr.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xk.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://je.lnxyls.cn

Ruby: s == s.reverse
来源：http://la.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ax.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://sk.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ni.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xb.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qw.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://jn.shxzskj.cn

Java: // 手写 HashMap
来源：http://xw.nszjky.cn

Go:   // 手写 map[int]int
来源：http://gs.shxzskj.cn

Ruby: // 手写 Hash
来源：http://lg.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fq.panjiajie.cn

[N08] 生成全排列
来源：http://im.asd995.cn

Py:   itertools.permutations(arr)
来源：http://hd.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://dm.lnxyls.cn

JS:   // 手写回溯递归
来源：http://ur.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://qm.huanxung.cn

Java: // 手写回溯递归
来源：http://bw.nicolike.cn

Go:   // 手写回溯递归
来源：http://vo.521024.cn

Ruby: arr.permutation.to_a
来源：http://eq.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://ds.shxzskj.cn

[N09] 栈与队列
来源：http://fn.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hy.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ph.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rd.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://na.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jc.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cb.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fv.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://te.shtwfgs.cn

[N10] 链表节点定义
来源：http://vw.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vv.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ac.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yf.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qz.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://gm.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bx.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lz.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lz.nicolike.cn

[N11] 二叉树中序遍历
来源：http://wk.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mw.9csxet.cn

PHP:  // 手写递归函数
来源：http://vs.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jd.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qx.jctech888.com.cn

Java: // 手写递归
来源：http://by.nicolike.cn

Go:   // 手写递归
来源：http://mg.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kj.hahajie.cn

C#:   // 手写递归
来源：http://ln.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://to.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eh.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mo.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ym.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yd.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pk.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uk.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tz.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wr.newstarts.cn

================================================================================
来源：http://xl.hnjuh.cn

O. 并发与异步
来源：http://cb.yuntaijiaju.cn

================================================================================
来源：http://qh.shxzskj.cn

[O01] 启动一个线程
来源：http://on.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wz.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hs.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lw.wgjwhj.cn

TS:   // 同 JS
来源：http://wo.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://ys.shtwfgs.cn

Go:   go f()
来源：http://cy.lnxyls.cn

Ruby: Thread.new { f }
来源：http://gk.521024.cn

C#:   Task.Run(() => F());
来源：http://cw.panjiajie.cn

[O02] 使用线程池
来源：http://xt.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qm.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://il.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://jt.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://kb.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pi.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nn.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wx.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://no.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://gu.huanxung.cn

Py:   with lock: shared += 1
来源：http://zt.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://qc.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://na.chemitech.net.cn

TS:   // 同 JS
来源：http://ni.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://bo.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://io.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://is.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://we.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://fs.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://cd.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sl.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://sz.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qd.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sr.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gj.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lu.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://za.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://xw.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://yv.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hi.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://ih.colortex.cn

TS:   await Promise.all(tasks)
来源：http://jf.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iw.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fk.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ma.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ct.hahajie.cn

[O06] 使用进程池
来源：http://xj.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bh.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hy.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://bx.colortex.cn

TS:   // child_process / cluster 模块
来源：http://gs.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mp.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ti.hahajie.cn

Ruby: // fork 块
来源：http://xv.asd995.cn

C#:   Parallel.For
来源：http://rd.bjjhwx.cn

================================================================================
来源：http://ti.shxzukj.cn

P. 常用工具函数
来源：http://bn.szxytkj.cn

================================================================================
来源：http://yk.lnxyls.cn

[P01] 生成 UUID
来源：http://do.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://pl.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vy.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://xb.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://dl.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://zx.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://te.colortex.cn

Ruby: SecureRandom.uuid
来源：http://dr.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://um.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://ub.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nl.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hj.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ta.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oc.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pb.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mb.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://co.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ny.9csxet.cn

[P03] 生成短随机字符串
来源：http://ku.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gf.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ve.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rb.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wi.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hf.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yb.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xl.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vn.yuntaijiaju.cn

[P04] 求长度
来源：http://aj.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://af.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pz.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://np.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://qi.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://va.huanxung.cn

Ruby: x.length;  x.size
来源：http://ax.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gw.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://dk.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sg.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bt.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://py.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ne.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bl.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wn.huanxung.cn

Ruby: a == b
来源：http://ia.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qa.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rf.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vh.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://ii.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bk.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://wa.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sv.shxzskj.cn

Go:   if x == nil {}
来源：http://op.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gy.panjiajie.cn

C#:   if (x is null) {}
来源：http://tw.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://tj.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vm.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://ad.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ej.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jn.yuntaijiaju.cn


<!-- 参考信息 -->