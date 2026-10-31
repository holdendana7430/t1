代发 wailian999

Ruby: ARGV
来源：http://rk.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://uj.shxzukj.cn

[M02] 读取环境变量
来源：http://rl.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://oa.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dx.hnjuh.cn

JS:   process.env.HOME
来源：http://gg.shxzukj.cn

TS:   process.env.HOME
来源：http://uu.szsharing.cn

Java: System.getenv("HOME")
来源：http://zk.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ek.hahajie.cn

Ruby: ENV["HOME"]
来源：http://cy.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fh.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://fq.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sj.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zf.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vh.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sm.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bc.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tm.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xy.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ad.colortex.cn

[M04] 获取当前工作目录
来源：http://pd.nicolike.cn

Py:   os.getcwd()
来源：http://jt.panjiajie.cn

PHP:  getcwd();
来源：http://cw.haigaiapp.cn

JS:   process.cwd()
来源：http://bb.9csxet.cn

TS:   process.cwd()
来源：http://to.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://le.wgjwhj.cn

Go:   os.Getwd()
来源：http://ek.wgjwhj.cn

Ruby: Dir.pwd
来源：http://fd.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://km.bjjhwx.cn

[M05] 设置退出码
来源：http://wf.521024.cn

Py:   sys.exit(1)
来源：http://rt.jianghongdianzi.cn

PHP:  exit(1);
来源：http://eq.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://dn.shxzukj.cn

TS:   process.exit(1)
来源：http://rl.hahajie.cn

Java: System.exit(1)
来源：http://tu.asd995.cn

Go:   os.Exit(1)
来源：http://sz.shxzskj.cn

Ruby: exit 1
来源：http://hf.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xg.lnxyls.cn

[M06] 向标准错误输出
来源：http://up.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://vn.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ol.szsharing.cn

JS:   console.error("err")
来源：http://wn.szxytkj.cn

TS:   console.error("err")
来源：http://fd.yuexingan06.cn

Java: System.err.println("err")
来源：http://xc.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wx.panjiajie.cn

Ruby: warn "err"
来源：http://zn.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://eg.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://xk.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://ld.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kz.asd995.cn

JS:   require.main === module
来源：http://hk.colortex.cn

TS:   require.main === module
来源：http://ex.newstarts.cn

Java: public static void main(String[] args)
来源：http://lr.wgjwhj.cn

Go:   func main()
来源：http://hk.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ud.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://za.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://fu.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://ev.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://uq.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://or.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ks.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hq.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zh.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zc.shxzskj.cn

================================================================================
来源：http://mw.newstarts.cn

N. 数据结构与算法
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://ob.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://nw.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rk.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aj.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xi.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qa.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xv.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://go.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://go.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pd.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://oa.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ih.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rc.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bw.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ir.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://it.huixiangedu.cn

Ruby: arr.sort
来源：http://kx.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zl.521024.cn

[N03] 快速排序（分治示例）
来源：http://bz.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bk.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://yv.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ip.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rk.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nv.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hc.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cd.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pt.521024.cn

[N04] 斐波那契数列
来源：http://sp.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dj.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vh.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rk.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yn.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nb.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hi.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ei.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sg.wgjwhj.cn

[N05] 最大公约数
来源：http://dt.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://mi.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rg.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xf.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wk.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pw.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://kx.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ln.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://rp.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://gs.newstarts.cn

PHP:  $s === strrev($s);
来源：http://cr.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ev.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://rf.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ky.nszjky.cn

Go:   // 双指针从两端比较
来源：http://sb.shxzskj.cn

Ruby: s == s.reverse
来源：http://no.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qn.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://uq.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wg.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rz.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://as.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://kh.hnjuh.cn

Java: // 手写 HashMap
来源：http://lm.huanxung.cn

Go:   // 手写 map[int]int
来源：http://rs.panjiajie.cn

Ruby: // 手写 Hash
来源：http://hi.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://in.szxytkj.cn

[N08] 生成全排列
来源：http://zq.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://tk.huanxung.cn

PHP:  // 手写递归交换
来源：http://ex.9csxet.cn

JS:   // 手写回溯递归
来源：http://vk.huanxung.cn

