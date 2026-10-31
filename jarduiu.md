代发 wailian999

JS:   process.argv.slice(2)
来源：http://xy.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://kp.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ia.newstarts.cn

Go:   os.Args[1:]
来源：http://ar.haigaiapp.cn

Ruby: ARGV
来源：http://ia.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://ji.wgjwhj.cn

[M02] 读取环境变量
来源：http://wj.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://dn.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oh.wgjwhj.cn

JS:   process.env.HOME
来源：http://aq.haigaiapp.cn

TS:   process.env.HOME
来源：http://po.nicolike.cn

Java: System.getenv("HOME")
来源：http://we.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pj.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://gy.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vg.jctech888.com.cn

[M03] 执行外部命令
来源：http://tt.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cm.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fw.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hn.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mb.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zl.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hp.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ho.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://fh.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://tr.gzmigu.cn

Py:   os.getcwd()
来源：http://bw.muxihuayi.cn

PHP:  getcwd();
来源：http://dx.szxytkj.cn

JS:   process.cwd()
来源：http://qw.521024.cn

TS:   process.cwd()
来源：http://ik.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://dt.huanxung.cn

Go:   os.Getwd()
来源：http://oc.9csxet.cn

Ruby: Dir.pwd
来源：http://ch.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wk.shxzskj.cn

[M05] 设置退出码
来源：http://qf.huanxung.cn

Py:   sys.exit(1)
来源：http://mw.jctech888.com.cn

PHP:  exit(1);
来源：http://uo.newstarts.cn

JS:   process.exit(1)
来源：http://fr.szsharing.cn

TS:   process.exit(1)
来源：http://qh.panjiajie.cn

Java: System.exit(1)
来源：http://vb.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://bs.szsharing.cn

Ruby: exit 1
来源：http://sk.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rs.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://dz.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://ve.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://co.szsharing.cn

JS:   console.error("err")
来源：http://zs.hahajie.cn

TS:   console.error("err")
来源：http://ft.shxzukj.cn

Java: System.err.println("err")
来源：http://fx.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xy.shxzskj.cn

Ruby: warn "err"
来源：http://ag.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://bm.hahajie.cn

[M07] 判断是否为主入口
来源：http://dv.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://dt.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ej.colortex.cn

JS:   require.main === module
来源：http://tq.chemitech.net.cn

TS:   require.main === module
来源：http://rp.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://qr.nicolike.cn

Go:   func main()
来源：http://vg.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bt.hahajie.cn

C#:   static void Main(string[] args)
来源：http://eg.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://sn.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://wo.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://nc.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://up.shxzukj.cn

TS:   process.platform;  process.version
来源：http://jb.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gk.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tb.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lt.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ht.huixinmuqiang.cn

================================================================================
来源：http://qc.lnxyls.cn

N. 数据结构与算法
来源：http://ac.wgjwhj.cn

================================================================================
来源：http://vi.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://pg.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pg.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vi.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ad.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://js.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hu.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://np.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ag.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mg.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://fd.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://vh.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://is.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nw.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ok.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sk.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://fi.huixinmuqiang.cn

Ruby: arr.sort
来源：http://lc.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dr.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://ng.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://br.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://yu.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nz.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xc.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sy.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ji.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ia.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xy.yuexingan06.cn

[N04] 斐波那契数列
来源：http://km.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ip.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gj.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fk.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rv.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bc.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dg.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vp.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://td.szsharing.cn

[N05] 最大公约数
来源：http://so.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://cf.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tm.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://um.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iv.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://st.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xp.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://kr.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://at.shtwfgs.cn

[N06] 判断回文字符串
来源：http://oj.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ve.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://ok.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ec.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://nw.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iz.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://tk.jctech888.com.cn

Ruby: s == s.reverse
来源：http://dm.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tv.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://hv.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fs.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yl.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qn.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ta.szsharing.cn

Java: // 手写 HashMap
来源：http://pz.9csxet.cn

Go:   // 手写 map[int]int
来源：http://lr.hahajie.cn

Ruby: // 手写 Hash
来源：http://va.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nl.szsharing.cn

[N08] 生成全排列
来源：http://qo.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://yf.521024.cn

