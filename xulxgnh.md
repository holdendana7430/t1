代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yo.shxzukj.cn

JS:   process.env.HOME
来源：http://ki.nicolike.cn

TS:   process.env.HOME
来源：http://ch.521024.cn

Java: System.getenv("HOME")
来源：http://hs.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fd.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://si.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vy.asd995.cn

[M03] 执行外部命令
来源：http://fu.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rh.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yb.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ta.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zy.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ow.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vm.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kj.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://zr.521024.cn

[M04] 获取当前工作目录
来源：http://mq.9csxet.cn

Py:   os.getcwd()
来源：http://to.gzmigu.cn

PHP:  getcwd();
来源：http://ab.wgjwhj.cn

JS:   process.cwd()
来源：http://hs.hahajie.cn

TS:   process.cwd()
来源：http://hj.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://pb.9csxet.cn

Go:   os.Getwd()
来源：http://fb.muxihuayi.cn

Ruby: Dir.pwd
来源：http://sx.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kn.nicolike.cn

[M05] 设置退出码
来源：http://yf.shtwfgs.cn

Py:   sys.exit(1)
来源：http://bv.muxihuayi.cn

PHP:  exit(1);
来源：http://bj.huanxung.cn

JS:   process.exit(1)
来源：http://vr.huixiangedu.cn

TS:   process.exit(1)
来源：http://gu.jianghongdianzi.cn

Java: System.exit(1)
来源：http://pp.jctech888.com.cn

Go:   os.Exit(1)
来源：http://dd.yuexingan06.cn

Ruby: exit 1
来源：http://ul.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xj.lnxyls.cn

[M06] 向标准错误输出
来源：http://av.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ku.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ip.yuntaijiaju.cn

JS:   console.error("err")
来源：http://om.bookmarksfly.cn

TS:   console.error("err")
来源：http://wi.szsharing.cn

Java: System.err.println("err")
来源：http://oi.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fo.wgjwhj.cn

Ruby: warn "err"
来源：http://kc.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://wc.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://ou.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://jt.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://at.hahajie.cn

JS:   require.main === module
来源：http://vg.hnjuh.cn

TS:   require.main === module
来源：http://ku.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ow.huixinmuqiang.cn

Go:   func main()
来源：http://uz.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ua.9csxet.cn

C#:   static void Main(string[] args)
来源：http://bx.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://lo.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ku.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://zg.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://fn.szxytkj.cn

TS:   process.platform;  process.version
来源：http://fo.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pv.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wh.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zb.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bc.hahajie.cn

================================================================================
来源：http://fz.muxihuayi.cn

N. 数据结构与算法
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://ou.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://aj.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xu.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://js.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ww.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bh.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ef.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mv.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pr.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://df.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://wb.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bp.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ei.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yd.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ze.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://sx.bookmarksfly.cn

Ruby: arr.sort
来源：http://om.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zn.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://wa.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xa.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://jw.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xk.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cg.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jq.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ip.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hc.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xm.newstarts.cn

[N04] 斐波那契数列
来源：http://nm.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://an.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bk.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cw.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wk.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rp.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tz.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xy.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nu.colortex.cn

[N05] 最大公约数
来源：http://oc.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://kq.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rr.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hn.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jp.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lv.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zw.shxzukj.cn

Ruby: a.gcd(b)
来源：http://kr.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ke.9csxet.cn

[N06] 判断回文字符串
来源：http://nr.jctech888.com.cn

Py:   s == s[::-1]
来源：http://pn.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://xk.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://sa.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://ms.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vz.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ax.newstarts.cn

Ruby: s == s.reverse
来源：http://fe.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yd.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://wf.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pf.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://on.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uy.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://wr.nicolike.cn

Java: // 手写 HashMap
来源：http://cl.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ns.nicolike.cn

Ruby: // 手写 Hash
来源：http://hv.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hw.bookmarksfly.cn

[N08] 生成全排列
来源：http://ru.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://hp.nszjky.cn

PHP:  // 手写递归交换
来源：http://tf.newstarts.cn

JS:   // 手写回溯递归
来源：http://pj.huanxung.cn

TS:   // 手写回溯递归
来源：http://ts.shxzukj.cn

