代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.shxzukj.cn

JS:   process.env.HOME
来源：http://fy.9csxet.cn

TS:   process.env.HOME
来源：http://po.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://dh.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tn.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://hy.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://my.chemitech.net.cn

[M03] 执行外部命令
来源：http://tv.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hi.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ve.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cq.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sn.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qv.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pp.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fz.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://xg.szsharing.cn

[M04] 获取当前工作目录
来源：http://up.shxzskj.cn

Py:   os.getcwd()
来源：http://iu.yuntaijiaju.cn

PHP:  getcwd();
来源：http://ts.asd995.cn

JS:   process.cwd()
来源：http://ew.bjjhwx.cn

TS:   process.cwd()
来源：http://yu.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://je.szsharing.cn

Go:   os.Getwd()
来源：http://cz.shtwfgs.cn

Ruby: Dir.pwd
来源：http://gg.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uo.9csxet.cn

[M05] 设置退出码
来源：http://gm.bjjhwx.cn

Py:   sys.exit(1)
来源：http://ep.nicolike.cn

PHP:  exit(1);
来源：http://bj.nszjky.cn

JS:   process.exit(1)
来源：http://kl.wgjwhj.cn

TS:   process.exit(1)
来源：http://bh.hahajie.cn

Java: System.exit(1)
来源：http://sx.521024.cn

Go:   os.Exit(1)
来源：http://ql.muxihuayi.cn

Ruby: exit 1
来源：http://tn.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ol.muxihuayi.cn

[M06] 向标准错误输出
来源：http://oo.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ha.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://to.wgjwhj.cn

JS:   console.error("err")
来源：http://pn.huanxung.cn

TS:   console.error("err")
来源：http://ft.newstarts.cn

Java: System.err.println("err")
来源：http://zn.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ho.hahajie.cn

Ruby: warn "err"
来源：http://jb.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://xx.nicolike.cn

[M07] 判断是否为主入口
来源：http://nb.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://lj.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wg.shxzskj.cn

JS:   require.main === module
来源：http://ma.bjjhwx.cn

TS:   require.main === module
来源：http://cs.szxytkj.cn

Java: public static void main(String[] args)
来源：http://fa.huanxung.cn

Go:   func main()
来源：http://nz.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wj.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://mr.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://mb.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ar.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://sv.colortex.cn

JS:   process.platform;  process.version
来源：http://rl.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://bo.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zg.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://if.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://na.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lz.shtwfgs.cn

================================================================================
来源：http://qz.panjiajie.cn

N. 数据结构与算法
来源：http://cv.gzmigu.cn

================================================================================
来源：http://eq.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://vi.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ta.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oo.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sr.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qq.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ja.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://aj.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dc.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jn.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://ij.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fk.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aa.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mc.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fd.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://el.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://fl.szsharing.cn

Ruby: arr.sort
来源：http://rw.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bb.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://hb.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pk.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://lb.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nf.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ax.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ei.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ru.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cj.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xr.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://km.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wa.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lb.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pt.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yu.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yt.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://am.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pk.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jh.hnjuh.cn

[N05] 最大公约数
来源：http://tm.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://cs.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tg.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rm.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ip.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yg.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yp.szsharing.cn

Ruby: a.gcd(b)
来源：http://ld.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qu.wgjwhj.cn

[N06] 判断回文字符串
来源：http://wl.shxzukj.cn

Py:   s == s[::-1]
来源：http://lg.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://tz.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://hz.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://gc.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://si.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://dg.gzmigu.cn

Ruby: s == s.reverse
来源：http://ux.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xi.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://po.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xw.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dw.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tc.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://nd.muxihuayi.cn

Java: // 手写 HashMap
来源：http://yz.newstarts.cn

Go:   // 手写 map[int]int
来源：http://cb.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://ey.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ni.chemitech.net.cn

[N08] 生成全排列
来源：http://tp.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://cd.nszjky.cn

