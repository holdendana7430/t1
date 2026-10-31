代发 wailian999

Ruby: ARGV
来源：http://zi.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://zx.shxzukj.cn

[M02] 读取环境变量
来源：http://la.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://kf.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ao.wgjwhj.cn

JS:   process.env.HOME
来源：http://xz.nicolike.cn

TS:   process.env.HOME
来源：http://gc.asd995.cn

Java: System.getenv("HOME")
来源：http://xr.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fc.nicolike.cn

Ruby: ENV["HOME"]
来源：http://yn.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://za.nicolike.cn

[M03] 执行外部命令
来源：http://sv.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pv.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://su.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hh.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fi.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vp.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bl.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qz.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://xj.521024.cn

[M04] 获取当前工作目录
来源：http://gm.nicolike.cn

Py:   os.getcwd()
来源：http://rc.hnjuh.cn

PHP:  getcwd();
来源：http://zj.chemitech.net.cn

JS:   process.cwd()
来源：http://hz.szxytkj.cn

TS:   process.cwd()
来源：http://ti.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://lc.nszjky.cn

Go:   os.Getwd()
来源：http://ch.szsharing.cn

Ruby: Dir.pwd
来源：http://yw.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ef.szxytkj.cn

[M05] 设置退出码
来源：http://td.nicolike.cn

Py:   sys.exit(1)
来源：http://be.bjjhwx.cn

PHP:  exit(1);
来源：http://bn.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://my.hahajie.cn

TS:   process.exit(1)
来源：http://zx.yuexingan06.cn

Java: System.exit(1)
来源：http://an.shtwfgs.cn

Go:   os.Exit(1)
来源：http://vy.jctech888.com.cn

Ruby: exit 1
来源：http://rn.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mt.haigaiapp.cn

[M06] 向标准错误输出
来源：http://rt.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://iz.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://un.newstarts.cn

JS:   console.error("err")
来源：http://vi.chemitech.net.cn

TS:   console.error("err")
来源：http://ix.bjjhwx.cn

Java: System.err.println("err")
来源：http://ec.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zb.shxzskj.cn

Ruby: warn "err"
来源：http://po.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ze.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://df.asd995.cn

Py:   if __name__ == "__main__":
来源：http://rn.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tj.hahajie.cn

JS:   require.main === module
来源：http://it.panjiajie.cn

TS:   require.main === module
来源：http://mz.shxzskj.cn

Java: public static void main(String[] args)
来源：http://cp.shxzukj.cn

Go:   func main()
来源：http://kn.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ev.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://xh.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://lp.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://vg.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://da.shxzukj.cn

JS:   process.platform;  process.version
来源：http://yc.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://yn.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yf.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://df.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nj.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://te.yuntaijiaju.cn

================================================================================
来源：http://zw.bookmarksfly.cn

N. 数据结构与算法
来源：http://wq.asd995.cn

================================================================================
来源：http://ab.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://zi.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qd.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vf.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://me.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tl.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gt.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://am.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ab.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qt.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://hb.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://er.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ry.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gx.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gp.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bx.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://xn.bjjhwx.cn

Ruby: arr.sort
来源：http://ux.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pt.521024.cn

[N03] 快速排序（分治示例）
来源：http://tv.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ns.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://jn.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://er.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xx.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bp.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ub.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cq.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://be.lnxyls.cn

[N04] 斐波那契数列
来源：http://lp.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://er.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wq.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://is.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bd.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xk.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aa.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://do.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rr.yuexingan06.cn

[N05] 最大公约数
来源：http://kb.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ze.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cb.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tt.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kl.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kz.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ef.521024.cn

Ruby: a.gcd(b)
来源：http://rf.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cl.shtwfgs.cn

[N06] 判断回文字符串
来源：http://oq.chemitech.net.cn

Py:   s == s[::-1]
来源：http://ik.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://cb.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://vh.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://qq.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tk.asd995.cn

Go:   // 双指针从两端比较
来源：http://bu.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ef.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hf.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://zk.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yo.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fv.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xn.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://sg.nicolike.cn

Java: // 手写 HashMap
来源：http://db.newstarts.cn

Go:   // 手写 map[int]int
来源：http://pe.szsharing.cn

