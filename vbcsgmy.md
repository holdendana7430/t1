代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nw.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yx.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://io.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://cw.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://kc.nicolike.cn

Py:   os.getcwd()
来源：http://ca.chemitech.net.cn

PHP:  getcwd();
来源：http://bt.hahajie.cn

JS:   process.cwd()
来源：http://hs.wgjwhj.cn

TS:   process.cwd()
来源：http://it.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ow.9csxet.cn

Go:   os.Getwd()
来源：http://hh.asd995.cn

Ruby: Dir.pwd
来源：http://pz.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yj.muxihuayi.cn

[M05] 设置退出码
来源：http://nn.hahajie.cn

Py:   sys.exit(1)
来源：http://ek.shxzskj.cn

PHP:  exit(1);
来源：http://jf.nicolike.cn

JS:   process.exit(1)
来源：http://eo.jctech888.com.cn

TS:   process.exit(1)
来源：http://ar.jianghongdianzi.cn

Java: System.exit(1)
来源：http://om.wgjwhj.cn

Go:   os.Exit(1)
来源：http://dh.9csxet.cn

Ruby: exit 1
来源：http://fl.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dl.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://zs.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://mf.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mz.nszjky.cn

JS:   console.error("err")
来源：http://tx.9csxet.cn

TS:   console.error("err")
来源：http://ch.9csxet.cn

Java: System.err.println("err")
来源：http://ai.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oe.muxihuayi.cn

Ruby: warn "err"
来源：http://vz.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://xc.newstarts.cn

[M07] 判断是否为主入口
来源：http://ts.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://hd.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://de.muxihuayi.cn

JS:   require.main === module
来源：http://sw.jctech888.com.cn

TS:   require.main === module
来源：http://wa.shxzskj.cn

Java: public static void main(String[] args)
来源：http://dw.hahajie.cn

Go:   func main()
来源：http://wf.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ti.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://km.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://lj.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ye.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://co.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://ka.huanxung.cn

TS:   process.platform;  process.version
来源：http://ob.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jj.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xq.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fg.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fb.gzmigu.cn

================================================================================
来源：http://do.jctech888.com.cn

N. 数据结构与算法
来源：http://xi.nicolike.cn

================================================================================
来源：http://ma.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://um.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sg.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cw.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tu.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ul.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ok.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://to.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://nh.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://jw.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://su.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jl.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xs.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xy.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://gk.521024.cn

Ruby: arr.sort
来源：http://ry.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vn.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://so.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kt.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://dn.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sq.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pr.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ti.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pc.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bi.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://em.huanxung.cn

[N04] 斐波那契数列
来源：http://hw.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xx.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ay.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hu.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ll.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wd.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fr.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rm.lnxyls.cn

[N05] 最大公约数
来源：http://pr.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://af.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rd.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uj.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pl.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ir.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tm.asd995.cn

Ruby: a.gcd(b)
来源：http://gl.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hx.lnxyls.cn

[N06] 判断回文字符串
来源：http://vz.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://sy.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://hd.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://wy.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://en.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qz.huanxung.cn

Go:   // 双指针从两端比较
来源：http://si.shxzukj.cn

Ruby: s == s.reverse
来源：http://fk.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eh.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://la.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lm.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://of.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://zm.asd995.cn

Java: // 手写 HashMap
来源：http://dj.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://mv.9csxet.cn

Ruby: // 手写 Hash
来源：http://xg.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hn.szsharing.cn

[N08] 生成全排列
来源：http://zc.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://wm.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ke.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://jr.asd995.cn

TS:   // 手写回溯递归
来源：http://eb.haigaiapp.cn

Java: // 手写回溯递归
来源：http://qt.szsharing.cn

Go:   // 手写回溯递归
来源：http://ic.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ek.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://rq.newstarts.cn

[N09] 栈与队列
来源：http://ap.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://us.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aa.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ea.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yi.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ge.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ul.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ye.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ad.9csxet.cn