TS:   // 手写回溯递归
来源：http://nw.asd995.cn

Java: // 手写回溯递归
来源：http://md.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://he.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://mx.gzmigu.cn

C#:   // 手写回溯递归
来源：http://mv.huanxung.cn

[N09] 栈与队列
来源：http://zv.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uh.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qh.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://po.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bu.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zs.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mz.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vs.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oh.wgjwhj.cn

[N10] 链表节点定义
来源：http://en.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ny.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fs.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nw.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.521024.cn

Java: class Node { int v; Node next; }
来源：http://ns.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dy.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mt.colortex.cn

[N11] 二叉树中序遍历
来源：http://ak.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oy.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ab.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mk.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://go.9csxet.cn

Java: // 手写递归
来源：http://ug.jctech888.com.cn

Go:   // 手写递归
来源：http://jq.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ou.szxytkj.cn

C#:   // 手写递归
来源：http://jf.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ze.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cr.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ir.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mt.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ea.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bw.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bk.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fq.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hk.gzmigu.cn

================================================================================
来源：http://yg.jctech888.com.cn

O. 并发与异步
来源：http://ge.yuntaijiaju.cn

================================================================================
来源：http://oy.asd995.cn

[O01] 启动一个线程
来源：http://zb.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ga.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ey.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://my.lnxyls.cn

TS:   // 同 JS
来源：http://zi.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://do.newstarts.cn

Go:   go f()
来源：http://nm.panjiajie.cn

Ruby: Thread.new { f }
来源：http://yu.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://jz.yuntaijiaju.cn

[O02] 使用线程池
来源：http://ba.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gr.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sj.newstarts.cn

JS:   // worker_threads 线程池
来源：http://qm.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://wv.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lm.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ny.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mf.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bz.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ek.szsharing.cn

Py:   with lock: shared += 1
来源：http://aj.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://tl.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cr.yuexingan06.cn

TS:   // 同 JS
来源：http://up.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://pg.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yw.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://np.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ps.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://mh.521024.cn

Py:   async def f():⏎    await g()
来源：http://hx.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sy.colortex.cn

JS:   async function f() { await g(); }
来源：http://dm.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bt.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nb.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ig.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zn.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ke.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://lq.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://yj.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kz.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://gd.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://of.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xs.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://da.asd995.cn

Ruby: threads.map(&:join)
来源：http://qi.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fh.szxytkj.cn

[O06] 使用进程池
来源：http://rc.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jq.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yr.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://pb.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://pl.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://js.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ph.nicolike.cn

Ruby: // fork 块
来源：http://rj.jctech888.com.cn

C#:   Parallel.For
来源：http://ws.jianghongdianzi.cn

================================================================================
来源：http://qd.chemitech.net.cn

P. 常用工具函数
来源：http://rn.bjjhwx.cn

================================================================================
来源：http://vk.shxzskj.cn

[P01] 生成 UUID
来源：http://bw.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://xu.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dd.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://ae.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ai.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://rv.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://io.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://md.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://oh.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://tt.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://an.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ts.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dl.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wa.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vs.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fw.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lt.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vk.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://bf.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://um.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yk.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://me.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rn.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gz.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://px.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://de.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ip.gzmigu.cn

[P04] 求长度
来源：http://xk.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yr.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://la.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ni.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gw.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://xd.szsharing.cn

Go:   len(arr);  len(m)
来源：http://uq.shxzskj.cn

Ruby: x.length;  x.size
来源：http://ei.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qt.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://ex.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eq.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nt.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wm.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://su.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wt.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fi.szxytkj.cn

Ruby: a == b
来源：http://dk.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://la.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fg.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yu.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://tn.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lc.521024.cn

TS:   if (x == null) {}
来源：http://xb.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ja.szsharing.cn

Go:   if x == nil {}
来源：http://hl.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://en.jctech888.com.cn

C#:   if (x is null) {}
来源：http://bg.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ro.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hk.colortex.cn

PHP:  // 手写时间戳比较
来源：http://nn.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gh.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bs.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lf.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://py.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xq.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uv.nicolike.cn

[P08] 处理浮点精度问题
来源：http://lo.nicolike.cn


<!-- 参考信息 -->