代发 wailian999

JS:   process.argv.slice(2)
来源：http://xo.szsharing.cn

TS:   process.argv.slice(2)
来源：http://pf.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://dv.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://jb.shtwfgs.cn

Ruby: ARGV
来源：http://gt.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ud.hahajie.cn

[M02] 读取环境变量
来源：http://ox.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://wk.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zx.chemitech.net.cn

JS:   process.env.HOME
来源：http://nr.szxytkj.cn

TS:   process.env.HOME
来源：http://by.9csxet.cn

Java: System.getenv("HOME")
来源：http://fu.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ls.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://cw.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pz.huanxung.cn

[M03] 执行外部命令
来源：http://dp.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qo.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qy.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mw.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xa.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mz.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ux.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sp.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://wq.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://qg.bookmarksfly.cn

Py:   os.getcwd()
来源：http://dx.muxihuayi.cn

PHP:  getcwd();
来源：http://fg.szxytkj.cn

JS:   process.cwd()
来源：http://kx.chemitech.net.cn

TS:   process.cwd()
来源：http://fw.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://qu.shtwfgs.cn

Go:   os.Getwd()
来源：http://qo.huixiangedu.cn

Ruby: Dir.pwd
来源：http://ba.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yp.huixinmuqiang.cn

[M05] 设置退出码
来源：http://oc.szxytkj.cn

Py:   sys.exit(1)
来源：http://it.shxzskj.cn

PHP:  exit(1);
来源：http://mm.newstarts.cn

JS:   process.exit(1)
来源：http://vz.bjjhwx.cn

TS:   process.exit(1)
来源：http://aq.gzmigu.cn

Java: System.exit(1)
来源：http://bq.newstarts.cn

Go:   os.Exit(1)
来源：http://iz.asd995.cn

Ruby: exit 1
来源：http://mm.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yb.colortex.cn

[M06] 向标准错误输出
来源：http://sr.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://hg.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://im.yuntaijiaju.cn

JS:   console.error("err")
来源：http://rb.shtwfgs.cn

TS:   console.error("err")
来源：http://aj.9csxet.cn

Java: System.err.println("err")
来源：http://hb.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sz.newstarts.cn

Ruby: warn "err"
来源：http://fz.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ei.nicolike.cn

[M07] 判断是否为主入口
来源：http://vv.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://xy.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oo.hnjuh.cn

JS:   require.main === module
来源：http://cd.huixiangedu.cn

TS:   require.main === module
来源：http://hc.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ws.chemitech.net.cn

Go:   func main()
来源：http://jn.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ff.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://fl.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://eq.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://vk.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://ao.szsharing.cn

JS:   process.platform;  process.version
来源：http://gw.shxzskj.cn

TS:   process.platform;  process.version
来源：http://hh.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qq.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lt.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sb.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vv.shxzukj.cn

================================================================================
来源：http://oq.newstarts.cn

N. 数据结构与算法
来源：http://tp.szxytkj.cn

================================================================================
来源：http://bc.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://kk.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sb.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ry.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bc.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zv.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ed.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://su.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qh.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lj.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://ie.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://gy.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ir.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ch.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uu.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yb.9csxet.cn

Go:   slices.Sort(arr)
来源：http://fo.gzmigu.cn

Ruby: arr.sort
来源：http://ha.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iy.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://vl.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rm.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://kz.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zx.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rs.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ck.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lu.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tl.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wh.asd995.cn

[N04] 斐波那契数列
来源：http://ut.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wt.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pa.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wi.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ok.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wb.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rb.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iq.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://te.muxihuayi.cn

[N05] 最大公约数
来源：http://pf.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://qa.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ig.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gi.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kd.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sy.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://br.nszjky.cn

Ruby: a.gcd(b)
来源：http://ab.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gh.shxzukj.cn

[N06] 判断回文字符串
来源：http://zn.colortex.cn

Py:   s == s[::-1]
来源：http://xd.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://bz.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://bh.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://bz.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://an.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://jd.nszjky.cn

Ruby: s == s.reverse
来源：http://gm.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nj.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://to.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ga.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wa.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pr.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://jd.9csxet.cn

