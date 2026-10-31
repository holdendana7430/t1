代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pt.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zb.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oz.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://gk.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://yb.panjiajie.cn

Py:   os.getcwd()
来源：http://xz.yuntaijiaju.cn

PHP:  getcwd();
来源：http://ne.muxihuayi.cn

JS:   process.cwd()
来源：http://il.szxytkj.cn

TS:   process.cwd()
来源：http://lp.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://js.shxzukj.cn

Go:   os.Getwd()
来源：http://fs.huanxung.cn

Ruby: Dir.pwd
来源：http://la.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oc.colortex.cn

[M05] 设置退出码
来源：http://xg.chemitech.net.cn

Py:   sys.exit(1)
来源：http://vz.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ui.newstarts.cn

JS:   process.exit(1)
来源：http://ta.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://lw.huixinmuqiang.cn

Java: System.exit(1)
来源：http://sb.9csxet.cn

Go:   os.Exit(1)
来源：http://nu.shxzukj.cn

Ruby: exit 1
来源：http://yb.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ow.szsharing.cn

[M06] 向标准错误输出
来源：http://nv.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ds.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hs.jianghongdianzi.cn

JS:   console.error("err")
来源：http://px.szsharing.cn

TS:   console.error("err")
来源：http://fv.muxihuayi.cn

Java: System.err.println("err")
来源：http://ks.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yn.9csxet.cn

Ruby: warn "err"
来源：http://ew.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://na.shxzskj.cn

[M07] 判断是否为主入口
来源：http://yl.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://xw.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gl.newstarts.cn

JS:   require.main === module
来源：http://dc.colortex.cn

TS:   require.main === module
来源：http://lr.colortex.cn

Java: public static void main(String[] args)
来源：http://ev.panjiajie.cn

Go:   func main()
来源：http://vj.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kq.521024.cn

C#:   static void Main(string[] args)
来源：http://ix.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://wl.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ah.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://dl.szsharing.cn

JS:   process.platform;  process.version
来源：http://tl.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://in.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wx.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pp.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bu.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lc.colortex.cn

================================================================================
来源：http://sn.yuexingan06.cn

N. 数据结构与算法
来源：http://ps.huixinmuqiang.cn

================================================================================
来源：http://et.521024.cn

[N01] 二分查找（有序数组）
来源：http://ye.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ju.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zg.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cw.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rq.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ad.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ap.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rp.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pc.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://hl.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ur.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ww.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://py.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hq.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://av.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://wa.yuexingan06.cn

Ruby: arr.sort
来源：http://sx.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mo.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://mn.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xe.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ie.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aw.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qz.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://av.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pp.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sk.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vs.chemitech.net.cn

[N04] 斐波那契数列
来源：http://bu.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wv.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://za.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ak.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://br.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vx.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tw.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fu.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nl.huixinmuqiang.cn

[N05] 最大公约数
来源：http://oj.hahajie.cn

Py:   math.gcd(a, b)
来源：http://cl.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bp.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qv.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wq.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fv.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zs.hahajie.cn

Ruby: a.gcd(b)
来源：http://hg.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ud.newstarts.cn

[N06] 判断回文字符串
来源：http://jh.szxytkj.cn

Py:   s == s[::-1]
来源：http://ox.colortex.cn

PHP:  $s === strrev($s);
来源：http://nq.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://qe.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://az.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ds.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://po.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://xy.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ux.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://ax.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dx.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jn.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yh.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://fx.colortex.cn

Java: // 手写 HashMap
来源：http://lb.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://gu.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://aa.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cv.shtwfgs.cn

[N08] 生成全排列
来源：http://ob.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://hd.szxytkj.cn

PHP:  // 手写递归交换
来源：http://vf.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://pw.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://am.shtwfgs.cn

Java: // 手写回溯递归
来源：http://rq.colortex.cn

Go:   // 手写回溯递归
来源：http://bl.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://hh.shxzskj.cn

C#:   // 手写回溯递归
来源：http://xw.521024.cn

