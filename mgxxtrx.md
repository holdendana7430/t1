代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ue.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kw.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qo.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://kw.hahajie.cn

[M04] 获取当前工作目录
来源：http://lh.nicolike.cn

Py:   os.getcwd()
来源：http://wz.wgjwhj.cn

PHP:  getcwd();
来源：http://gs.colortex.cn

JS:   process.cwd()
来源：http://xx.lnxyls.cn

TS:   process.cwd()
来源：http://lw.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bj.newstarts.cn

Go:   os.Getwd()
来源：http://dg.lnxyls.cn

Ruby: Dir.pwd
来源：http://jc.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fe.hahajie.cn

[M05] 设置退出码
来源：http://nl.huixiangedu.cn

Py:   sys.exit(1)
来源：http://oq.hahajie.cn

PHP:  exit(1);
来源：http://sm.panjiajie.cn

JS:   process.exit(1)
来源：http://uk.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ir.shtwfgs.cn

Java: System.exit(1)
来源：http://ay.shxzskj.cn

Go:   os.Exit(1)
来源：http://ch.nicolike.cn

Ruby: exit 1
来源：http://lx.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vp.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://lx.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://kw.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vq.szxytkj.cn

JS:   console.error("err")
来源：http://qi.chemitech.net.cn

TS:   console.error("err")
来源：http://kh.huanxung.cn

Java: System.err.println("err")
来源：http://vs.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vi.shxzskj.cn

Ruby: warn "err"
来源：http://mk.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ca.lnxyls.cn

[M07] 判断是否为主入口
来源：http://ts.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://fm.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tu.lnxyls.cn

JS:   require.main === module
来源：http://so.bjjhwx.cn

TS:   require.main === module
来源：http://kf.lnxyls.cn

Java: public static void main(String[] args)
来源：http://mv.jctech888.com.cn

Go:   func main()
来源：http://as.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dx.colortex.cn

C#:   static void Main(string[] args)
来源：http://ni.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://yq.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://zm.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://og.gzmigu.cn

JS:   process.platform;  process.version
来源：http://gj.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://ko.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bo.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mn.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sk.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wa.nszjky.cn

================================================================================
来源：http://sa.shxzskj.cn

N. 数据结构与算法
来源：http://rg.szxytkj.cn

================================================================================
来源：http://ty.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://un.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mp.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://do.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://od.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zx.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ra.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://kh.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mt.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xr.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://iv.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://cc.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ld.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tz.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rt.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ie.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://da.jianghongdianzi.cn

Ruby: arr.sort
来源：http://dz.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gy.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://vc.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sx.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://zz.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nu.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yv.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://em.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nz.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hg.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vg.muxihuayi.cn

[N04] 斐波那契数列
来源：http://ba.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uf.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://do.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iw.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nk.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bs.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gg.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://la.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eg.hnjuh.cn

[N05] 最大公约数
来源：http://lv.asd995.cn

Py:   math.gcd(a, b)
来源：http://za.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zu.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wx.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ql.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wh.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xu.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://gd.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ew.yuexingan06.cn

[N06] 判断回文字符串
来源：http://he.jctech888.com.cn

Py:   s == s[::-1]
来源：http://ml.colortex.cn

PHP:  $s === strrev($s);
来源：http://pq.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://tp.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://fn.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sq.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ry.colortex.cn

Ruby: s == s.reverse
来源：http://ee.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nf.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://vr.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ia.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nx.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kt.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ls.nszjky.cn

Java: // 手写 HashMap
来源：http://xp.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://wv.newstarts.cn

Ruby: // 手写 Hash
来源：http://ke.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bp.haigaiapp.cn

[N08] 生成全排列
来源：http://xv.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://kn.newstarts.cn

PHP:  // 手写递归交换
来源：http://bq.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://ac.gzmigu.cn

TS:   // 手写回溯递归
来源：http://cc.521024.cn

Java: // 手写回溯递归
来源：http://so.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://hp.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://db.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://kz.521024.cn

[N09] 栈与队列
来源：http://xu.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bi.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fx.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lh.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qt.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pj.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yk.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xm.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vy.shtwfgs.cn

