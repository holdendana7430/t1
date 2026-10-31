代发 wailian999

JS:   process.argv.slice(2)
来源：http://jk.asd995.cn

TS:   process.argv.slice(2)
来源：http://jx.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://nq.colortex.cn

Go:   os.Args[1:]
来源：http://vk.bookmarksfly.cn

Ruby: ARGV
来源：http://pc.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://rk.szsharing.cn

[M02] 读取环境变量
来源：http://rs.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://po.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wq.hahajie.cn

JS:   process.env.HOME
来源：http://hy.colortex.cn

TS:   process.env.HOME
来源：http://mf.newstarts.cn

Java: System.getenv("HOME")
来源：http://it.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://re.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://mv.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mp.asd995.cn

[M03] 执行外部命令
来源：http://lu.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ee.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yd.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iv.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yj.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wm.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gb.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jv.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://tn.szxytkj.cn

[M04] 获取当前工作目录
来源：http://rv.colortex.cn

Py:   os.getcwd()
来源：http://eb.newstarts.cn

PHP:  getcwd();
来源：http://bi.wgjwhj.cn

JS:   process.cwd()
来源：http://on.panjiajie.cn

TS:   process.cwd()
来源：http://mm.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://zs.muxihuayi.cn

Go:   os.Getwd()
来源：http://jv.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://pn.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mm.szsharing.cn

[M05] 设置退出码
来源：http://ng.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ob.szsharing.cn

PHP:  exit(1);
来源：http://yl.colortex.cn

JS:   process.exit(1)
来源：http://pi.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ov.hahajie.cn

Java: System.exit(1)
来源：http://kv.shtwfgs.cn

Go:   os.Exit(1)
来源：http://ib.jianghongdianzi.cn

Ruby: exit 1
来源：http://uw.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ji.asd995.cn

[M06] 向标准错误输出
来源：http://lu.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://sv.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fc.panjiajie.cn

JS:   console.error("err")
来源：http://on.huanxung.cn

TS:   console.error("err")
来源：http://da.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://du.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ck.szsharing.cn

Ruby: warn "err"
来源：http://ss.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://ck.nicolike.cn

[M07] 判断是否为主入口
来源：http://pv.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://nr.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mz.szxytkj.cn

JS:   require.main === module
来源：http://pn.chemitech.net.cn

TS:   require.main === module
来源：http://wg.colortex.cn

Java: public static void main(String[] args)
来源：http://ck.nszjky.cn

Go:   func main()
来源：http://zx.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vb.szsharing.cn

C#:   static void Main(string[] args)
来源：http://tl.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://py.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://jc.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.asd995.cn

JS:   process.platform;  process.version
来源：http://xa.521024.cn

TS:   process.platform;  process.version
来源：http://mi.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ia.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lm.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ek.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mb.gzmigu.cn

================================================================================
来源：http://ob.yuexingan06.cn

N. 数据结构与算法
来源：http://kw.szxytkj.cn

================================================================================
来源：http://mk.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://vw.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ss.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nv.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oi.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zd.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pp.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://wh.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nj.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jr.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://lj.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ux.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tg.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ab.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fu.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://zy.yuntaijiaju.cn

Ruby: arr.sort
来源：http://hs.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vp.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://xv.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pe.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://jv.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lm.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hw.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rc.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qk.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ps.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wu.panjiajie.cn

[N04] 斐波那契数列
来源：http://rb.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sr.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://do.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hm.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ft.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ls.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mv.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jj.yuexingan06.cn

[N05] 最大公约数
来源：http://va.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ny.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mh.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wu.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ps.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vy.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yp.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://dv.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gz.muxihuayi.cn

[N06] 判断回文字符串
来源：http://og.szxytkj.cn

Py:   s == s[::-1]
来源：http://um.hahajie.cn

PHP:  $s === strrev($s);
来源：http://wj.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://kf.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://eo.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zy.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ld.yuexingan06.cn

Ruby: s == s.reverse
来源：http://bn.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pw.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://lp.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mv.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aj.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bv.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://kx.newstarts.cn