[N09] 栈与队列
来源：http://zr.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zq.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yv.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iy.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ko.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ze.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ol.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xr.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wp.yuexingan06.cn

[N10] 链表节点定义
来源：http://ro.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rq.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://es.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qo.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lx.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://xa.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sa.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ur.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://li.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://wy.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vb.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://aq.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yq.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pc.lnxyls.cn

Java: // 手写递归
来源：http://gm.asd995.cn

Go:   // 手写递归
来源：http://qv.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xt.panjiajie.cn

C#:   // 手写递归
来源：http://ve.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nd.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jd.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jz.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ej.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://li.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mk.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ab.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://id.nicolike.cn

================================================================================
来源：http://md.yuexingan06.cn

O. 并发与异步
来源：http://bk.shxzskj.cn

================================================================================
来源：http://go.muxihuayi.cn

[O01] 启动一个线程
来源：http://ir.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wx.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ml.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://we.panjiajie.cn

TS:   // 同 JS
来源：http://tx.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://jl.bookmarksfly.cn

Go:   go f()
来源：http://xe.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://bo.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://qy.panjiajie.cn

[O02] 使用线程池
来源：http://lx.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uh.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jn.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://ai.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://aq.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://et.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nu.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ps.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cy.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://uq.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://yi.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://tk.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://on.huixinmuqiang.cn

TS:   // 同 JS
来源：http://yj.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ug.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ot.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fr.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://gu.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://my.521024.cn

Py:   async def f():⏎    await g()
来源：http://pc.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uh.colortex.cn

JS:   async function f() { await g(); }
来源：http://ya.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ls.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ek.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eu.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ac.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://xb.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://ez.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://gh.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://or.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://cp.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://ca.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rg.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://td.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://bg.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ga.hahajie.cn

[O06] 使用进程池
来源：http://hr.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cu.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vo.521024.cn

JS:   // child_process / cluster 模块
来源：http://qy.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://jo.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xy.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mh.huanxung.cn

Ruby: // fork 块
来源：http://si.nszjky.cn

C#:   Parallel.For
来源：http://cz.chemitech.net.cn

================================================================================
来源：http://yy.shtwfgs.cn

P. 常用工具函数
来源：http://up.huixiangedu.cn

================================================================================
来源：http://ft.muxihuayi.cn

[P01] 生成 UUID
来源：http://zu.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://da.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vn.nszjky.cn

JS:   crypto.randomUUID()
来源：http://fb.colortex.cn

TS:   crypto.randomUUID()
来源：http://xb.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://je.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://nv.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://qy.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://cf.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://yt.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yb.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ib.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://km.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xn.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://to.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rk.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nr.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bl.lnxyls.cn

[P03] 生成短随机字符串
来源：http://tj.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rr.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kw.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wn.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ee.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xw.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ot.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fx.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ga.panjiajie.cn

[P04] 求长度
来源：http://hz.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wi.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ky.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://if.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kf.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://pk.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://wc.hnjuh.cn

Ruby: x.length;  x.size
来源：http://yi.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mr.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://xe.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fu.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vk.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://he.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kv.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rw.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pd.jianghongdianzi.cn

Ruby: a == b
来源：http://bi.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cp.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qt.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wh.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://ez.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yd.9csxet.cn

TS:   if (x == null) {}
来源：http://iv.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lr.haigaiapp.cn

Go:   if x == nil {}
来源：http://bm.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wo.521024.cn

C#:   if (x is null) {}
来源：http://xq.szxytkj.cn

[P07] 防抖与节流
来源：http://jw.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ru.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://px.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bx.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xc.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nv.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xj.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jt.asd995.cn

[P08] 处理浮点精度问题
来源：http://kl.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://di.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iy.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://im.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uo.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dy.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://au.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ta.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oc.nicolike.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xk.hahajie.cn

================================================================================
来源：http://pl.szsharing.cn

[Q01] 创建表
来源：http://ys.9csxet.cn

CREATE TABLE users (
来源：http://qk.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rc.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ov.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://ih.jctech888.com.cn


<!-- 参考信息 -->