代发 wailian999

Ruby: ARGV
来源：http://ui.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://cl.9csxet.cn

[M02] 读取环境变量
来源：http://ve.asd995.cn

Py:   os.environ.get("HOME")
来源：http://gw.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yu.yuexingan06.cn

JS:   process.env.HOME
来源：http://xd.huanxung.cn

TS:   process.env.HOME
来源：http://sv.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://nb.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jc.asd995.cn

Ruby: ENV["HOME"]
来源：http://px.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qr.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://kn.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ms.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ps.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gj.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://om.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cf.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ig.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wh.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://iu.huanxung.cn

[M04] 获取当前工作目录
来源：http://tp.haigaiapp.cn

Py:   os.getcwd()
来源：http://vj.shxzukj.cn

PHP:  getcwd();
来源：http://pz.asd995.cn

JS:   process.cwd()
来源：http://wt.9csxet.cn

TS:   process.cwd()
来源：http://ky.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kx.chemitech.net.cn

Go:   os.Getwd()
来源：http://yv.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://iw.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yw.panjiajie.cn

[M05] 设置退出码
来源：http://tw.wgjwhj.cn

Py:   sys.exit(1)
来源：http://bq.jctech888.com.cn

PHP:  exit(1);
来源：http://cs.yuexingan06.cn

JS:   process.exit(1)
来源：http://zn.nicolike.cn

TS:   process.exit(1)
来源：http://wj.haigaiapp.cn

Java: System.exit(1)
来源：http://xs.newstarts.cn

Go:   os.Exit(1)
来源：http://ge.haigaiapp.cn

Ruby: exit 1
来源：http://om.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cl.newstarts.cn

[M06] 向标准错误输出
来源：http://md.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://xd.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jv.lnxyls.cn

JS:   console.error("err")
来源：http://rp.haigaiapp.cn

TS:   console.error("err")
来源：http://wf.haigaiapp.cn

Java: System.err.println("err")
来源：http://ju.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mf.yuntaijiaju.cn

Ruby: warn "err"
来源：http://zy.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://xb.szxytkj.cn

[M07] 判断是否为主入口
来源：http://zt.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://yl.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ag.9csxet.cn

JS:   require.main === module
来源：http://mb.szxytkj.cn

TS:   require.main === module
来源：http://zi.nszjky.cn

Java: public static void main(String[] args)
来源：http://tx.lnxyls.cn

Go:   func main()
来源：http://xw.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://px.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://me.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://wv.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://nx.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://li.9csxet.cn

JS:   process.platform;  process.version
来源：http://xc.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://yp.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xd.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bz.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kd.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nc.yuexingan06.cn

================================================================================
来源：http://mb.haigaiapp.cn

N. 数据结构与算法
来源：http://vr.chemitech.net.cn

================================================================================
来源：http://hi.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://zj.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ps.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ur.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tg.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qn.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xr.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://cb.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bh.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dk.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ok.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://xf.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rk.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sg.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kz.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uu.521024.cn

Go:   slices.Sort(arr)
来源：http://eo.szxytkj.cn

Ruby: arr.sort
来源：http://ls.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nb.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://wk.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ro.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://ih.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zi.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hx.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ou.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wd.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://om.hnjuh.cn

[N04] 斐波那契数列
来源：http://ca.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fj.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rm.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fc.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oy.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vz.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://et.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lc.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hf.gzmigu.cn

[N05] 最大公约数
来源：http://hx.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ri.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jm.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hh.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ke.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xj.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://de.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://wd.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://za.shxzskj.cn

[N06] 判断回文字符串
来源：http://pj.shtwfgs.cn

Py:   s == s[::-1]
来源：http://wd.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://pd.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://zx.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://kv.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tt.nszjky.cn

Go:   // 双指针从两端比较
来源：http://yf.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://qb.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gz.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://pz.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gh.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gn.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dy.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://zc.nicolike.cn

Java: // 手写 HashMap
来源：http://dn.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://jo.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://bo.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wb.shtwfgs.cn