[N10] 链表节点定义
来源：http://bm.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pm.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fx.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hx.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zw.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://bg.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xz.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yx.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wb.hahajie.cn

[N11] 二叉树中序遍历
来源：http://mp.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vv.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://yw.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ej.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kv.nicolike.cn

Java: // 手写递归
来源：http://in.wgjwhj.cn

Go:   // 手写递归
来源：http://cf.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vf.hnjuh.cn

C#:   // 手写递归
来源：http://th.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bq.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ym.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zl.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xl.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vd.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hs.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nl.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qy.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uf.huixinmuqiang.cn

================================================================================
来源：http://qt.gzmigu.cn

O. 并发与异步
来源：http://se.hahajie.cn

================================================================================
来源：http://vo.muxihuayi.cn

[O01] 启动一个线程
来源：http://fd.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gw.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sm.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ic.lnxyls.cn

TS:   // 同 JS
来源：http://yb.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://oz.nszjky.cn

Go:   go f()
来源：http://cv.nicolike.cn

Ruby: Thread.new { f }
来源：http://zq.521024.cn

C#:   Task.Run(() => F());
来源：http://lg.lnxyls.cn

[O02] 使用线程池
来源：http://zo.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ee.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ph.asd995.cn

JS:   // worker_threads 线程池
来源：http://ay.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://ax.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ad.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mw.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ta.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bl.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://gl.huanxung.cn

Py:   with lock: shared += 1
来源：http://xs.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://zf.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ga.shtwfgs.cn

TS:   // 同 JS
来源：http://rn.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://ji.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yr.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ce.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://jy.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://ua.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://hv.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hq.asd995.cn

JS:   async function f() { await g(); }
来源：http://sg.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oe.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pu.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wf.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sc.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ju.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://gb.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://cu.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bc.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ue.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://xf.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nk.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zh.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://gd.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qm.colortex.cn

[O06] 使用进程池
来源：http://zl.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oa.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xf.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://tq.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://wq.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://li.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xm.jctech888.com.cn

Ruby: // fork 块
来源：http://qi.jctech888.com.cn

C#:   Parallel.For
来源：http://sw.521024.cn

================================================================================
来源：http://jq.shxzskj.cn

P. 常用工具函数
来源：http://dj.panjiajie.cn

================================================================================
来源：http://el.jctech888.com.cn

[P01] 生成 UUID
来源：http://mv.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://lb.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ox.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://gq.nicolike.cn

TS:   crypto.randomUUID()
来源：http://yx.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://mw.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://ij.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://lx.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://zd.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://pw.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ku.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hu.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bx.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gl.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cv.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hv.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mo.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fo.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ka.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yo.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yr.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uu.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ef.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ct.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hq.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xw.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qo.haigaiapp.cn

[P04] 求长度
来源：http://fw.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vg.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oc.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vj.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hq.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://bt.521024.cn

Go:   len(arr);  len(m)
来源：http://ly.shxzukj.cn

Ruby: x.length;  x.size
来源：http://hq.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vl.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ur.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gr.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cs.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zn.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ri.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wf.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jv.shxzskj.cn

Ruby: a == b
来源：http://mp.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wr.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vq.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qc.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://cf.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yn.panjiajie.cn

TS:   if (x == null) {}
来源：http://ue.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xz.nszjky.cn

Go:   if x == nil {}
来源：http://bx.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ao.9csxet.cn

C#:   if (x is null) {}
来源：http://ex.521024.cn

[P07] 防抖与节流
来源：http://dk.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dv.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://um.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nv.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xb.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fw.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rq.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pd.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nl.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://mb.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ti.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wb.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yo.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eu.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pc.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ux.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jd.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cr.newstarts.cn

================================================================================
来源：http://zb.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://er.shxzskj.cn

================================================================================
来源：http://ne.muxihuayi.cn

[Q01] 创建表
来源：http://eq.hahajie.cn

CREATE TABLE users (
来源：http://qw.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://og.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://lc.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://vg.asd995.cn


<!-- 参考信息 -->