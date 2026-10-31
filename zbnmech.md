代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uv.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kb.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xv.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ok.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://zd.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://bq.huanxung.cn

PHP:  getcwd();
来源：http://yk.newstarts.cn

JS:   process.cwd()
来源：http://va.hahajie.cn

TS:   process.cwd()
来源：http://eo.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kz.lnxyls.cn

Go:   os.Getwd()
来源：http://hb.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://gt.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ut.bookmarksfly.cn

[M05] 设置退出码
来源：http://bh.shtwfgs.cn

Py:   sys.exit(1)
来源：http://go.shxzukj.cn

PHP:  exit(1);
来源：http://sn.bjjhwx.cn

JS:   process.exit(1)
来源：http://hf.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ym.wgjwhj.cn

Java: System.exit(1)
来源：http://zs.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://fg.szsharing.cn

Ruby: exit 1
来源：http://ww.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ik.muxihuayi.cn

[M06] 向标准错误输出
来源：http://er.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://ho.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eh.gzmigu.cn

JS:   console.error("err")
来源：http://ef.wgjwhj.cn

TS:   console.error("err")
来源：http://rh.panjiajie.cn

Java: System.err.println("err")
来源：http://xc.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oa.huixinmuqiang.cn

Ruby: warn "err"
来源：http://oj.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ty.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://zw.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://mb.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sa.muxihuayi.cn

JS:   require.main === module
来源：http://pl.yuntaijiaju.cn

TS:   require.main === module
来源：http://em.hahajie.cn

Java: public static void main(String[] args)
来源：http://ex.shxzskj.cn

Go:   func main()
来源：http://fw.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iz.9csxet.cn

C#:   static void Main(string[] args)
来源：http://ll.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://ah.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://bo.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ot.nszjky.cn

JS:   process.platform;  process.version
来源：http://fv.panjiajie.cn

TS:   process.platform;  process.version
来源：http://xi.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pk.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dp.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yn.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vf.huixinmuqiang.cn

================================================================================
来源：http://ej.yuntaijiaju.cn

N. 数据结构与算法
来源：http://zt.colortex.cn

================================================================================
来源：http://qz.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://fg.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jz.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ep.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://if.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bq.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bg.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://wh.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qw.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uy.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://co.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://cs.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xs.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://it.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wz.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qp.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://yf.szsharing.cn

Ruby: arr.sort
来源：http://gd.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fh.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://xx.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ir.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ia.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uv.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yt.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mp.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jd.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xg.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rv.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://fi.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://se.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uy.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://va.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ga.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ln.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eu.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sb.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cj.chemitech.net.cn

[N05] 最大公约数
来源：http://fl.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ki.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ng.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ov.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ww.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dg.asd995.cn

Ruby: a.gcd(b)
来源：http://uu.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qt.hnjuh.cn

[N06] 判断回文字符串
来源：http://jo.wgjwhj.cn

Py:   s == s[::-1]
来源：http://kt.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://cu.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://fc.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://if.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://of.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://ni.hahajie.cn

Ruby: s == s.reverse
来源：http://pt.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://os.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://sj.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ob.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wa.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zs.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://nf.shtwfgs.cn

Java: // 手写 HashMap
来源：http://vs.hahajie.cn

Go:   // 手写 map[int]int
来源：http://vi.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://hy.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yl.panjiajie.cn

[N08] 生成全排列
来源：http://ma.colortex.cn

Py:   itertools.permutations(arr)
来源：http://fz.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://oi.9csxet.cn

JS:   // 手写回溯递归
来源：http://xn.newstarts.cn

TS:   // 手写回溯递归
来源：http://um.szsharing.cn

Java: // 手写回溯递归
来源：http://bc.huanxung.cn

Go:   // 手写回溯递归
来源：http://bq.521024.cn

Ruby: arr.permutation.to_a
来源：http://aq.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://rx.gzmigu.cn