Java: // 手写 HashMap
来源：http://vr.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://gm.shxzskj.cn

Ruby: // 手写 Hash
来源：http://hp.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jx.shtwfgs.cn

[N08] 生成全排列
来源：http://sf.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://qh.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://sq.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://wf.huanxung.cn

TS:   // 手写回溯递归
来源：http://rm.panjiajie.cn

Java: // 手写回溯递归
来源：http://vf.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://it.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://yu.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://ki.colortex.cn

[N09] 栈与队列
来源：http://ly.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gc.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tf.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yk.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wb.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ut.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nd.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uf.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nb.asd995.cn

[N10] 链表节点定义
来源：http://lx.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://le.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rk.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://in.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ag.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://sv.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nu.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pd.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ua.colortex.cn

[N11] 二叉树中序遍历
来源：http://qe.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yl.shxzskj.cn

PHP:  // 手写递归函数
来源：http://bw.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ez.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qf.yuexingan06.cn

Java: // 手写递归
来源：http://qi.shtwfgs.cn

Go:   // 手写递归
来源：http://kl.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ad.huanxung.cn

C#:   // 手写递归
来源：http://fi.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bk.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ry.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://af.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jj.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qj.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rz.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nk.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uu.nszjky.cn

================================================================================
来源：http://bi.szsharing.cn

O. 并发与异步
来源：http://dp.nszjky.cn

================================================================================
来源：http://eh.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://nq.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ur.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nf.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://if.chemitech.net.cn

TS:   // 同 JS
来源：http://gb.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://dx.huixiangedu.cn

Go:   go f()
来源：http://rq.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://xl.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ef.shxzskj.cn

[O02] 使用线程池
来源：http://ql.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rz.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rk.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://if.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://mo.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bw.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ya.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gj.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hu.szsharing.cn

[O03] 加锁保护共享数据
来源：http://vn.newstarts.cn

Py:   with lock: shared += 1
来源：http://ha.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://iy.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://je.shxzukj.cn

TS:   // 同 JS
来源：http://vh.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ty.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tp.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pb.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://uj.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://cu.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ih.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://si.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://jb.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vq.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dj.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ue.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ha.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://gy.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://ab.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://ly.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://is.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://aw.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://fn.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zw.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vo.szsharing.cn

Ruby: threads.map(&:join)
来源：http://gt.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xe.yuntaijiaju.cn

[O06] 使用进程池
来源：http://mx.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lm.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yo.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://uc.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://pi.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vi.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ft.jianghongdianzi.cn

Ruby: // fork 块
来源：http://pi.jctech888.com.cn

C#:   Parallel.For
来源：http://pd.yuntaijiaju.cn

================================================================================
来源：http://ld.bookmarksfly.cn

P. 常用工具函数
来源：http://zh.haigaiapp.cn

================================================================================
来源：http://eb.shxzskj.cn

[P01] 生成 UUID
来源：http://we.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://gp.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ay.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ng.9csxet.cn

TS:   crypto.randomUUID()
来源：http://aq.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://mk.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://dp.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://kv.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://cl.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://so.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tb.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kk.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://og.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ml.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cq.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ie.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zj.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://al.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://lt.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lt.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jv.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pi.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ho.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ih.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dt.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yn.muxihuayi.cn

[P04] 求长度
来源：http://mk.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sd.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yc.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uc.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xd.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://qm.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://jk.nszjky.cn

Ruby: x.length;  x.size
来源：http://jk.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iu.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://ct.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mu.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kj.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sx.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hx.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hv.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xl.huixiangedu.cn

Ruby: a == b
来源：http://jo.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cv.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fx.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://af.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://au.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zp.nszjky.cn

TS:   if (x == null) {}
来源：http://qr.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xq.hnjuh.cn

Go:   if x == nil {}
来源：http://wy.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mv.shxzukj.cn

C#:   if (x is null) {}
来源：http://kt.bookmarksfly.cn

[P07] 防抖与节流
来源：http://rd.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uj.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://do.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nn.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dw.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iy.lnxyls.cn


<!-- 参考信息 -->