PHP:  // 手写递归交换
来源：http://dr.nszjky.cn

JS:   // 手写回溯递归
来源：http://xm.nszjky.cn

TS:   // 手写回溯递归
来源：http://tz.asd995.cn

Java: // 手写回溯递归
来源：http://sg.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://wt.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://kt.hnjuh.cn

C#:   // 手写回溯递归
来源：http://xs.colortex.cn

[N09] 栈与队列
来源：http://kx.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rn.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tb.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jx.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ml.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vk.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://th.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tc.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wu.chemitech.net.cn

[N10] 链表节点定义
来源：http://kk.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lf.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xg.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ih.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mb.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://pf.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tb.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://td.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kt.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://hw.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eo.szsharing.cn

PHP:  // 手写递归函数
来源：http://ki.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fa.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hp.shxzukj.cn

Java: // 手写递归
来源：http://zf.huanxung.cn

Go:   // 手写递归
来源：http://cy.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://py.huanxung.cn

C#:   // 手写递归
来源：http://rm.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vt.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uz.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zr.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nh.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jr.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bj.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lz.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xy.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eq.shxzukj.cn

================================================================================
来源：http://kx.szxytkj.cn

O. 并发与异步
来源：http://gn.shxzskj.cn

================================================================================
来源：http://mo.nszjky.cn

[O01] 启动一个线程
来源：http://av.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tn.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vu.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yv.hahajie.cn

TS:   // 同 JS
来源：http://le.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://jb.newstarts.cn

Go:   go f()
来源：http://zb.huanxung.cn

Ruby: Thread.new { f }
来源：http://kg.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://iz.szsharing.cn

[O02] 使用线程池
来源：http://bw.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kv.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vo.521024.cn

JS:   // worker_threads 线程池
来源：http://qn.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://vc.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nv.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mh.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ob.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qq.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://wu.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://il.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ma.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ty.shxzskj.cn

TS:   // 同 JS
来源：http://bo.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://qj.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bu.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qi.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://wm.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://uj.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://bs.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mo.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://po.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rh.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://td.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hw.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gh.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://ug.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://gs.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://cz.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xf.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://pj.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://di.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xv.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qy.9csxet.cn

Ruby: threads.map(&:join)
来源：http://qa.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sz.bookmarksfly.cn

[O06] 使用进程池
来源：http://fc.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bf.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hp.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://uo.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://al.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://li.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://we.shxzukj.cn

Ruby: // fork 块
来源：http://ww.panjiajie.cn

C#:   Parallel.For
来源：http://ec.lnxyls.cn

================================================================================
来源：http://kk.bookmarksfly.cn

P. 常用工具函数
来源：http://kx.hahajie.cn

================================================================================
来源：http://qr.haigaiapp.cn

[P01] 生成 UUID
来源：http://yf.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://ir.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ta.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://hz.huanxung.cn

TS:   crypto.randomUUID()
来源：http://wp.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://rk.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://wm.asd995.cn

Ruby: SecureRandom.uuid
来源：http://wb.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://go.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://op.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ku.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jf.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lw.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rf.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zo.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dh.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ts.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sv.szxytkj.cn

[P03] 生成短随机字符串
来源：http://fq.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pi.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bh.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wq.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gw.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lf.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tc.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ar.hahajie.cn

[P04] 求长度
来源：http://lg.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dp.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vq.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fa.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rl.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://db.9csxet.cn

Go:   len(arr);  len(m)
来源：http://tz.nszjky.cn

Ruby: x.length;  x.size
来源：http://jz.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nm.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://nb.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cn.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hf.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oc.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ax.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kl.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yx.jctech888.com.cn

Ruby: a == b
来源：http://da.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gi.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jw.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bf.521024.cn

PHP:  if (empty($x)) {}
来源：http://sw.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kp.gzmigu.cn

TS:   if (x == null) {}
来源：http://sn.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ju.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://tc.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wf.yuexingan06.cn

C#:   if (x is null) {}
来源：http://kn.521024.cn

[P07] 防抖与节流
来源：http://ih.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mi.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://gd.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ok.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ae.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ms.panjiajie.cn


<!-- 参考信息 -->