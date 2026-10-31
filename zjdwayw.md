代发 wailian999

[M04] 获取当前工作目录
来源：http://cj.huanxung.cn

Py:   os.getcwd()
来源：http://hi.szxytkj.cn

PHP:  getcwd();
来源：http://et.9csxet.cn

JS:   process.cwd()
来源：http://db.asd995.cn

TS:   process.cwd()
来源：http://ou.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://ml.9csxet.cn

Go:   os.Getwd()
来源：http://fk.huanxung.cn

Ruby: Dir.pwd
来源：http://ll.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dd.nicolike.cn

[M05] 设置退出码
来源：http://fn.colortex.cn

Py:   sys.exit(1)
来源：http://fd.bjjhwx.cn

PHP:  exit(1);
来源：http://as.jctech888.com.cn

JS:   process.exit(1)
来源：http://yp.bookmarksfly.cn

TS:   process.exit(1)
来源：http://yf.shtwfgs.cn

Java: System.exit(1)
来源：http://un.chemitech.net.cn

Go:   os.Exit(1)
来源：http://aa.shxzskj.cn

Ruby: exit 1
来源：http://vw.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ls.shxzukj.cn

[M06] 向标准错误输出
来源：http://rw.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://zl.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pj.newstarts.cn

JS:   console.error("err")
来源：http://zw.yuntaijiaju.cn

TS:   console.error("err")
来源：http://ix.shxzukj.cn

Java: System.err.println("err")
来源：http://ab.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sg.chemitech.net.cn

Ruby: warn "err"
来源：http://ag.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://cx.9csxet.cn

[M07] 判断是否为主入口
来源：http://xm.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://tu.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aq.hahajie.cn

JS:   require.main === module
来源：http://gx.bookmarksfly.cn

TS:   require.main === module
来源：http://dg.szxytkj.cn

Java: public static void main(String[] args)
来源：http://tt.jianghongdianzi.cn

Go:   func main()
来源：http://ci.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rn.hahajie.cn

C#:   static void Main(string[] args)
来源：http://fg.colortex.cn

[M08] 获取系统与运行时信息
来源：http://ad.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://as.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://vt.hahajie.cn

JS:   process.platform;  process.version
来源：http://mm.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://qu.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sg.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://py.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://np.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuntaijiaju.cn

================================================================================
来源：http://tj.newstarts.cn

N. 数据结构与算法
来源：http://hd.szsharing.cn

================================================================================
来源：http://vf.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://pt.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sv.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qz.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fm.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nv.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qw.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://gl.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qv.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kw.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://wg.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zw.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xv.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xd.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tm.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wa.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://mb.newstarts.cn

Ruby: arr.sort
来源：http://iu.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nn.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ww.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gd.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://tg.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rr.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://be.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yz.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ab.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gm.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xk.newstarts.cn

[N04] 斐波那契数列
来源：http://gc.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dn.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ok.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cn.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uw.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nz.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fq.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cr.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yl.jianghongdianzi.cn

[N05] 最大公约数
来源：http://or.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://po.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dk.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ha.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gr.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://te.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://xw.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ib.521024.cn

[N06] 判断回文字符串
来源：http://et.szsharing.cn

Py:   s == s[::-1]
来源：http://ck.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://tl.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://rz.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://nx.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oh.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ac.nszjky.cn

Ruby: s == s.reverse
来源：http://xs.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yb.521024.cn

[N07] 两数之和（返回下标）
来源：http://cb.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nq.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uw.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ml.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://gw.hahajie.cn

Java: // 手写 HashMap
来源：http://hv.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://kn.gzmigu.cn

Ruby: // 手写 Hash
来源：http://eg.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ge.huixiangedu.cn

[N08] 生成全排列
来源：http://yn.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://xw.nicolike.cn

PHP:  // 手写递归交换
来源：http://yq.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://og.newstarts.cn

TS:   // 手写回溯递归
来源：http://ei.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://oj.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://fe.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://sv.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://dm.wgjwhj.cn

[N09] 栈与队列
来源：http://qj.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://al.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fr.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zz.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://en.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fg.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ze.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ls.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kn.gzmigu.cn

