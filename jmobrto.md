代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ws.huanxung.cn

Ruby: ENV["HOME"]
来源：http://nq.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ks.lnxyls.cn

[M03] 执行外部命令
来源：http://zn.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hj.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jf.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ek.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rg.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xt.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gv.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://eh.bjjhwx.cn

Py:   os.getcwd()
来源：http://ex.jianghongdianzi.cn

PHP:  getcwd();
来源：http://tx.bookmarksfly.cn

JS:   process.cwd()
来源：http://wq.huixiangedu.cn

TS:   process.cwd()
来源：http://fz.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://qm.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://us.colortex.cn

Ruby: Dir.pwd
来源：http://ca.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xu.hnjuh.cn

[M05] 设置退出码
来源：http://qh.gzmigu.cn

Py:   sys.exit(1)
来源：http://dp.hahajie.cn

PHP:  exit(1);
来源：http://ak.bjjhwx.cn

JS:   process.exit(1)
来源：http://or.huixiangedu.cn

TS:   process.exit(1)
来源：http://ab.huanxung.cn

Java: System.exit(1)
来源：http://jw.shxzukj.cn

Go:   os.Exit(1)
来源：http://wf.muxihuayi.cn

Ruby: exit 1
来源：http://lc.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lt.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://on.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ja.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tl.bookmarksfly.cn

JS:   console.error("err")
来源：http://gk.hahajie.cn

TS:   console.error("err")
来源：http://jl.hnjuh.cn

Java: System.err.println("err")
来源：http://pp.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vp.jianghongdianzi.cn

Ruby: warn "err"
来源：http://se.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://fw.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ku.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://ii.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dp.wgjwhj.cn

JS:   require.main === module
来源：http://ad.9csxet.cn

TS:   require.main === module
来源：http://lp.gzmigu.cn

Java: public static void main(String[] args)
来源：http://uj.jctech888.com.cn

Go:   func main()
来源：http://go.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vm.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://rf.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://ic.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://lw.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://bo.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://hq.hahajie.cn

TS:   process.platform;  process.version
来源：http://kg.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kx.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hl.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lf.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rd.szsharing.cn

================================================================================
来源：http://zd.muxihuayi.cn

N. 数据结构与算法
来源：http://ex.yuexingan06.cn

================================================================================
来源：http://tp.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://gu.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dr.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mc.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hk.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://th.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fg.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://ms.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ya.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bl.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qe.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://qr.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gz.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hp.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uo.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zb.szsharing.cn

Go:   slices.Sort(arr)
来源：http://wb.colortex.cn

Ruby: arr.sort
来源：http://eo.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ck.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://vf.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qt.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://vh.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sy.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dl.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://az.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zi.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nn.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ff.nszjky.cn

[N04] 斐波那契数列
来源：http://az.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ck.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://we.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://km.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bk.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://az.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mg.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ma.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tq.lnxyls.cn

[N05] 最大公约数
来源：http://ks.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://ex.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vs.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yf.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ea.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mk.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ib.nszjky.cn

Ruby: a.gcd(b)
来源：http://sj.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xb.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://wy.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://jl.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://rj.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ch.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://ui.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fx.521024.cn

Go:   // 双指针从两端比较
来源：http://nr.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://qc.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ux.521024.cn

[N07] 两数之和（返回下标）
来源：http://pz.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://el.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iw.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fo.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://pm.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://xy.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://ig.huanxung.cn

Ruby: // 手写 Hash
来源：http://xb.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tw.nszjky.cn

[N08] 生成全排列
来源：http://fh.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ci.szsharing.cn

PHP:  // 手写递归交换
来源：http://su.hnjuh.cn

JS:   // 手写回溯递归
来源：http://fq.asd995.cn

TS:   // 手写回溯递归
来源：http://ws.haigaiapp.cn

Java: // 手写回溯递归
来源：http://bu.szxytkj.cn

Go:   // 手写回溯递归
来源：http://wb.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://st.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://ws.bjjhwx.cn

[N09] 栈与队列
来源：http://uy.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pq.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rj.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gv.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://br.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ut.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sj.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ve.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fj.nszjky.cn

[N10] 链表节点定义
来源：http://yv.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://td.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rm.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mf.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ls.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://ms.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zs.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jc.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rm.huanxung.cn

[N11] 二叉树中序遍历
来源：http://io.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jl.asd995.cn

PHP:  // 手写递归函数
来源：http://ft.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zx.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ez.wgjwhj.cn

Java: // 手写递归
来源：http://oz.huixiangedu.cn

Go:   // 手写递归
来源：http://bb.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zq.hahajie.cn

C#:   // 手写递归
来源：http://np.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tm.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cx.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zy.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pp.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sz.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gj.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bs.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dl.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dg.lnxyls.cn

================================================================================
来源：http://ri.521024.cn

O. 并发与异步
来源：http://pq.wgjwhj.cn

================================================================================
来源：http://uz.huanxung.cn

[O01] 启动一个线程
来源：http://ky.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nw.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ut.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fu.hahajie.cn

TS:   // 同 JS
来源：http://qt.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://vw.hnjuh.cn

Go:   go f()
来源：http://ao.asd995.cn

Ruby: Thread.new { f }
来源：http://dt.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://zu.hnjuh.cn

[O02] 使用线程池
来源：http://yl.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lk.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vv.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ap.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://ao.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yx.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qf.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cg.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://it.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://yy.panjiajie.cn

Py:   with lock: shared += 1
来源：http://ps.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://dj.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vn.asd995.cn

TS:   // 同 JS
来源：http://kc.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://bf.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ym.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hd.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://rt.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://kh.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://qe.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xv.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://fn.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wo.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://re.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dr.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mr.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://yg.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://oz.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://rq.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fd.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ad.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://ji.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fb.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vl.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://qp.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yx.hnjuh.cn

[O06] 使用进程池
来源：http://bg.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lu.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yz.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://lb.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://pu.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dv.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xm.szsharing.cn

Ruby: // fork 块
来源：http://dv.jianghongdianzi.cn

C#:   Parallel.For
来源：http://fq.9csxet.cn

================================================================================
来源：http://wd.panjiajie.cn

P. 常用工具函数
来源：http://yu.huanxung.cn

================================================================================
来源：http://lr.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://qm.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://qq.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ew.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://co.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://xq.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://pv.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://qs.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://ah.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://jn.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://dm.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zo.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fr.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zg.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sy.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hc.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sx.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bv.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ns.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://we.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zy.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://io.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pg.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qs.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fl.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kn.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ir.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://th.9csxet.cn

[P04] 求长度
来源：http://uy.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xw.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eu.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dq.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://or.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://it.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://af.gzmigu.cn

Ruby: x.length;  x.size
来源：http://ru.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://th.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ix.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dv.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://si.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pk.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bd.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wf.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yt.panjiajie.cn

Ruby: a == b
来源：http://ov.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qm.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cc.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zj.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://gi.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uv.colortex.cn

TS:   if (x == null) {}
来源：http://ul.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rj.shxzskj.cn

Go:   if x == nil {}
来源：http://we.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sh.gzmigu.cn

C#:   if (x is null) {}
来源：http://ko.bookmarksfly.cn

[P07] 防抖与节流
来源：http://vr.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://et.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ac.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ee.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vh.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cr.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gr.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zr.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qc.521024.cn

[P08] 处理浮点精度问题
来源：http://vo.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bh.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ey.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rt.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tv.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://je.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mm.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ib.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tr.gzmigu.cn


<!-- 参考信息 -->