代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yr.szsharing.cn

Ruby: ENV["HOME"]
来源：http://fi.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hy.colortex.cn

[M03] 执行外部命令
来源：http://ni.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ts.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bg.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mo.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ka.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://so.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yc.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lv.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://hn.colortex.cn

[M04] 获取当前工作目录
来源：http://um.521024.cn

Py:   os.getcwd()
来源：http://cu.asd995.cn

PHP:  getcwd();
来源：http://ci.hahajie.cn

JS:   process.cwd()
来源：http://je.shtwfgs.cn

TS:   process.cwd()
来源：http://ts.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://se.huixiangedu.cn

Go:   os.Getwd()
来源：http://th.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://fo.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ab.jianghongdianzi.cn

[M05] 设置退出码
来源：http://on.chemitech.net.cn

Py:   sys.exit(1)
来源：http://nv.szsharing.cn

PHP:  exit(1);
来源：http://hk.huixiangedu.cn

JS:   process.exit(1)
来源：http://bl.521024.cn

TS:   process.exit(1)
来源：http://ke.colortex.cn

Java: System.exit(1)
来源：http://zp.panjiajie.cn

Go:   os.Exit(1)
来源：http://pi.yuexingan06.cn

Ruby: exit 1
来源：http://kc.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uz.chemitech.net.cn

[M06] 向标准错误输出
来源：http://dz.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://aa.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xn.gzmigu.cn

JS:   console.error("err")
来源：http://nm.lnxyls.cn

TS:   console.error("err")
来源：http://mk.521024.cn

Java: System.err.println("err")
来源：http://tx.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bn.hnjuh.cn

Ruby: warn "err"
来源：http://kg.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ad.szsharing.cn

[M07] 判断是否为主入口
来源：http://ir.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://qp.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kd.panjiajie.cn

JS:   require.main === module
来源：http://xa.gzmigu.cn

TS:   require.main === module
来源：http://ib.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://vy.lnxyls.cn

Go:   func main()
来源：http://in.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ay.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://sc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://tb.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://yt.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://zs.asd995.cn

JS:   process.platform;  process.version
来源：http://rd.colortex.cn

TS:   process.platform;  process.version
来源：http://rw.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ef.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kq.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lf.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.nszjky.cn

================================================================================
来源：http://oe.bjjhwx.cn

N. 数据结构与算法
来源：http://uv.muxihuayi.cn

================================================================================
来源：http://pg.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://cp.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://np.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ly.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sr.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ne.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://ja.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://de.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pi.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://yt.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zp.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rh.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zw.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zr.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bi.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://sh.szsharing.cn

Ruby: arr.sort
来源：http://ji.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zw.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://ep.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kx.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://gl.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dq.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bs.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xc.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kw.bjjhwx.cn

[N04] 斐波那契数列
来源：http://fm.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tb.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sg.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uo.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yi.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pd.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uy.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ua.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kz.nicolike.cn

[N05] 最大公约数
来源：http://rm.nszjky.cn

Py:   math.gcd(a, b)
来源：http://hj.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gy.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cq.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vf.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ce.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cl.szsharing.cn

Ruby: a.gcd(b)
来源：http://wn.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://od.shxzukj.cn

[N06] 判断回文字符串
来源：http://db.shxzukj.cn

Py:   s == s[::-1]
来源：http://ad.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://jb.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://gb.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://ju.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gj.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://jp.9csxet.cn

Ruby: s == s.reverse
来源：http://ji.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uu.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://al.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hu.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sg.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ny.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://xf.szxytkj.cn

Java: // 手写 HashMap
来源：http://gb.nicolike.cn

Go:   // 手写 map[int]int
来源：http://wc.shxzukj.cn

Ruby: // 手写 Hash
来源：http://xh.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gn.panjiajie.cn

[N08] 生成全排列
来源：http://ad.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://eg.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://cy.colortex.cn

JS:   // 手写回溯递归
来源：http://ma.szsharing.cn