[N10] 链表节点定义
来源：http://ni.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ah.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uo.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ve.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yg.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://dw.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uw.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xt.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://km.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://yf.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eb.nicolike.cn

PHP:  // 手写递归函数
来源：http://dn.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nt.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xj.gzmigu.cn

Java: // 手写递归
来源：http://uh.asd995.cn

Go:   // 手写递归
来源：http://ff.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tt.szsharing.cn

C#:   // 手写递归
来源：http://gs.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wy.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kq.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://im.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ho.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://re.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hn.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gh.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dy.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oa.bookmarksfly.cn

================================================================================
来源：http://lj.panjiajie.cn

O. 并发与异步
来源：http://ov.nszjky.cn

================================================================================
来源：http://zs.lnxyls.cn

[O01] 启动一个线程
来源：http://dv.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dm.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nz.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ep.asd995.cn

TS:   // 同 JS
来源：http://hq.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://ev.panjiajie.cn

Go:   go f()
来源：http://lm.lnxyls.cn

Ruby: Thread.new { f }
来源：http://dw.hahajie.cn

C#:   Task.Run(() => F());
来源：http://qc.haigaiapp.cn

[O02] 使用线程池
来源：http://sy.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wr.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ks.9csxet.cn

JS:   // worker_threads 线程池
来源：http://kk.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://fp.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nb.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mm.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fe.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yb.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://ph.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://fn.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://cz.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://co.yuexingan06.cn

TS:   // 同 JS
来源：http://rt.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ea.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tz.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://at.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://cg.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://je.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://wt.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gb.nszjky.cn

JS:   async function f() { await g(); }
来源：http://au.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dj.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kl.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ft.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ux.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://xw.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://md.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ob.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qj.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://ho.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://xu.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cv.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uk.szsharing.cn

Ruby: threads.map(&:join)
来源：http://wy.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mn.yuexingan06.cn

[O06] 使用进程池
来源：http://jx.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://an.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ua.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://gq.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://dz.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gb.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dh.hahajie.cn

Ruby: // fork 块
来源：http://mj.huixinmuqiang.cn

C#:   Parallel.For
来源：http://gf.nszjky.cn

================================================================================
来源：http://ow.jianghongdianzi.cn

P. 常用工具函数
来源：http://eh.bookmarksfly.cn

================================================================================
来源：http://fx.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://xh.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://nt.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kx.521024.cn

JS:   crypto.randomUUID()
来源：http://mb.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://yl.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://gr.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://zh.521024.cn

Ruby: SecureRandom.uuid
来源：http://uo.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://qo.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://km.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fz.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://en.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sf.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rk.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xs.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xg.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hy.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ms.asd995.cn

[P03] 生成短随机字符串
来源：http://kx.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uy.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://si.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cq.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://su.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qr.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gm.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://md.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ph.yuntaijiaju.cn

[P04] 求长度
来源：http://ea.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://py.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://no.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://be.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ow.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://vf.hahajie.cn

Go:   len(arr);  len(m)
来源：http://zu.szxytkj.cn

Ruby: x.length;  x.size
来源：http://zy.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rx.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://wu.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gp.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ru.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hy.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bo.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rs.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oa.nicolike.cn

Ruby: a == b
来源：http://sj.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ij.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aq.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://st.asd995.cn

PHP:  if (empty($x)) {}
来源：http://eg.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bs.wgjwhj.cn

TS:   if (x == null) {}
来源：http://uc.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sh.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://su.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pe.shxzukj.cn

C#:   if (x is null) {}
来源：http://bm.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://vb.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://li.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://qy.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vs.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gx.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ex.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nf.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jw.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vi.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://dy.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ja.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hl.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gc.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ya.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uf.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://au.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pe.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fb.nszjky.cn

================================================================================
来源：http://ew.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xw.yuexingan06.cn

================================================================================
来源：http://az.nszjky.cn

[Q01] 创建表
来源：http://cg.chemitech.net.cn

CREATE TABLE users (
来源：http://hw.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kz.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://gg.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://sa.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vt.bookmarksfly.cn

);
来源：http://vm.9csxet.cn

[Q02] 创建带外键的表
来源：http://mp.wgjwhj.cn

CREATE TABLE orders (
来源：http://gr.9csxet.cn


<!-- 参考信息 -->