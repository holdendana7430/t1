代发 wailian999

[M04] 获取当前工作目录
来源：http://uf.newstarts.cn

Py:   os.getcwd()
来源：http://lj.bookmarksfly.cn

PHP:  getcwd();
来源：http://uz.yuntaijiaju.cn

JS:   process.cwd()
来源：http://wv.shxzukj.cn

TS:   process.cwd()
来源：http://nm.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://jg.shtwfgs.cn

Go:   os.Getwd()
来源：http://fn.hahajie.cn

Ruby: Dir.pwd
来源：http://aq.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://il.hahajie.cn

[M05] 设置退出码
来源：http://xm.wgjwhj.cn

Py:   sys.exit(1)
来源：http://jh.bookmarksfly.cn

PHP:  exit(1);
来源：http://hb.chemitech.net.cn

JS:   process.exit(1)
来源：http://lv.yuexingan06.cn

TS:   process.exit(1)
来源：http://tt.szxytkj.cn

Java: System.exit(1)
来源：http://zb.wgjwhj.cn

Go:   os.Exit(1)
来源：http://qx.bookmarksfly.cn

Ruby: exit 1
来源：http://oj.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qn.hahajie.cn

[M06] 向标准错误输出
来源：http://et.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://su.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jo.nszjky.cn

JS:   console.error("err")
来源：http://ak.chemitech.net.cn

TS:   console.error("err")
来源：http://hy.wgjwhj.cn

Java: System.err.println("err")
来源：http://hy.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xz.9csxet.cn

Ruby: warn "err"
来源：http://hk.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ys.hnjuh.cn

[M07] 判断是否为主入口
来源：http://rs.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://hr.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hu.hnjuh.cn

JS:   require.main === module
来源：http://ae.chemitech.net.cn

TS:   require.main === module
来源：http://ev.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://qk.huanxung.cn

Go:   func main()
来源：http://xo.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vb.hahajie.cn

C#:   static void Main(string[] args)
来源：http://bt.asd995.cn

[M08] 获取系统与运行时信息
来源：http://ry.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://ab.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://mn.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://vq.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lm.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kv.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fn.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ah.shxzukj.cn

================================================================================
来源：http://dr.colortex.cn

N. 数据结构与算法
来源：http://xj.huixinmuqiang.cn

================================================================================
来源：http://bt.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://nv.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ii.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nk.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sp.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://in.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://oz.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lq.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kp.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://pj.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://vz.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://af.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zf.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vd.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ef.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://tx.muxihuayi.cn

Ruby: arr.sort
来源：http://ai.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ax.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://fp.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hy.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://kb.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gw.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bj.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fs.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lt.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ag.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pi.shxzukj.cn

[N04] 斐波那契数列
来源：http://ju.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mk.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xn.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lv.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dw.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nr.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ac.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vd.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fg.colortex.cn

[N05] 最大公约数
来源：http://fa.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://ry.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jn.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ov.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xy.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ip.hahajie.cn

Ruby: a.gcd(b)
来源：http://cl.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sk.lnxyls.cn

[N06] 判断回文字符串
来源：http://mf.chemitech.net.cn

Py:   s == s[::-1]
来源：http://eh.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://gt.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://gc.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://kk.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yv.newstarts.cn

Go:   // 双指针从两端比较
来源：http://py.9csxet.cn

Ruby: s == s.reverse
来源：http://ja.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ce.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://fb.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fk.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wa.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ei.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://gg.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://dj.huanxung.cn

Go:   // 手写 map[int]int
来源：http://qw.nszjky.cn

Ruby: // 手写 Hash
来源：http://fb.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sa.muxihuayi.cn

[N08] 生成全排列
来源：http://ja.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ul.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://cg.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ix.asd995.cn

TS:   // 手写回溯递归
来源：http://yn.9csxet.cn

Java: // 手写回溯递归
来源：http://ix.gzmigu.cn

Go:   // 手写回溯递归
来源：http://lq.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://nr.szsharing.cn

C#:   // 手写回溯递归
来源：http://iz.wgjwhj.cn

[N09] 栈与队列
来源：http://sz.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hx.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pk.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ij.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nk.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xv.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rd.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gv.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vu.szsharing.cn

