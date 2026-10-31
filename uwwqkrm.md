代发 wailian999

Ruby: ARGV
来源：http://vy.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://ry.shtwfgs.cn

[M02] 读取环境变量
来源：http://nu.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://pc.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.shtwfgs.cn

JS:   process.env.HOME
来源：http://ka.nicolike.cn

TS:   process.env.HOME
来源：http://li.9csxet.cn

Java: System.getenv("HOME")
来源：http://at.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ts.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://zr.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://av.9csxet.cn

[M03] 执行外部命令
来源：http://xe.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fb.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nj.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xi.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xa.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ld.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://md.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wz.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://yh.gzmigu.cn

[M04] 获取当前工作目录
来源：http://ad.nszjky.cn

Py:   os.getcwd()
来源：http://md.huixiangedu.cn

PHP:  getcwd();
来源：http://uz.521024.cn

JS:   process.cwd()
来源：http://ge.szsharing.cn

TS:   process.cwd()
来源：http://mm.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ai.asd995.cn

Go:   os.Getwd()
来源：http://ir.521024.cn

Ruby: Dir.pwd
来源：http://uz.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jz.521024.cn

[M05] 设置退出码
来源：http://te.lnxyls.cn

Py:   sys.exit(1)
来源：http://rl.szsharing.cn

PHP:  exit(1);
来源：http://qp.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://qk.bjjhwx.cn

TS:   process.exit(1)
来源：http://qh.colortex.cn

Java: System.exit(1)
来源：http://lx.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://mw.asd995.cn

Ruby: exit 1
来源：http://dq.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vr.gzmigu.cn

[M06] 向标准错误输出
来源：http://bg.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://yk.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ie.chemitech.net.cn

JS:   console.error("err")
来源：http://kz.bjjhwx.cn

TS:   console.error("err")
来源：http://vi.9csxet.cn

Java: System.err.println("err")
来源：http://sf.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cc.nszjky.cn

Ruby: warn "err"
来源：http://bl.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://jy.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://mc.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://br.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zu.huanxung.cn

JS:   require.main === module
来源：http://qn.bookmarksfly.cn

TS:   require.main === module
来源：http://vl.nszjky.cn

Java: public static void main(String[] args)
来源：http://jp.9csxet.cn

Go:   func main()
来源：http://xe.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ee.asd995.cn

C#:   static void Main(string[] args)
来源：http://lz.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://mu.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://cu.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://pb.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://hw.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://nb.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rf.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ty.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zm.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://su.bjjhwx.cn

================================================================================
来源：http://lr.521024.cn

N. 数据结构与算法
来源：http://gj.szxytkj.cn

================================================================================
来源：http://fu.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://hk.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ps.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vt.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vx.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nx.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ul.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://qb.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ql.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://rz.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://zu.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yg.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jx.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rm.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ff.asd995.cn

Go:   slices.Sort(arr)
来源：http://ag.gzmigu.cn

Ruby: arr.sort
来源：http://ng.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jy.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://pa.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ax.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://nc.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pt.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ik.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pu.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yw.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gs.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://go.shxzskj.cn

[N04] 斐波那契数列
来源：http://yu.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xs.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mb.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cx.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nb.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dk.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sc.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pe.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iu.9csxet.cn

[N05] 最大公约数
来源：http://wr.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://zn.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ym.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://at.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oq.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tw.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gl.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://ap.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ab.chemitech.net.cn

[N06] 判断回文字符串
来源：http://gz.szxytkj.cn

Py:   s == s[::-1]
来源：http://hm.9csxet.cn

PHP:  $s === strrev($s);
来源：http://pc.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://zn.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://nm.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nt.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://fa.szsharing.cn

Ruby: s == s.reverse
来源：http://zw.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nf.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://pr.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://no.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qt.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xj.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://bb.shtwfgs.cn

Java: // 手写 HashMap
来源：http://cn.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ck.szxytkj.cn

Ruby: // 手写 Hash
来源：http://si.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lc.gzmigu.cn

[N08] 生成全排列
来源：http://ch.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://pj.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://bd.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://bo.hnjuh.cn

TS:   // 手写回溯递归
来源：http://km.newstarts.cn