TS:   // 手写回溯递归
来源：http://rn.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://mm.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://mp.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://jr.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://ro.chemitech.net.cn

[N09] 栈与队列
来源：http://vh.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ud.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jj.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mz.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jz.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gm.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://va.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ow.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wz.shxzukj.cn

[N10] 链表节点定义
来源：http://wk.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tl.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uz.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bz.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mf.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://dy.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dx.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ku.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pq.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://oq.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rt.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://xx.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ns.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nj.jctech888.com.cn

Java: // 手写递归
来源：http://xo.wgjwhj.cn

Go:   // 手写递归
来源：http://sh.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hr.huanxung.cn

C#:   // 手写递归
来源：http://sc.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tt.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tf.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ss.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vr.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jl.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kf.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ir.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ud.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wt.9csxet.cn

================================================================================
来源：http://cn.asd995.cn

O. 并发与异步
来源：http://tf.bjjhwx.cn

================================================================================
来源：http://fp.colortex.cn

[O01] 启动一个线程
来源：http://xb.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jt.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cj.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wc.chemitech.net.cn

TS:   // 同 JS
来源：http://qb.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://kx.haigaiapp.cn

Go:   go f()
来源：http://bs.nszjky.cn

Ruby: Thread.new { f }
来源：http://qc.521024.cn

C#:   Task.Run(() => F());
来源：http://cb.shtwfgs.cn

[O02] 使用线程池
来源：http://bg.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qc.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pv.szsharing.cn

JS:   // worker_threads 线程池
来源：http://jn.nicolike.cn

TS:   // worker_threads 线程池
来源：http://xc.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uy.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dt.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fz.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qn.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://we.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://bg.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://pr.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tm.huanxung.cn

TS:   // 同 JS
来源：http://ac.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://zb.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://du.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lq.521024.cn

C#:   lock (gate) { shared++; }
来源：http://rt.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://em.colortex.cn

Py:   async def f():⏎    await g()
来源：http://oo.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ir.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://xw.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vg.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ar.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xx.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aa.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://kx.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ef.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://ay.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jx.521024.cn

JS:   await Promise.all(tasks)
来源：http://ov.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://up.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gc.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nh.nicolike.cn

Ruby: threads.map(&:join)
来源：http://go.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fz.colortex.cn

[O06] 使用进程池
来源：http://lb.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dk.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gx.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://lj.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://vt.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zy.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sl.muxihuayi.cn

Ruby: // fork 块
来源：http://tm.szsharing.cn

C#:   Parallel.For
来源：http://us.huixiangedu.cn

================================================================================
来源：http://vf.lnxyls.cn

P. 常用工具函数
来源：http://ju.wgjwhj.cn

================================================================================
来源：http://ty.hnjuh.cn

[P01] 生成 UUID
来源：http://tk.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://ba.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fw.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://te.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://aa.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://vb.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://qw.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://np.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://hi.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://kg.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xh.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zl.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pi.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kt.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yn.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ic.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ju.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://is.asd995.cn

[P03] 生成短随机字符串
来源：http://xw.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yd.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ob.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://il.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qb.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://go.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wx.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bj.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://po.yuntaijiaju.cn

[P04] 求长度
来源：http://cd.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tx.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pg.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hd.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lh.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://xu.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://ia.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://wr.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ls.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://hh.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://la.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xc.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tr.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wb.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ws.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ef.9csxet.cn

Ruby: a == b
来源：http://xn.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ho.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sp.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ta.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ly.jctech888.com.cn

TS:   if (x == null) {}
来源：http://cf.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bc.lnxyls.cn

Go:   if x == nil {}
来源：http://hz.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fu.521024.cn

C#:   if (x is null) {}
来源：http://en.huixiangedu.cn

[P07] 防抖与节流
来源：http://fz.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rk.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ct.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ms.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xg.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://la.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lj.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rm.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wu.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://mx.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kz.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kz.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bj.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wm.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gv.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mp.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jj.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://is.wgjwhj.cn


<!-- 参考信息 -->