Java: // 手写 HashMap
来源：http://gf.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://vq.asd995.cn

Ruby: // 手写 Hash
来源：http://nu.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ds.jianghongdianzi.cn

[N08] 生成全排列
来源：http://hd.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://aa.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://bd.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://qm.hahajie.cn

TS:   // 手写回溯递归
来源：http://kx.asd995.cn

Java: // 手写回溯递归
来源：http://eb.hahajie.cn

Go:   // 手写回溯递归
来源：http://sq.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://jc.szsharing.cn

C#:   // 手写回溯递归
来源：http://dy.muxihuayi.cn

[N09] 栈与队列
来源：http://od.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rs.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qq.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xy.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xn.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hu.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://te.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tn.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tv.colortex.cn

[N10] 链表节点定义
来源：http://bf.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://su.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kk.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dr.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bc.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://px.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cd.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ke.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zy.huanxung.cn

[N11] 二叉树中序遍历
来源：http://qx.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rw.9csxet.cn

PHP:  // 手写递归函数
来源：http://yf.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oj.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zy.521024.cn

Java: // 手写递归
来源：http://wj.521024.cn

Go:   // 手写递归
来源：http://jh.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pu.szsharing.cn

C#:   // 手写递归
来源：http://gh.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nk.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pl.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ek.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tg.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jf.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yd.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mq.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qt.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pw.huanxung.cn

================================================================================
来源：http://bc.gzmigu.cn

O. 并发与异步
来源：http://al.shtwfgs.cn

================================================================================
来源：http://oz.9csxet.cn

[O01] 启动一个线程
来源：http://vs.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ux.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cz.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ko.shxzukj.cn

TS:   // 同 JS
来源：http://ok.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://qp.bjjhwx.cn

Go:   go f()
来源：http://gk.shxzukj.cn

Ruby: Thread.new { f }
来源：http://kz.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://rg.bookmarksfly.cn

[O02] 使用线程池
来源：http://zo.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oe.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kl.521024.cn

JS:   // worker_threads 线程池
来源：http://dv.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://fm.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lo.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fo.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xa.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sy.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://eg.newstarts.cn

Py:   with lock: shared += 1
来源：http://dh.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ev.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zu.szxytkj.cn

TS:   // 同 JS
来源：http://ke.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://ts.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uy.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gy.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://iu.szsharing.cn

[O04] 定义异步函数并等待
来源：http://mn.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://gb.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lx.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://oo.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oi.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rp.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ou.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cj.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://fr.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://ya.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://rp.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mi.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://sw.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://rh.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kc.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ku.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://vs.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hx.jianghongdianzi.cn

[O06] 使用进程池
来源：http://ck.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iu.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://di.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://no.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://np.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ad.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tl.asd995.cn

Ruby: // fork 块
来源：http://lb.yuexingan06.cn

C#:   Parallel.For
来源：http://gd.shxzskj.cn

================================================================================
来源：http://ff.hahajie.cn

P. 常用工具函数
来源：http://gi.jctech888.com.cn

================================================================================
来源：http://cj.nicolike.cn

[P01] 生成 UUID
来源：http://gf.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://hh.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lv.521024.cn

JS:   crypto.randomUUID()
来源：http://rh.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://ic.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://hd.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://mw.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://vy.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://dh.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ep.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xf.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xn.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tw.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bw.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uy.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vd.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ti.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xp.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://pz.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bm.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ha.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eu.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xt.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jb.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nf.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pp.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ow.jctech888.com.cn

[P04] 求长度
来源：http://mz.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rg.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ly.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ae.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://il.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://yx.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://rq.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://wi.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rg.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://nh.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ww.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fh.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mm.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wp.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cr.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hw.hahajie.cn

Ruby: a == b
来源：http://tk.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tn.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tf.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://us.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://xu.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bv.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://rl.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rz.shtwfgs.cn

Go:   if x == nil {}
来源：http://hh.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sn.hnjuh.cn

C#:   if (x is null) {}
来源：http://qp.szxytkj.cn

[P07] 防抖与节流
来源：http://cb.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lx.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://cj.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xh.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://up.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vz.lnxyls.cn


<!-- 参考信息 -->