Java: // 手写回溯递归
来源：http://uv.szsharing.cn

Go:   // 手写回溯递归
来源：http://ni.colortex.cn

Ruby: arr.permutation.to_a
来源：http://tx.panjiajie.cn

C#:   // 手写回溯递归
来源：http://rs.hnjuh.cn

[N09] 栈与队列
来源：http://op.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wx.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bm.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://es.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ws.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jh.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jr.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vd.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ge.9csxet.cn

[N10] 链表节点定义
来源：http://mh.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fp.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rc.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rg.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xk.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://tj.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gk.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://le.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vh.nszjky.cn

[N11] 二叉树中序遍历
来源：http://pc.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://am.panjiajie.cn

PHP:  // 手写递归函数
来源：http://kd.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cu.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tv.huixinmuqiang.cn

Java: // 手写递归
来源：http://ug.wgjwhj.cn

Go:   // 手写递归
来源：http://tm.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wi.9csxet.cn

C#:   // 手写递归
来源：http://ph.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jp.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rf.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ys.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pr.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mj.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hf.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gv.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gb.szsharing.cn

================================================================================
来源：http://ss.nszjky.cn

O. 并发与异步
来源：http://fk.gzmigu.cn

================================================================================
来源：http://mt.hahajie.cn

[O01] 启动一个线程
来源：http://gy.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dm.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ey.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ur.hahajie.cn

TS:   // 同 JS
来源：http://af.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://dw.szxytkj.cn

Go:   go f()
来源：http://ho.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://ik.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://pq.newstarts.cn

[O02] 使用线程池
来源：http://ua.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ya.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wf.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://uq.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://mh.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eq.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pe.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rs.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fy.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://au.lnxyls.cn

Py:   with lock: shared += 1
来源：http://gz.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://vu.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cs.haigaiapp.cn

TS:   // 同 JS
来源：http://ed.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://nc.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tx.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://et.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://db.hahajie.cn

[O04] 定义异步函数并等待
来源：http://gq.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://ex.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kt.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://vc.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oh.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gc.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kw.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rq.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://rs.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://vs.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://qr.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aa.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://xh.521024.cn

TS:   await Promise.all(tasks)
来源：http://tn.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oe.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ga.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://eg.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ti.lnxyls.cn

[O06] 使用进程池
来源：http://ei.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xn.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dm.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://wp.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://pe.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mz.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://in.hahajie.cn

Ruby: // fork 块
来源：http://uz.yuntaijiaju.cn

C#:   Parallel.For
来源：http://iy.hnjuh.cn

================================================================================
来源：http://vp.jctech888.com.cn

P. 常用工具函数
来源：http://hb.nicolike.cn

================================================================================
来源：http://wp.9csxet.cn

[P01] 生成 UUID
来源：http://gl.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://ew.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yi.szsharing.cn

JS:   crypto.randomUUID()
来源：http://tl.huanxung.cn

TS:   crypto.randomUUID()
来源：http://hb.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://qn.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://dy.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://ug.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://kh.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://xe.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wj.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sh.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nf.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xv.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fz.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dg.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ok.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://do.colortex.cn

[P03] 生成短随机字符串
来源：http://jn.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yg.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://km.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ih.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://js.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zh.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://on.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://un.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bq.asd995.cn

[P04] 求长度
来源：http://ay.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rl.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lv.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rq.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uf.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://nv.9csxet.cn

Go:   len(arr);  len(m)
来源：http://ds.9csxet.cn

Ruby: x.length;  x.size
来源：http://er.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mv.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://ty.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sn.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cl.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://au.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://js.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zj.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://te.wgjwhj.cn

Ruby: a == b
来源：http://qa.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tk.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vw.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nd.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://sw.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tz.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://es.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cy.szxytkj.cn

Go:   if x == nil {}
来源：http://yv.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ts.9csxet.cn

C#:   if (x is null) {}
来源：http://jk.shtwfgs.cn

[P07] 防抖与节流
来源：http://ng.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ai.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://cm.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://te.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ci.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mw.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lc.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uc.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gg.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://su.gzmigu.cn


<!-- 参考信息 -->