PHP:  // 手写递归交换
来源：http://sn.nicolike.cn

JS:   // 手写回溯递归
来源：http://dj.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://fw.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://iy.huanxung.cn

Go:   // 手写回溯递归
来源：http://ep.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://hn.521024.cn

C#:   // 手写回溯递归
来源：http://fl.huixiangedu.cn

[N09] 栈与队列
来源：http://hu.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vt.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iz.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mz.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://om.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zu.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pi.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qw.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sm.shxzskj.cn

[N10] 链表节点定义
来源：http://rd.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wk.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vn.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oc.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kf.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://vz.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cr.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cf.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pn.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://ia.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vb.colortex.cn

PHP:  // 手写递归函数
来源：http://ly.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bz.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qs.szxytkj.cn

Java: // 手写递归
来源：http://uk.szsharing.cn

Go:   // 手写递归
来源：http://hj.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wr.colortex.cn

C#:   // 手写递归
来源：http://qa.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://im.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qm.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rw.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qf.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bj.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xr.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ed.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kp.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bn.chemitech.net.cn

================================================================================
来源：http://ic.newstarts.cn

O. 并发与异步
来源：http://lh.521024.cn

================================================================================
来源：http://og.jctech888.com.cn

[O01] 启动一个线程
来源：http://us.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ut.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vb.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rt.huixiangedu.cn

TS:   // 同 JS
来源：http://zw.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://iz.colortex.cn

Go:   go f()
来源：http://bw.shxzskj.cn

Ruby: Thread.new { f }
来源：http://rh.szsharing.cn

C#:   Task.Run(() => F());
来源：http://st.yuexingan06.cn

[O02] 使用线程池
来源：http://xd.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ig.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cf.nszjky.cn

JS:   // worker_threads 线程池
来源：http://gn.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://mh.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fo.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wp.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ha.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xm.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://pw.shxzskj.cn

Py:   with lock: shared += 1
来源：http://jz.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://ay.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xb.lnxyls.cn

TS:   // 同 JS
来源：http://vs.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://jt.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vf.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ag.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://wl.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://aw.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://xe.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ff.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://fc.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://po.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gc.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mj.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hc.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://mk.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://jv.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://dd.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qs.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ls.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://qa.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gs.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sy.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://bo.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lq.huanxung.cn

[O06] 使用进程池
来源：http://xz.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://df.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cm.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://wl.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://xt.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mp.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xs.muxihuayi.cn

Ruby: // fork 块
来源：http://hg.bookmarksfly.cn

C#:   Parallel.For
来源：http://ra.haigaiapp.cn

================================================================================
来源：http://jd.shtwfgs.cn

P. 常用工具函数
来源：http://hi.9csxet.cn

================================================================================
来源：http://ui.shxzskj.cn

[P01] 生成 UUID
来源：http://jc.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://sr.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dz.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ol.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://jf.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://lk.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://bk.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://qr.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://rf.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://gx.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wr.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kc.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ix.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sz.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ir.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://io.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pp.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dn.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://ub.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kv.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dz.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://di.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ui.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zt.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nr.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cg.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ay.muxihuayi.cn

[P04] 求长度
来源：http://xm.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sf.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ju.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ra.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://qp.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://ti.szsharing.cn

Ruby: x.length;  x.size
来源：http://me.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ch.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://hi.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://en.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cp.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eo.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lj.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fo.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bh.chemitech.net.cn

Ruby: a == b
来源：http://sl.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://us.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jb.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fa.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ob.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pe.shxzskj.cn

TS:   if (x == null) {}
来源：http://ot.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cy.nicolike.cn

Go:   if x == nil {}
来源：http://gq.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xs.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ie.yuexingan06.cn

[P07] 防抖与节流
来源：http://lh.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yg.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://mo.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sy.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wp.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fn.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fc.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sp.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jb.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://yp.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kp.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jx.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gq.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ns.bookmarksfly.cn


<!-- 参考信息 -->