Java: // 手写回溯递归
来源：http://ws.nszjky.cn

Go:   // 手写回溯递归
来源：http://fl.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://vj.panjiajie.cn

C#:   // 手写回溯递归
来源：http://bi.yuexingan06.cn

[N09] 栈与队列
来源：http://ah.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zz.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://re.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vc.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gg.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nb.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dn.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lu.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bf.bookmarksfly.cn

[N10] 链表节点定义
来源：http://pj.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mr.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bk.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yd.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ca.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://pq.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rg.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rw.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ll.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://to.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gp.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://tk.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ut.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gi.huanxung.cn

Java: // 手写递归
来源：http://tk.bjjhwx.cn

Go:   // 手写递归
来源：http://ff.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fg.bookmarksfly.cn

C#:   // 手写递归
来源：http://bx.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lp.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sq.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://he.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fv.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://am.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tq.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://af.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ec.huixiangedu.cn

================================================================================
来源：http://qe.gzmigu.cn

O. 并发与异步
来源：http://kq.yuexingan06.cn

================================================================================
来源：http://mg.panjiajie.cn

[O01] 启动一个线程
来源：http://tf.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cx.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dj.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fu.hahajie.cn

TS:   // 同 JS
来源：http://ng.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://zz.shtwfgs.cn

Go:   go f()
来源：http://ws.hnjuh.cn

Ruby: Thread.new { f }
来源：http://wr.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://xx.lnxyls.cn

[O02] 使用线程池
来源：http://vj.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hs.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lx.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://jz.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://lc.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ek.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://do.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vy.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ez.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://xc.hnjuh.cn

Py:   with lock: shared += 1
来源：http://pk.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://gf.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zk.nszjky.cn

TS:   // 同 JS
来源：http://oh.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://mf.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hq.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://sz.newstarts.cn

[O04] 定义异步函数并等待
来源：http://cv.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://pi.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nc.newstarts.cn

JS:   async function f() { await g(); }
来源：http://gc.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gq.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sx.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xo.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ij.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://mt.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://mc.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://dx.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ko.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://he.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://ia.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bo.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lb.szsharing.cn

Ruby: threads.map(&:join)
来源：http://nv.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vj.huanxung.cn

[O06] 使用进程池
来源：http://ch.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yk.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cl.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://ot.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://fj.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bx.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ey.9csxet.cn

Ruby: // fork 块
来源：http://ls.panjiajie.cn

C#:   Parallel.For
来源：http://hp.szxytkj.cn

================================================================================
来源：http://dk.jctech888.com.cn

P. 常用工具函数
来源：http://za.bjjhwx.cn

================================================================================
来源：http://dt.gzmigu.cn

[P01] 生成 UUID
来源：http://cv.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://ty.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ui.521024.cn

JS:   crypto.randomUUID()
来源：http://bn.asd995.cn

TS:   crypto.randomUUID()
来源：http://jz.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://sj.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://av.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://km.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://qy.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://zy.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://za.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zu.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jk.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pe.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ak.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zh.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nw.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ff.hahajie.cn

[P03] 生成短随机字符串
来源：http://pi.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hp.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ha.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zo.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bh.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lh.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fo.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iq.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://go.jianghongdianzi.cn

[P04] 求长度
来源：http://pe.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ur.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://su.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lz.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://uu.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://ul.gzmigu.cn

Ruby: x.length;  x.size
来源：http://od.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xp.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://tc.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gi.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://po.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ay.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pt.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://km.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oi.chemitech.net.cn

Ruby: a == b
来源：http://xj.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wb.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nd.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zt.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://do.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bt.huanxung.cn

TS:   if (x == null) {}
来源：http://xl.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sw.szsharing.cn

Go:   if x == nil {}
来源：http://pw.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tx.521024.cn

C#:   if (x is null) {}
来源：http://au.huanxung.cn

[P07] 防抖与节流
来源：http://pe.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mv.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://do.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kr.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ny.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sw.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vd.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sj.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nk.521024.cn

[P08] 处理浮点精度问题
来源：http://iw.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xh.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ey.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kl.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xk.szsharing.cn


<!-- 参考信息 -->