代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tg.huixiangedu.cn

JS:   process.env.HOME
来源：http://hu.asd995.cn

TS:   process.env.HOME
来源：http://ky.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://uc.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ih.szsharing.cn

Ruby: ENV["HOME"]
来源：http://pk.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fn.bjjhwx.cn

[M03] 执行外部命令
来源：http://ga.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://en.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gt.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hx.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lx.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bd.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mw.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yc.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://jw.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://fu.jctech888.com.cn

Py:   os.getcwd()
来源：http://zg.asd995.cn

PHP:  getcwd();
来源：http://zx.yuexingan06.cn

JS:   process.cwd()
来源：http://ma.haigaiapp.cn

TS:   process.cwd()
来源：http://tl.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://ap.haigaiapp.cn

Go:   os.Getwd()
来源：http://gq.nicolike.cn

Ruby: Dir.pwd
来源：http://zd.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lq.bjjhwx.cn

[M05] 设置退出码
来源：http://up.shxzukj.cn

Py:   sys.exit(1)
来源：http://er.nicolike.cn

PHP:  exit(1);
来源：http://ic.bjjhwx.cn

JS:   process.exit(1)
来源：http://ga.gzmigu.cn

TS:   process.exit(1)
来源：http://wy.nszjky.cn

Java: System.exit(1)
来源：http://ot.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://gc.colortex.cn

Ruby: exit 1
来源：http://js.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gr.yuexingan06.cn

[M06] 向标准错误输出
来源：http://qj.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://rg.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ht.chemitech.net.cn

JS:   console.error("err")
来源：http://nc.lnxyls.cn

TS:   console.error("err")
来源：http://xw.shxzukj.cn

Java: System.err.println("err")
来源：http://vo.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pn.jianghongdianzi.cn

Ruby: warn "err"
来源：http://xq.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://nu.hnjuh.cn

[M07] 判断是否为主入口
来源：http://he.colortex.cn

Py:   if __name__ == "__main__":
来源：http://gy.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://co.haigaiapp.cn

JS:   require.main === module
来源：http://mr.newstarts.cn

TS:   require.main === module
来源：http://tg.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://qx.bookmarksfly.cn

Go:   func main()
来源：http://gz.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://za.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://gd.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://dn.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://rd.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://dv.hahajie.cn

JS:   process.platform;  process.version
来源：http://go.521024.cn

TS:   process.platform;  process.version
来源：http://mz.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gm.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ix.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pw.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gx.szsharing.cn

================================================================================
来源：http://js.bjjhwx.cn

N. 数据结构与算法
来源：http://gt.huixinmuqiang.cn

================================================================================
来源：http://yx.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://bi.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ja.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xl.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fi.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://as.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mz.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://sw.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://db.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vj.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ze.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://bq.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xh.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dg.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://se.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fw.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://lj.jianghongdianzi.cn

Ruby: arr.sort
来源：http://kn.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wx.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://cc.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://at.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://mt.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bl.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lx.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hk.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rr.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lt.asd995.cn

[N04] 斐波那契数列
来源：http://px.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://re.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ah.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pz.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ed.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qp.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wt.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tj.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://th.huixinmuqiang.cn

[N05] 最大公约数
来源：http://cm.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://sl.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bi.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wz.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dj.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://um.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yo.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://xx.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rh.shxzukj.cn

[N06] 判断回文字符串
来源：http://sx.yuexingan06.cn

Py:   s == s[::-1]
来源：http://gg.szsharing.cn

PHP:  $s === strrev($s);
来源：http://ez.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://jx.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://ce.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gu.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://sm.huanxung.cn

Ruby: s == s.reverse
来源：http://kk.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bk.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://ho.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rj.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fo.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jg.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://mt.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ja.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://zs.lnxyls.cn

Ruby: // 手写 Hash
来源：http://bf.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ja.gzmigu.cn

