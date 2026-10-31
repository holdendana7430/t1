代发 wailian999

JS:   process.argv.slice(2)
来源：http://gr.nicolike.cn

TS:   process.argv.slice(2)
来源：http://ju.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://wb.hahajie.cn

Go:   os.Args[1:]
来源：http://qb.muxihuayi.cn

Ruby: ARGV
来源：http://kg.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://zn.szsharing.cn

[M02] 读取环境变量
来源：http://lw.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://kn.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://td.nicolike.cn

JS:   process.env.HOME
来源：http://sk.panjiajie.cn

TS:   process.env.HOME
来源：http://sj.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ok.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vy.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://ku.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ms.yuexingan06.cn

[M03] 执行外部命令
来源：http://it.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mp.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://az.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lv.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ps.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tj.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://he.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ny.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://ta.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://um.nszjky.cn

Py:   os.getcwd()
来源：http://et.521024.cn

PHP:  getcwd();
来源：http://ds.szsharing.cn

JS:   process.cwd()
来源：http://pq.hnjuh.cn

TS:   process.cwd()
来源：http://jh.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://bj.panjiajie.cn

Go:   os.Getwd()
来源：http://vb.szxytkj.cn

Ruby: Dir.pwd
来源：http://kw.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nl.shxzskj.cn

[M05] 设置退出码
来源：http://uc.nszjky.cn

Py:   sys.exit(1)
来源：http://zb.nicolike.cn

PHP:  exit(1);
来源：http://ya.yuexingan06.cn

JS:   process.exit(1)
来源：http://qx.panjiajie.cn

TS:   process.exit(1)
来源：http://uq.bookmarksfly.cn

Java: System.exit(1)
来源：http://xz.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://vv.hnjuh.cn

Ruby: exit 1
来源：http://fk.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hu.szxytkj.cn

[M06] 向标准错误输出
来源：http://ka.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://og.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://su.haigaiapp.cn

JS:   console.error("err")
来源：http://mr.wgjwhj.cn

TS:   console.error("err")
来源：http://ku.huixiangedu.cn

Java: System.err.println("err")
来源：http://mt.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lr.lnxyls.cn

Ruby: warn "err"
来源：http://al.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://xp.shxzukj.cn

[M07] 判断是否为主入口
来源：http://fb.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://dx.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oq.jianghongdianzi.cn

JS:   require.main === module
来源：http://ab.jianghongdianzi.cn

TS:   require.main === module
来源：http://es.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://oe.haigaiapp.cn

Go:   func main()
来源：http://nt.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tf.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://xv.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://cc.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://mq.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://fa.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://bh.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://ih.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ov.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vu.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nv.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rg.lnxyls.cn

================================================================================
来源：http://wp.wgjwhj.cn

N. 数据结构与算法
来源：http://ql.szsharing.cn

================================================================================
来源：http://hf.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://xv.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vo.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jm.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://re.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vo.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://pt.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ig.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mx.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://pj.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://vu.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sl.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rn.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ty.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nb.521024.cn

Go:   slices.Sort(arr)
来源：http://xd.colortex.cn

Ruby: arr.sort
来源：http://fx.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ky.521024.cn

[N03] 快速排序（分治示例）
来源：http://yd.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mf.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://rj.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://us.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ay.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cs.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://js.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fo.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aj.lnxyls.cn

[N04] 斐波那契数列
来源：http://om.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nb.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://au.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nb.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://np.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bm.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gx.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qt.huanxung.cn

[N05] 最大公约数
来源：http://tz.newstarts.cn

Py:   math.gcd(a, b)
来源：http://rs.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lg.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qc.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aa.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yi.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ho.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://bo.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bu.shxzukj.cn

[N06] 判断回文字符串
来源：http://ur.huanxung.cn

Py:   s == s[::-1]
来源：http://pn.521024.cn

PHP:  $s === strrev($s);
来源：http://dv.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://dk.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://kd.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wl.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://cl.shxzukj.cn

Ruby: s == s.reverse
来源：http://oq.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fu.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://gf.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vb.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yo.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ky.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://we.shxzukj.cn

