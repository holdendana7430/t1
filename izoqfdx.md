代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://td.shtwfgs.cn

JS:   process.env.HOME
来源：http://my.huixiangedu.cn

TS:   process.env.HOME
来源：http://oa.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://cj.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pf.asd995.cn

Ruby: ENV["HOME"]
来源：http://ed.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://an.chemitech.net.cn

[M03] 执行外部命令
来源：http://lp.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qq.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://us.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rd.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tt.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bh.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fl.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qm.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://xh.hahajie.cn

[M04] 获取当前工作目录
来源：http://kc.shxzukj.cn

Py:   os.getcwd()
来源：http://ux.chemitech.net.cn

PHP:  getcwd();
来源：http://vw.huanxung.cn

JS:   process.cwd()
来源：http://tz.chemitech.net.cn

TS:   process.cwd()
来源：http://ps.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://dh.yuexingan06.cn

Go:   os.Getwd()
来源：http://yi.huanxung.cn

Ruby: Dir.pwd
来源：http://ld.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gi.yuexingan06.cn

[M05] 设置退出码
来源：http://zf.hahajie.cn

Py:   sys.exit(1)
来源：http://cr.wgjwhj.cn

PHP:  exit(1);
来源：http://rl.9csxet.cn

JS:   process.exit(1)
来源：http://dp.bookmarksfly.cn

TS:   process.exit(1)
来源：http://au.shxzskj.cn

Java: System.exit(1)
来源：http://yz.521024.cn

Go:   os.Exit(1)
来源：http://qj.hnjuh.cn

Ruby: exit 1
来源：http://ua.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ah.jctech888.com.cn

[M06] 向标准错误输出
来源：http://lz.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://wk.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fl.bookmarksfly.cn

JS:   console.error("err")
来源：http://gs.shxzukj.cn

TS:   console.error("err")
来源：http://tg.muxihuayi.cn

Java: System.err.println("err")
来源：http://vr.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bv.shtwfgs.cn

Ruby: warn "err"
来源：http://qu.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ic.hahajie.cn

[M07] 判断是否为主入口
来源：http://yl.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://wj.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sy.asd995.cn

JS:   require.main === module
来源：http://ma.jianghongdianzi.cn

TS:   require.main === module
来源：http://ka.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://me.wgjwhj.cn

Go:   func main()
来源：http://lk.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dv.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://fu.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://ey.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://pf.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://lm.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://fy.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://ld.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ui.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ig.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ii.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fd.nszjky.cn

================================================================================
来源：http://pz.hnjuh.cn

N. 数据结构与算法
来源：http://yr.haigaiapp.cn

================================================================================
来源：http://bb.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://tm.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bx.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ap.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jo.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cl.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zc.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://ms.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ol.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qk.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://kx.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://kt.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kv.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ki.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pk.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tt.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://si.hahajie.cn

Ruby: arr.sort
来源：http://fv.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://me.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://sl.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://my.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://da.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zg.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zp.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ms.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sx.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xh.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xk.shxzskj.cn

[N04] 斐波那契数列
来源：http://li.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ds.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ir.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://me.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nn.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://av.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aa.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://co.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nx.huixinmuqiang.cn

[N05] 最大公约数
来源：http://uu.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://tc.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://su.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rn.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sl.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nq.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fs.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://qt.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yg.muxihuayi.cn

[N06] 判断回文字符串
来源：http://xu.huixiangedu.cn

Py:   s == s[::-1]
来源：http://li.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://hq.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://wm.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://zh.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://by.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://wq.521024.cn

Ruby: s == s.reverse
来源：http://wy.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ui.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://xf.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zm.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fv.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ul.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://en.hahajie.cn

Java: // 手写 HashMap
来源：http://tw.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://gl.gzmigu.cn

Ruby: // 手写 Hash
来源：http://mo.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pb.bookmarksfly.cn

[N08] 生成全排列
来源：http://mi.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://cb.panjiajie.cn

PHP:  // 手写递归交换
来源：http://bw.shxzukj.cn

