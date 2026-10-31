代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jn.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fu.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fy.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://sc.521024.cn

[M04] 获取当前工作目录
来源：http://iw.shtwfgs.cn

Py:   os.getcwd()
来源：http://ay.jianghongdianzi.cn

PHP:  getcwd();
来源：http://xq.bjjhwx.cn

JS:   process.cwd()
来源：http://bj.nszjky.cn

TS:   process.cwd()
来源：http://ef.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://yl.huixiangedu.cn

Go:   os.Getwd()
来源：http://zz.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://nx.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sf.bjjhwx.cn

[M05] 设置退出码
来源：http://iu.gzmigu.cn

Py:   sys.exit(1)
来源：http://bt.muxihuayi.cn

PHP:  exit(1);
来源：http://hv.colortex.cn

JS:   process.exit(1)
来源：http://cw.haigaiapp.cn

TS:   process.exit(1)
来源：http://ft.hnjuh.cn

Java: System.exit(1)
来源：http://sc.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://gf.shtwfgs.cn

Ruby: exit 1
来源：http://ck.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ea.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://af.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://ab.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wp.yuntaijiaju.cn

JS:   console.error("err")
来源：http://qj.shxzukj.cn

TS:   console.error("err")
来源：http://tj.haigaiapp.cn

Java: System.err.println("err")
来源：http://fm.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fk.szxytkj.cn

Ruby: warn "err"
来源：http://ia.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://le.szxytkj.cn

[M07] 判断是否为主入口
来源：http://gn.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ty.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lm.lnxyls.cn

JS:   require.main === module
来源：http://rx.chemitech.net.cn

TS:   require.main === module
来源：http://zi.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://dq.bjjhwx.cn

Go:   func main()
来源：http://wc.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fg.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xq.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://qy.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://lq.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vx.nszjky.cn

JS:   process.platform;  process.version
来源：http://kb.gzmigu.cn

TS:   process.platform;  process.version
来源：http://wt.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ia.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ig.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://im.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ym.asd995.cn

================================================================================
来源：http://yb.huixinmuqiang.cn

N. 数据结构与算法
来源：http://wd.huixinmuqiang.cn

================================================================================
来源：http://xq.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://vx.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pr.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bn.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tv.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cl.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://kj.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lb.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gp.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ov.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://wq.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ok.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ep.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gb.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gi.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://qr.nicolike.cn

Ruby: arr.sort
来源：http://xo.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yf.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ke.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vu.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://pd.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hf.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pc.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gx.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mt.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ol.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://sp.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zy.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sl.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wc.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jd.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://le.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ul.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bv.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ez.nszjky.cn

[N05] 最大公约数
来源：http://mt.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ny.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kf.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bn.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uf.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rr.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qt.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://er.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ir.huanxung.cn

[N06] 判断回文字符串
来源：http://ru.hnjuh.cn

Py:   s == s[::-1]
来源：http://ho.szsharing.cn

PHP:  $s === strrev($s);
来源：http://zq.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ww.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://wo.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xr.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ud.wgjwhj.cn

Ruby: s == s.reverse
来源：http://he.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cf.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://lx.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kt.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://it.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jw.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://vz.newstarts.cn

Java: // 手写 HashMap
来源：http://nf.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://tb.hahajie.cn

Ruby: // 手写 Hash
来源：http://qe.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sm.hnjuh.cn

[N08] 生成全排列
来源：http://qh.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://jc.huanxung.cn

PHP:  // 手写递归交换
来源：http://oh.lnxyls.cn

JS:   // 手写回溯递归
来源：http://yt.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://wd.asd995.cn

Java: // 手写回溯递归
来源：http://ho.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://kr.colortex.cn

Ruby: arr.permutation.to_a
来源：http://le.colortex.cn

C#:   // 手写回溯递归
来源：http://fe.shxzukj.cn

[N09] 栈与队列
来源：http://bo.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fl.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wg.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tr.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sf.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cl.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jr.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ua.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.9csxet.cn