[N09] 栈与队列
来源：http://tm.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qj.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xd.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://li.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fc.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sd.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://an.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lh.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hm.shtwfgs.cn

[N10] 链表节点定义
来源：http://dx.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fs.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eh.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tw.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sm.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://cl.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gs.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lt.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ar.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://qr.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zm.newstarts.cn

PHP:  // 手写递归函数
来源：http://ts.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rm.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zb.muxihuayi.cn

Java: // 手写递归
来源：http://hc.521024.cn

Go:   // 手写递归
来源：http://nu.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bt.asd995.cn

C#:   // 手写递归
来源：http://ss.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ot.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cq.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ez.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gy.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://du.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gy.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uz.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eo.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bq.jctech888.com.cn

================================================================================
来源：http://zh.muxihuayi.cn

O. 并发与异步
来源：http://wr.jctech888.com.cn

================================================================================
来源：http://xf.newstarts.cn

[O01] 启动一个线程
来源：http://vr.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vl.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gy.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mw.9csxet.cn

TS:   // 同 JS
来源：http://im.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://ic.colortex.cn

Go:   go f()
来源：http://pt.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://cd.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://zu.huanxung.cn

[O02] 使用线程池
来源：http://fm.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nr.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pk.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://qv.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://hg.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bl.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ai.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hq.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uk.szsharing.cn

[O03] 加锁保护共享数据
来源：http://nn.asd995.cn

Py:   with lock: shared += 1
来源：http://fh.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://pi.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yc.szsharing.cn

TS:   // 同 JS
来源：http://aa.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://qj.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oq.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://um.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://yq.9csxet.cn

[O04] 定义异步函数并等待
来源：http://um.521024.cn

Py:   async def f():⏎    await g()
来源：http://ze.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://td.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://mw.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sg.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vh.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://su.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dj.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://pa.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ih.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://ji.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dw.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://oc.colortex.cn

TS:   await Promise.all(tasks)
来源：http://eh.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jl.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rj.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://un.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jy.chemitech.net.cn

[O06] 使用进程池
来源：http://db.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cs.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yt.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://pg.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://dj.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ey.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pg.shxzskj.cn

Ruby: // fork 块
来源：http://ns.521024.cn

C#:   Parallel.For
来源：http://oz.muxihuayi.cn

================================================================================
来源：http://rc.nszjky.cn

P. 常用工具函数
来源：http://jl.muxihuayi.cn

================================================================================
来源：http://cl.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://ze.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://gb.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://me.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ll.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://np.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://xy.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://xp.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://ij.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://sl.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://vs.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dn.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fu.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://px.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mx.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gt.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nn.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ab.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iy.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://mn.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pa.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wy.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ry.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ou.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lp.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wz.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jw.yuntaijiaju.cn

[P04] 求长度
来源：http://ey.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ze.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://po.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zi.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qx.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://hd.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://mm.panjiajie.cn

Ruby: x.length;  x.size
来源：http://jc.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ht.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://xs.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nc.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yh.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wk.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://um.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cq.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ui.bookmarksfly.cn

Ruby: a == b
来源：http://pc.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://du.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://of.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ps.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://gd.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zu.haigaiapp.cn

TS:   if (x == null) {}
来源：http://aj.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uy.szxytkj.cn

Go:   if x == nil {}
来源：http://ut.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oh.nicolike.cn

C#:   if (x is null) {}
来源：http://vv.szxytkj.cn

[P07] 防抖与节流
来源：http://jo.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hx.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://py.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ui.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ri.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xe.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://du.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rb.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://od.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://yh.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://st.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bl.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xm.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wl.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kr.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://er.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cy.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nc.wgjwhj.cn

================================================================================
来源：http://dc.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://au.chemitech.net.cn

================================================================================
来源：http://pc.nszjky.cn

[Q01] 创建表
来源：http://wb.huixiangedu.cn

CREATE TABLE users (
来源：http://si.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ed.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://ic.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://vt.hnjuh.cn


<!-- 参考信息 -->