[N10] 链表节点定义
来源：http://gj.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aq.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ky.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hj.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dw.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://kx.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gr.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pv.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pe.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://ru.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ur.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://bd.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gs.jctech888.com.cn

Java: // 手写递归
来源：http://kb.huixinmuqiang.cn

Go:   // 手写递归
来源：http://lj.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uu.lnxyls.cn

C#:   // 手写递归
来源：http://xd.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mf.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ol.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://by.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oa.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ah.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ly.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lw.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aa.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cx.chemitech.net.cn

================================================================================
来源：http://hy.haigaiapp.cn

O. 并发与异步
来源：http://qa.shxzukj.cn

================================================================================
来源：http://xt.shxzskj.cn

[O01] 启动一个线程
来源：http://gb.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yn.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ef.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fz.huanxung.cn

TS:   // 同 JS
来源：http://vl.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://uh.9csxet.cn

Go:   go f()
来源：http://bs.huanxung.cn

Ruby: Thread.new { f }
来源：http://ih.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://pb.asd995.cn

[O02] 使用线程池
来源：http://uo.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lg.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://si.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://lb.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://ob.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fo.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://am.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lu.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vf.9csxet.cn

[O03] 加锁保护共享数据
来源：http://fz.szsharing.cn

Py:   with lock: shared += 1
来源：http://lt.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://he.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mx.jianghongdianzi.cn

TS:   // 同 JS
来源：http://pt.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ap.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ml.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bw.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://gd.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://fq.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://gi.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ko.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ee.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xv.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ue.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qp.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pl.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ds.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://zk.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://jj.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fo.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://dw.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ww.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kq.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nc.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://kf.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ie.shtwfgs.cn

[O06] 使用进程池
来源：http://iz.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ix.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://il.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://aq.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ix.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rc.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sk.haigaiapp.cn

Ruby: // fork 块
来源：http://cp.lnxyls.cn

C#:   Parallel.For
来源：http://gm.newstarts.cn

================================================================================
来源：http://ze.huixinmuqiang.cn

P. 常用工具函数
来源：http://kk.huixiangedu.cn

================================================================================
来源：http://rx.huixiangedu.cn

[P01] 生成 UUID
来源：http://ab.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://il.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xt.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://qb.9csxet.cn

TS:   crypto.randomUUID()
来源：http://yz.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://ku.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://zv.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://ae.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://bk.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://np.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://og.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gm.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qv.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dn.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ce.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gg.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yp.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ki.9csxet.cn

[P03] 生成短随机字符串
来源：http://ak.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pd.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sn.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oa.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sa.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ky.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pt.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dg.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bq.gzmigu.cn

[P04] 求长度
来源：http://kv.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bo.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eq.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://is.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rq.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://zh.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://le.9csxet.cn

Ruby: x.length;  x.size
来源：http://io.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fr.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://zh.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bo.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rt.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zt.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://az.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ps.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cw.wgjwhj.cn

Ruby: a == b
来源：http://od.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tv.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vs.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gc.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://md.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kf.wgjwhj.cn

TS:   if (x == null) {}
来源：http://ms.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pi.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://vp.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dq.huanxung.cn

C#:   if (x is null) {}
来源：http://ql.wgjwhj.cn

[P07] 防抖与节流
来源：http://mq.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oe.colortex.cn

PHP:  // 手写时间戳比较
来源：http://my.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sz.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pz.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qo.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://du.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://dz.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ug.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bk.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vd.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xo.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lk.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ea.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gd.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hv.muxihuayi.cn

================================================================================
来源：http://mg.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rg.bjjhwx.cn

================================================================================
来源：http://jy.haigaiapp.cn

[Q01] 创建表
来源：http://ge.bookmarksfly.cn

CREATE TABLE users (
来源：http://xs.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ej.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://oo.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://qi.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hy.huanxung.cn

);
来源：http://vn.nicolike.cn

[Q02] 创建带外键的表
来源：http://ph.shtwfgs.cn

CREATE TABLE orders (
来源：http://ea.wgjwhj.cn


<!-- 参考信息 -->