[N10] 链表节点定义
来源：http://lk.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ld.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ad.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yh.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mg.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://pt.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nl.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ke.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wk.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://tg.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jz.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ft.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mm.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kp.shxzskj.cn

Java: // 手写递归
来源：http://ig.panjiajie.cn

Go:   // 手写递归
来源：http://ps.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jg.huanxung.cn

C#:   // 手写递归
来源：http://uq.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pq.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://br.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://he.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ca.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mo.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jo.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qf.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qw.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gn.panjiajie.cn

================================================================================
来源：http://yq.jianghongdianzi.cn

O. 并发与异步
来源：http://sy.szxytkj.cn

================================================================================
来源：http://jv.9csxet.cn

[O01] 启动一个线程
来源：http://bc.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yw.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ka.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rf.nszjky.cn

TS:   // 同 JS
来源：http://oi.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://au.panjiajie.cn

Go:   go f()
来源：http://so.szsharing.cn

Ruby: Thread.new { f }
来源：http://et.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://vd.wgjwhj.cn

[O02] 使用线程池
来源：http://rw.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ny.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wq.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://lb.newstarts.cn

TS:   // worker_threads 线程池
来源：http://yq.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pb.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dk.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cw.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zg.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://hv.colortex.cn

Py:   with lock: shared += 1
来源：http://vd.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zi.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sk.yuntaijiaju.cn

TS:   // 同 JS
来源：http://rm.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://vi.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zz.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sv.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://xd.newstarts.cn

[O04] 定义异步函数并等待
来源：http://pb.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://hr.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uu.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://by.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ql.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sc.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://us.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qg.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://ul.521024.cn

[O05] 并发执行并等待全部完成
来源：http://jb.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://or.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zq.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://bq.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://qw.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oo.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hn.nicolike.cn

Ruby: threads.map(&:join)
来源：http://kb.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ey.huanxung.cn

[O06] 使用进程池
来源：http://la.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yw.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nu.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://op.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://um.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://co.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dw.gzmigu.cn

Ruby: // fork 块
来源：http://kn.muxihuayi.cn

C#:   Parallel.For
来源：http://xz.jctech888.com.cn

================================================================================
来源：http://qt.muxihuayi.cn

P. 常用工具函数
来源：http://po.yuntaijiaju.cn

================================================================================
来源：http://yw.yuexingan06.cn

[P01] 生成 UUID
来源：http://lo.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://jy.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sm.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://jc.9csxet.cn

TS:   crypto.randomUUID()
来源：http://ag.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://lt.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://md.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://nd.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://ph.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://yb.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ei.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rh.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rp.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xr.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gu.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xn.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wj.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jp.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://gx.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oh.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ig.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fd.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ts.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yb.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pr.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vt.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sz.wgjwhj.cn

[P04] 求长度
来源：http://xp.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qf.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mo.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ut.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sg.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://cz.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://bz.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://yl.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://az.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://sj.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vq.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ob.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ti.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bf.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ze.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lb.9csxet.cn

Ruby: a == b
来源：http://oe.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pj.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dy.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zp.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://ei.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zs.szxytkj.cn

TS:   if (x == null) {}
来源：http://uj.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wj.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://ym.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bq.521024.cn

C#:   if (x is null) {}
来源：http://dp.bjjhwx.cn

[P07] 防抖与节流
来源：http://rf.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kn.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://df.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uw.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gy.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://at.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gx.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://az.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sr.colortex.cn

[P08] 处理浮点精度问题
来源：http://fe.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://re.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tb.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kb.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oy.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mr.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://em.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eb.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://in.9csxet.cn

================================================================================
来源：http://sr.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ww.huixinmuqiang.cn

================================================================================
来源：http://cq.521024.cn

[Q01] 创建表
来源：http://jq.hnjuh.cn

CREATE TABLE users (
来源：http://uf.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://st.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://zk.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://jq.chemitech.net.cn


<!-- 参考信息 -->