Java: // 手写 HashMap
来源：http://rd.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://lg.newstarts.cn

Ruby: // 手写 Hash
来源：http://kl.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ky.szxytkj.cn

[N08] 生成全排列
来源：http://ui.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://mt.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://du.szsharing.cn

JS:   // 手写回溯递归
来源：http://gg.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ah.nszjky.cn

Java: // 手写回溯递归
来源：http://rn.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://rb.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://vy.gzmigu.cn

C#:   // 手写回溯递归
来源：http://uv.muxihuayi.cn

[N09] 栈与队列
来源：http://xx.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bh.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wx.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://db.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ld.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sj.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dc.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://py.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dk.panjiajie.cn

[N10] 链表节点定义
来源：http://ny.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lb.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ka.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://th.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pj.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ei.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yp.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xn.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ze.asd995.cn

[N11] 二叉树中序遍历
来源：http://xd.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nt.newstarts.cn

PHP:  // 手写递归函数
来源：http://dh.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wt.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://su.huixinmuqiang.cn

Java: // 手写递归
来源：http://ci.wgjwhj.cn

Go:   // 手写递归
来源：http://hy.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rm.shtwfgs.cn

C#:   // 手写递归
来源：http://bz.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kp.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gf.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pd.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hx.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dn.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ji.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nd.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ei.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://an.521024.cn

================================================================================
来源：http://vn.huixiangedu.cn

O. 并发与异步
来源：http://ek.haigaiapp.cn

================================================================================
来源：http://bd.wgjwhj.cn

[O01] 启动一个线程
来源：http://cm.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nw.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://np.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yw.shxzukj.cn

TS:   // 同 JS
来源：http://vc.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://me.hahajie.cn

Go:   go f()
来源：http://nx.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://co.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://qb.521024.cn

[O02] 使用线程池
来源：http://eo.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iy.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pd.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://mp.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://cf.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jj.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kg.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://va.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ey.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://bg.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://aa.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://zt.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tz.nszjky.cn

TS:   // 同 JS
来源：http://gv.521024.cn

Java: synchronized (this) { shared++; }
来源：http://rs.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hk.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vb.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://bk.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://sv.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://oa.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pt.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://vj.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nt.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xw.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nm.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xj.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://cl.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://zr.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://wc.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tl.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://xy.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://cx.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kg.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sw.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://xk.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjjhwx.cn

[O06] 使用进程池
来源：http://va.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xi.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bg.colortex.cn

JS:   // child_process / cluster 模块
来源：http://gr.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://uu.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sh.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xg.asd995.cn

Ruby: // fork 块
来源：http://qg.colortex.cn

C#:   Parallel.For
来源：http://vo.szxytkj.cn

================================================================================
来源：http://wv.521024.cn

P. 常用工具函数
来源：http://hv.hahajie.cn

================================================================================
来源：http://em.bjjhwx.cn

[P01] 生成 UUID
来源：http://gq.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://lr.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pn.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://zc.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://qk.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://dg.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://oz.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://dw.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bb.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://nx.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nj.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zy.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ok.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hs.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rx.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dm.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ej.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zf.nicolike.cn

[P03] 生成短随机字符串
来源：http://jr.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yo.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sp.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lp.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ol.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uh.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uc.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jp.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gl.jctech888.com.cn

[P04] 求长度
来源：http://ny.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://up.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nk.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ye.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mv.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://br.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://rx.szsharing.cn

Ruby: x.length;  x.size
来源：http://kx.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bo.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://lh.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yc.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vf.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lf.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sx.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://en.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iy.jctech888.com.cn

Ruby: a == b
来源：http://my.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tb.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kx.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://br.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://fa.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jy.shxzskj.cn

TS:   if (x == null) {}
来源：http://hv.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xv.shtwfgs.cn

Go:   if x == nil {}
来源：http://lc.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rs.lnxyls.cn

C#:   if (x is null) {}
来源：http://xh.shtwfgs.cn

[P07] 防抖与节流
来源：http://yz.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wr.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://zc.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xq.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zx.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ag.asd995.cn


<!-- 参考信息 -->