[N08] 生成全排列
来源：http://xp.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://mm.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://bm.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://ut.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://gz.szsharing.cn

Java: // 手写回溯递归
来源：http://ri.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://uv.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://yr.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://ei.chemitech.net.cn

[N09] 栈与队列
来源：http://jf.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://md.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mq.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ht.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ml.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mz.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://er.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://za.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lj.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://cm.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ks.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tm.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wf.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://or.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://oy.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qk.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nr.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ua.nszjky.cn

[N11] 二叉树中序遍历
来源：http://di.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fz.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://nw.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://er.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.muxihuayi.cn

Java: // 手写递归
来源：http://xa.nicolike.cn

Go:   // 手写递归
来源：http://od.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kx.shtwfgs.cn

C#:   // 手写递归
来源：http://nn.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nh.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vm.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ld.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cm.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xf.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kz.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sc.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aw.nicolike.cn

================================================================================
来源：http://bb.bookmarksfly.cn

O. 并发与异步
来源：http://wf.szxytkj.cn

================================================================================
来源：http://or.lnxyls.cn

[O01] 启动一个线程
来源：http://fa.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eq.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sb.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qm.nszjky.cn

TS:   // 同 JS
来源：http://yr.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://cu.hahajie.cn

Go:   go f()
来源：http://cv.hnjuh.cn

Ruby: Thread.new { f }
来源：http://qu.szsharing.cn

C#:   Task.Run(() => F());
来源：http://uw.jctech888.com.cn

[O02] 使用线程池
来源：http://xl.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ui.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ss.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://qb.nicolike.cn

TS:   // worker_threads 线程池
来源：http://nl.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://se.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ip.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ym.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kc.asd995.cn

[O03] 加锁保护共享数据
来源：http://lb.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://bb.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://cx.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oe.nszjky.cn

TS:   // 同 JS
来源：http://bl.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://lr.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jm.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ti.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://qu.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://hk.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ns.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nt.521024.cn

JS:   async function f() { await g(); }
来源：http://nb.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ei.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zb.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zf.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xt.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://hz.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://jw.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://fn.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rf.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://gq.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ig.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wr.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nq.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://wm.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://la.jctech888.com.cn

[O06] 使用进程池
来源：http://bq.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zl.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hh.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://nr.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://sa.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yn.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gk.9csxet.cn

Ruby: // fork 块
来源：http://yr.521024.cn

C#:   Parallel.For
来源：http://el.nicolike.cn

================================================================================
来源：http://uc.hahajie.cn

P. 常用工具函数
来源：http://id.yuntaijiaju.cn

================================================================================
来源：http://er.muxihuayi.cn

[P01] 生成 UUID
来源：http://cm.asd995.cn

Py:   str(uuid.uuid4())
来源：http://up.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://db.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://so.521024.cn

TS:   crypto.randomUUID()
来源：http://ic.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://ho.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://rk.asd995.cn

Ruby: SecureRandom.uuid
来源：http://md.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ui.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://yl.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://en.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hw.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://su.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://za.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mv.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ks.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mt.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ew.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ca.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://so.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tc.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wn.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nd.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pf.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rt.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pz.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dw.huixinmuqiang.cn

[P04] 求长度
来源：http://fn.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ff.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ib.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cq.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zm.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://oh.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://gg.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://hp.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oe.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://th.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qy.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uk.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nh.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ia.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ut.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ar.9csxet.cn

Ruby: a == b
来源：http://gi.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mp.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wl.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fz.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://up.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cc.bjjhwx.cn

TS:   if (x == null) {}
来源：http://mi.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ip.chemitech.net.cn

Go:   if x == nil {}
来源：http://lt.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ko.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://ca.9csxet.cn

[P07] 防抖与节流
来源：http://dh.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cv.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://lz.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lc.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ol.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xx.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ie.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dn.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://hy.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jx.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cz.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://go.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rj.huixinmuqiang.cn


<!-- 参考信息 -->