Ruby: // 手写 Hash
来源：http://ug.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mg.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ly.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://zm.shxzskj.cn

PHP:  // 手写递归交换
来源：http://bv.szsharing.cn

JS:   // 手写回溯递归
来源：http://bt.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://fu.9csxet.cn

Java: // 手写回溯递归
来源：http://ha.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://rs.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://rb.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ok.shxzukj.cn

[N09] 栈与队列
来源：http://zq.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ti.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yw.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sz.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wp.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uj.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ob.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ve.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://au.huanxung.cn

[N10] 链表节点定义
来源：http://ce.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kh.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rk.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ma.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wh.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://in.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nh.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fk.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fw.hahajie.cn

[N11] 二叉树中序遍历
来源：http://wo.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pj.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://ob.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bx.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oq.jianghongdianzi.cn

Java: // 手写递归
来源：http://eo.bjjhwx.cn

Go:   // 手写递归
来源：http://kb.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bu.9csxet.cn

C#:   // 手写递归
来源：http://sr.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ub.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ac.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://go.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gc.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bb.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vg.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zz.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ln.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hp.jctech888.com.cn

================================================================================
来源：http://an.shtwfgs.cn

O. 并发与异步
来源：http://pk.muxihuayi.cn

================================================================================
来源：http://bx.asd995.cn

[O01] 启动一个线程
来源：http://py.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jm.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fh.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qj.jctech888.com.cn

TS:   // 同 JS
来源：http://al.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://yu.muxihuayi.cn

Go:   go f()
来源：http://hr.hahajie.cn

Ruby: Thread.new { f }
来源：http://tr.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://ox.muxihuayi.cn

[O02] 使用线程池
来源：http://mg.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iv.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tg.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://zv.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://sd.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fc.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bu.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://es.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ek.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://un.asd995.cn

Py:   with lock: shared += 1
来源：http://li.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://jw.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tw.bookmarksfly.cn

TS:   // 同 JS
来源：http://hz.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://np.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tk.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://am.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://xc.szsharing.cn

[O04] 定义异步函数并等待
来源：http://jr.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://cv.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bw.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://of.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kz.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ca.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ea.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ww.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://nl.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://vg.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://no.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ed.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://fu.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://oc.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zw.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sx.nszjky.cn

Ruby: threads.map(&:join)
来源：http://yv.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cd.huixiangedu.cn

[O06] 使用进程池
来源：http://hq.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ms.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oz.colortex.cn

JS:   // child_process / cluster 模块
来源：http://sr.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://pr.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xl.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lu.wgjwhj.cn

Ruby: // fork 块
来源：http://qr.gzmigu.cn

C#:   Parallel.For
来源：http://yc.nszjky.cn

================================================================================
来源：http://gn.bjjhwx.cn

P. 常用工具函数
来源：http://fj.newstarts.cn

================================================================================
来源：http://da.hahajie.cn

[P01] 生成 UUID
来源：http://wp.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://dq.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fv.nicolike.cn

JS:   crypto.randomUUID()
来源：http://dz.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ez.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://vr.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://zm.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://ih.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://fr.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://bi.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oy.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oo.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eg.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gn.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ix.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ch.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://po.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://do.521024.cn

[P03] 生成短随机字符串
来源：http://bx.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://da.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zi.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oy.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://un.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vl.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bp.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cs.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dd.jctech888.com.cn

[P04] 求长度
来源：http://kk.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ud.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wr.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gw.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qy.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://mo.nicolike.cn

Go:   len(arr);  len(m)
来源：http://tl.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://hz.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ty.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://kj.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mc.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qq.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cd.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yf.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fr.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tv.huanxung.cn

Ruby: a == b
来源：http://fr.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qc.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://to.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pi.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://aj.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pr.hahajie.cn

TS:   if (x == null) {}
来源：http://pr.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iu.yuexingan06.cn

Go:   if x == nil {}
来源：http://jg.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rc.muxihuayi.cn

C#:   if (x is null) {}
来源：http://ue.panjiajie.cn

[P07] 防抖与节流
来源：http://nt.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cj.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://rp.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pr.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wn.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://by.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://na.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vs.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://ie.shxzukj.cn


<!-- 参考信息 -->