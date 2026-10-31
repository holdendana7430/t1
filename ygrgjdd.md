代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://em.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pk.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fi.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ic.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://pk.asd995.cn

Py:   os.getcwd()
来源：http://xm.newstarts.cn

PHP:  getcwd();
来源：http://wk.521024.cn

JS:   process.cwd()
来源：http://yf.jctech888.com.cn

TS:   process.cwd()
来源：http://ad.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://be.nicolike.cn

Go:   os.Getwd()
来源：http://pt.hnjuh.cn

Ruby: Dir.pwd
来源：http://jd.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wh.newstarts.cn

[M05] 设置退出码
来源：http://jv.gzmigu.cn

Py:   sys.exit(1)
来源：http://jw.gzmigu.cn

PHP:  exit(1);
来源：http://wk.521024.cn

JS:   process.exit(1)
来源：http://vl.chemitech.net.cn

TS:   process.exit(1)
来源：http://tz.shtwfgs.cn

Java: System.exit(1)
来源：http://cl.haigaiapp.cn

Go:   os.Exit(1)
来源：http://gg.jctech888.com.cn

Ruby: exit 1
来源：http://bl.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.hnjuh.cn

[M06] 向标准错误输出
来源：http://ag.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://ru.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dv.hahajie.cn

JS:   console.error("err")
来源：http://pw.521024.cn

TS:   console.error("err")
来源：http://el.panjiajie.cn

Java: System.err.println("err")
来源：http://lp.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mk.muxihuayi.cn

Ruby: warn "err"
来源：http://eq.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://kh.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://ay.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://fg.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ha.nszjky.cn

JS:   require.main === module
来源：http://ua.panjiajie.cn

TS:   require.main === module
来源：http://ud.szxytkj.cn

Java: public static void main(String[] args)
来源：http://rq.muxihuayi.cn

Go:   func main()
来源：http://oe.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zc.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://wd.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://ca.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://ho.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://us.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ic.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://gh.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vq.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hx.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://co.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ee.shtwfgs.cn

================================================================================
来源：http://ac.hnjuh.cn

N. 数据结构与算法
来源：http://ho.haigaiapp.cn

================================================================================
来源：http://sa.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://wt.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mk.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ie.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hc.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ge.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://pk.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://th.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://re.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://rr.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://zc.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ne.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gj.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://te.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sp.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://if.colortex.cn

Ruby: arr.sort
来源：http://hg.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://db.521024.cn

[N03] 快速排序（分治示例）
来源：http://rc.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dl.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://uv.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pw.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ov.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qe.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nz.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lw.hahajie.cn

[N04] 斐波那契数列
来源：http://dg.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://as.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yy.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xx.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pc.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cg.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gp.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hk.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ii.wgjwhj.cn

[N05] 最大公约数
来源：http://vh.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://bs.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mf.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jz.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://se.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ce.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pr.hahajie.cn

Ruby: a.gcd(b)
来源：http://zq.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rb.shxzskj.cn

[N06] 判断回文字符串
来源：http://pc.panjiajie.cn

Py:   s == s[::-1]
来源：http://up.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://nc.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://fw.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://lj.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xk.nicolike.cn

Go:   // 双指针从两端比较
来源：http://sp.muxihuayi.cn

Ruby: s == s.reverse
来源：http://zm.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uy.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://xe.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://io.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://we.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dz.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://mj.newstarts.cn

Java: // 手写 HashMap
来源：http://kg.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://gf.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://iu.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xf.asd995.cn

[N08] 生成全排列
来源：http://eu.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://ii.hnjuh.cn

PHP:  // 手写递归交换
来源：http://vw.hnjuh.cn

JS:   // 手写回溯递归
来源：http://lp.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://uv.bjjhwx.cn

Java: // 手写回溯递归
来源：http://vx.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://cw.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://co.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://fo.huanxung.cn