JS:   // 手写回溯递归
来源：http://rq.colortex.cn

TS:   // 手写回溯递归
来源：http://df.huixiangedu.cn

Java: // 手写回溯递归
来源：http://qv.nszjky.cn

Go:   // 手写回溯递归
来源：http://yj.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://vt.huanxung.cn

C#:   // 手写回溯递归
来源：http://nz.huixinmuqiang.cn

[N09] 栈与队列
来源：http://wt.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mh.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pv.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://er.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nh.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://st.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bz.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://og.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://lr.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mg.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lq.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ss.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ae.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://lj.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cm.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dw.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://td.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://aj.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iz.hahajie.cn

PHP:  // 手写递归函数
来源：http://va.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uw.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jn.nicolike.cn

Java: // 手写递归
来源：http://gg.huanxung.cn

Go:   // 手写递归
来源：http://ks.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ui.shxzukj.cn

C#:   // 手写递归
来源：http://ik.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nq.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://by.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mx.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tv.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cj.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dq.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lo.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ru.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sy.haigaiapp.cn

================================================================================
来源：http://ev.lnxyls.cn

O. 并发与异步
来源：http://hh.huanxung.cn

================================================================================
来源：http://ax.szxytkj.cn

[O01] 启动一个线程
来源：http://xo.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://et.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fk.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uu.jianghongdianzi.cn

TS:   // 同 JS
来源：http://lf.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://jj.gzmigu.cn

Go:   go f()
来源：http://ln.gzmigu.cn

Ruby: Thread.new { f }
来源：http://cr.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://sc.newstarts.cn

[O02] 使用线程池
来源：http://gi.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ls.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ua.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://ju.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://tf.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tr.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bi.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tk.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zo.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://yz.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://jm.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://sl.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ln.huixiangedu.cn

TS:   // 同 JS
来源：http://jv.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://nx.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lw.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hc.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://ho.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://lt.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://sh.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yh.huanxung.cn

JS:   async function f() { await g(); }
来源：http://nk.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uc.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qr.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ny.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sj.521024.cn

C#:   async Task F() { await G(); }
来源：http://ym.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://mx.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://gv.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kt.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://sy.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://yf.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yg.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lx.szsharing.cn

Ruby: threads.map(&:join)
来源：http://iq.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gx.shxzskj.cn

[O06] 使用进程池
来源：http://qk.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nq.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uq.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://dr.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://fw.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yc.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rh.wgjwhj.cn

Ruby: // fork 块
来源：http://lz.9csxet.cn

C#:   Parallel.For
来源：http://pi.lnxyls.cn

================================================================================
来源：http://no.newstarts.cn

P. 常用工具函数
来源：http://cy.haigaiapp.cn

================================================================================
来源：http://wt.bookmarksfly.cn

[P01] 生成 UUID
来源：http://pz.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://un.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ml.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://tq.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://kn.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://na.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://wi.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://qj.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://vt.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://rs.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dj.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ds.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ia.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iv.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nd.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wy.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mj.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vy.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://kd.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fz.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gi.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://go.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xq.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iy.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vx.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ar.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qf.szsharing.cn

[P04] 求长度
来源：http://pg.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kf.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ds.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://to.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ls.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://bx.asd995.cn

Go:   len(arr);  len(m)
来源：http://wi.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://ef.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lo.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://xc.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nb.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tx.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zp.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sg.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ba.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ca.newstarts.cn

Ruby: a == b
来源：http://fq.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qp.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ic.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nw.521024.cn

PHP:  if (empty($x)) {}
来源：http://az.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ui.gzmigu.cn

TS:   if (x == null) {}
来源：http://no.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mp.huanxung.cn

Go:   if x == nil {}
来源：http://lk.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://us.521024.cn

C#:   if (x is null) {}
来源：http://ab.newstarts.cn

[P07] 防抖与节流
来源：http://lv.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rj.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://vr.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rc.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uz.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://up.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rc.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vs.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vd.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://rl.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mv.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iv.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rm.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ij.szxytkj.cn


<!-- 参考信息 -->