[N08] 生成全排列
来源：http://jl.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://us.gzmigu.cn

PHP:  // 手写递归交换
来源：http://tn.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://bu.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://hw.wgjwhj.cn

Java: // 手写回溯递归
来源：http://rn.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://vk.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://pv.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://mp.huanxung.cn

[N09] 栈与队列
来源：http://wg.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xg.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cs.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yo.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rj.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zy.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zb.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wi.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cr.muxihuayi.cn

[N10] 链表节点定义
来源：http://uj.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dv.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xg.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ot.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zm.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://uh.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rk.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qx.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ko.9csxet.cn

[N11] 二叉树中序遍历
来源：http://zg.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uv.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://if.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://su.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sz.colortex.cn

Java: // 手写递归
来源：http://tt.hahajie.cn

Go:   // 手写递归
来源：http://dt.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://es.jctech888.com.cn

C#:   // 手写递归
来源：http://cm.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gm.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bo.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pb.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://um.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xm.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sl.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fj.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xt.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dl.asd995.cn

================================================================================
来源：http://kn.wgjwhj.cn

O. 并发与异步
来源：http://nt.nszjky.cn

================================================================================
来源：http://op.hnjuh.cn

[O01] 启动一个线程
来源：http://li.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yy.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hb.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fp.shxzukj.cn

TS:   // 同 JS
来源：http://ow.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://br.shxzskj.cn

Go:   go f()
来源：http://ip.nicolike.cn

Ruby: Thread.new { f }
来源：http://ze.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://pf.nszjky.cn

[O02] 使用线程池
来源：http://he.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qr.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mk.hahajie.cn

JS:   // worker_threads 线程池
来源：http://xo.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://wg.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://la.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pr.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uy.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xp.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://id.szsharing.cn

Py:   with lock: shared += 1
来源：http://hc.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://oz.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dw.yuexingan06.cn

TS:   // 同 JS
来源：http://pq.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://em.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jb.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lq.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://hw.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://ot.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://lu.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nr.9csxet.cn

JS:   async function f() { await g(); }
来源：http://tf.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zx.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yf.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ee.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vj.asd995.cn

C#:   async Task F() { await G(); }
来源：http://lh.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://qi.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://sv.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oo.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://pm.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://xo.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lr.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xz.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://zs.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://am.bjjhwx.cn

[O06] 使用进程池
来源：http://im.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ha.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fa.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://hj.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://ux.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ml.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eu.shtwfgs.cn

Ruby: // fork 块
来源：http://br.jctech888.com.cn

C#:   Parallel.For
来源：http://vt.shxzukj.cn

================================================================================
来源：http://ba.huixinmuqiang.cn

P. 常用工具函数
来源：http://cp.hnjuh.cn

================================================================================
来源：http://tj.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://qq.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://ch.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yx.9csxet.cn

JS:   crypto.randomUUID()
来源：http://kc.hahajie.cn

TS:   crypto.randomUUID()
来源：http://fb.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://qv.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://np.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://fq.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://ja.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://fg.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ma.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://da.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://we.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ch.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zp.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kf.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zn.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xn.lnxyls.cn

[P03] 生成短随机字符串
来源：http://fb.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://an.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yd.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://is.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dt.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hq.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cv.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vq.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aw.panjiajie.cn

[P04] 求长度
来源：http://na.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wa.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hp.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uq.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wy.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://hl.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://tn.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://ll.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ce.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://lp.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hc.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tx.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rz.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mj.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nk.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ln.haigaiapp.cn

Ruby: a == b
来源：http://dh.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eb.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zy.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://so.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://dr.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zj.gzmigu.cn

TS:   if (x == null) {}
来源：http://ug.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xz.bookmarksfly.cn

Go:   if x == nil {}
来源：http://ni.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eg.hahajie.cn

C#:   if (x is null) {}
来源：http://pf.yuexingan06.cn

[P07] 防抖与节流
来源：http://pl.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sz.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://dl.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zq.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ul.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gq.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rr.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://by.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://bd.bookmarksfly.cn


<!-- 参考信息 -->