[N09] 栈与队列
来源：http://bs.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zl.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pb.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bl.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bn.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cm.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yr.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ev.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hr.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://bj.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://er.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sq.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ut.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mt.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ha.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tw.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dq.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rs.newstarts.cn

[N11] 二叉树中序遍历
来源：http://fn.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bh.szxytkj.cn

PHP:  // 手写递归函数
来源：http://dp.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://am.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zk.nicolike.cn

Java: // 手写递归
来源：http://zk.newstarts.cn

Go:   // 手写递归
来源：http://sc.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xh.hnjuh.cn

C#:   // 手写递归
来源：http://ei.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hk.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xv.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mu.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nj.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fi.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bw.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hd.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://di.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://di.hnjuh.cn

================================================================================
来源：http://fq.huixiangedu.cn

O. 并发与异步
来源：http://lt.shxzukj.cn

================================================================================
来源：http://ce.huixiangedu.cn

[O01] 启动一个线程
来源：http://vi.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vv.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fa.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eg.yuntaijiaju.cn

TS:   // 同 JS
来源：http://fo.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://fl.haigaiapp.cn

Go:   go f()
来源：http://vl.nicolike.cn

Ruby: Thread.new { f }
来源：http://uf.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://as.shxzukj.cn

[O02] 使用线程池
来源：http://ct.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ua.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qo.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://rl.nszjky.cn

TS:   // worker_threads 线程池
来源：http://ao.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mq.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ig.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nh.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zv.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://us.nszjky.cn

Py:   with lock: shared += 1
来源：http://qz.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://zh.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dv.chemitech.net.cn

TS:   // 同 JS
来源：http://dd.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://hu.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ba.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uw.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://em.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://pe.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://yx.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sm.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://az.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pu.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ln.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bs.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ri.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://iv.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://tx.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://pp.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hv.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://hx.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://qe.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uf.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fo.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://vo.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yf.wgjwhj.cn

[O06] 使用进程池
来源：http://ui.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://go.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zz.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://tv.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://nu.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://un.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hv.jctech888.com.cn

Ruby: // fork 块
来源：http://ej.bjjhwx.cn

C#:   Parallel.For
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://pn.yuntaijiaju.cn

P. 常用工具函数
来源：http://sv.hahajie.cn

================================================================================
来源：http://nx.nszjky.cn

[P01] 生成 UUID
来源：http://vc.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://cd.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ji.colortex.cn

JS:   crypto.randomUUID()
来源：http://no.9csxet.cn

TS:   crypto.randomUUID()
来源：http://is.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://aa.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://ck.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://vx.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://vs.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://mq.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wa.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yt.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lu.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://df.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ce.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wn.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rd.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vu.nszjky.cn

[P03] 生成短随机字符串
来源：http://ij.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mn.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://en.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://be.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ri.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ct.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://no.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xi.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nx.huixiangedu.cn

[P04] 求长度
来源：http://iz.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://il.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vl.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lp.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://ia.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://zz.hnjuh.cn

Ruby: x.length;  x.size
来源：http://ti.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pi.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://hu.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mv.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mh.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ye.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ou.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bh.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://no.szxytkj.cn

Ruby: a == b
来源：http://ts.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vy.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://se.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yw.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://em.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fq.shxzukj.cn

TS:   if (x == null) {}
来源：http://ta.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mj.colortex.cn

Go:   if x == nil {}
来源：http://zh.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xy.colortex.cn

C#:   if (x is null) {}
来源：http://wk.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://gu.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jb.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://nh.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gw.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bq.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dy.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xr.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qp.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fs.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://if.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tf.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eq.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tw.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fg.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dr.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qo.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cm.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dy.shxzukj.cn

================================================================================
来源：http://bk.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pc.nszjky.cn

================================================================================
来源：http://xo.nicolike.cn

[Q01] 创建表
来源：http://dp.newstarts.cn

CREATE TABLE users (
来源：http://xx.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rl.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://fp.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://lf.lnxyls.cn


<!-- 参考信息 -->