[N10] 链表节点定义
来源：http://yg.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zp.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gc.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hn.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://la.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://iw.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wg.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://va.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nu.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://bd.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hv.szxytkj.cn

PHP:  // 手写递归函数
来源：http://eb.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yg.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tq.gzmigu.cn

Java: // 手写递归
来源：http://ov.9csxet.cn

Go:   // 手写递归
来源：http://ae.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ex.shxzukj.cn

C#:   // 手写递归
来源：http://dk.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sp.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ah.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uz.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yg.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xc.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://th.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dn.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lh.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://db.gzmigu.cn

================================================================================
来源：http://ai.nicolike.cn

O. 并发与异步
来源：http://mq.jctech888.com.cn

================================================================================
来源：http://ff.szxytkj.cn

[O01] 启动一个线程
来源：http://ai.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ev.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gr.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ue.chemitech.net.cn

TS:   // 同 JS
来源：http://xj.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://dc.shxzskj.cn

Go:   go f()
来源：http://rn.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://mz.nszjky.cn

C#:   Task.Run(() => F());
来源：http://nr.bookmarksfly.cn

[O02] 使用线程池
来源：http://jl.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sl.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ro.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ks.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://yf.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ci.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ow.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hq.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wp.newstarts.cn

[O03] 加锁保护共享数据
来源：http://tr.szxytkj.cn

Py:   with lock: shared += 1
来源：http://ea.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://bm.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iu.hnjuh.cn

TS:   // 同 JS
来源：http://kk.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://my.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fo.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fi.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://gd.asd995.cn

[O04] 定义异步函数并等待
来源：http://jw.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ea.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gm.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://nw.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lo.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gm.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zb.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wz.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://qh.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://ee.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ic.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ou.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://aa.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://wg.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qh.asd995.cn

Ruby: threads.map(&:join)
来源：http://tr.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sn.asd995.cn

[O06] 使用进程池
来源：http://ze.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tv.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://di.colortex.cn

JS:   // child_process / cluster 模块
来源：http://bc.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://rl.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gn.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.bookmarksfly.cn

Ruby: // fork 块
来源：http://nx.muxihuayi.cn

C#:   Parallel.For
来源：http://ki.shtwfgs.cn

================================================================================
来源：http://wp.asd995.cn

P. 常用工具函数
来源：http://vv.shxzskj.cn

================================================================================
来源：http://mq.haigaiapp.cn

[P01] 生成 UUID
来源：http://vu.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://uy.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hs.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://up.newstarts.cn

TS:   crypto.randomUUID()
来源：http://fy.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://kp.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://fe.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://le.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://yv.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://jy.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kj.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oz.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ku.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kj.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tb.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://br.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oj.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kg.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://rf.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qe.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yu.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ma.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://na.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yg.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://td.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pb.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lt.nicolike.cn

[P04] 求长度
来源：http://aq.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kj.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://px.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fo.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bi.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://ge.asd995.cn

Go:   len(arr);  len(m)
来源：http://ul.hahajie.cn

Ruby: x.length;  x.size
来源：http://gn.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kt.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://zl.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://um.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sd.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sl.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ep.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://di.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mg.huixiangedu.cn

Ruby: a == b
来源：http://zm.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nc.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cb.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ch.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://gg.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pq.panjiajie.cn

TS:   if (x == null) {}
来源：http://go.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fj.jctech888.com.cn

Go:   if x == nil {}
来源：http://wq.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ob.9csxet.cn

C#:   if (x is null) {}
来源：http://kt.gzmigu.cn

[P07] 防抖与节流
来源：http://yn.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xe.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://vw.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://js.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hn.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zm.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xn.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fm.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tu.nicolike.cn

[P08] 处理浮点精度问题
来源：http://qk.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kt.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lg.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lj.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pg.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ql.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://si.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jf.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hy.bjjhwx.cn

================================================================================
来源：http://gb.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ew.haigaiapp.cn

================================================================================
来源：http://cw.muxihuayi.cn

[Q01] 创建表
来源：http://eo.huixiangedu.cn

CREATE TABLE users (
来源：http://dz.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jt.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://mh.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://pp.yuntaijiaju.cn


<!-- 参考信息 -->