代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sy.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ld.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rk.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ne.szsharing.cn

[M04] 获取当前工作目录
来源：http://ni.wgjwhj.cn

Py:   os.getcwd()
来源：http://sy.colortex.cn

PHP:  getcwd();
来源：http://xc.gzmigu.cn

JS:   process.cwd()
来源：http://mc.wgjwhj.cn

TS:   process.cwd()
来源：http://nw.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://ya.panjiajie.cn

Go:   os.Getwd()
来源：http://ib.nicolike.cn

Ruby: Dir.pwd
来源：http://hz.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uy.shxzukj.cn

[M05] 设置退出码
来源：http://in.newstarts.cn

Py:   sys.exit(1)
来源：http://mn.wgjwhj.cn

PHP:  exit(1);
来源：http://xc.colortex.cn

JS:   process.exit(1)
来源：http://rn.nszjky.cn

TS:   process.exit(1)
来源：http://pg.jianghongdianzi.cn

Java: System.exit(1)
来源：http://fo.9csxet.cn

Go:   os.Exit(1)
来源：http://hl.nszjky.cn

Ruby: exit 1
来源：http://wq.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lq.gzmigu.cn

[M06] 向标准错误输出
来源：http://gv.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://rm.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ww.colortex.cn

JS:   console.error("err")
来源：http://zh.yuntaijiaju.cn

TS:   console.error("err")
来源：http://pu.shtwfgs.cn

Java: System.err.println("err")
来源：http://uu.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ko.shxzukj.cn

Ruby: warn "err"
来源：http://wq.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ps.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://pv.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ha.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xt.yuexingan06.cn

JS:   require.main === module
来源：http://mz.muxihuayi.cn

TS:   require.main === module
来源：http://ul.hahajie.cn

Java: public static void main(String[] args)
来源：http://kw.huixiangedu.cn

Go:   func main()
来源：http://tz.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vl.asd995.cn

C#:   static void Main(string[] args)
来源：http://th.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ep.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://fs.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ql.lnxyls.cn

JS:   process.platform;  process.version
来源：http://xk.9csxet.cn

TS:   process.platform;  process.version
来源：http://lr.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dd.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gt.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qo.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yq.jctech888.com.cn

================================================================================
来源：http://nr.jianghongdianzi.cn

N. 数据结构与算法
来源：http://ti.muxihuayi.cn

================================================================================
来源：http://dq.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://ci.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wq.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gn.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yn.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://km.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ya.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://ok.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sn.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ga.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://iy.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://ep.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bp.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kj.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dl.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pm.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://xo.lnxyls.cn

Ruby: arr.sort
来源：http://qz.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nv.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://rw.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://br.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://uz.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vi.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ki.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qi.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uh.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wy.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://na.521024.cn

[N04] 斐波那契数列
来源：http://bg.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kn.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ie.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zj.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bi.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vf.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://un.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ba.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haigaiapp.cn

[N05] 最大公约数
来源：http://mg.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://fk.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cb.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fx.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://co.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ru.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xx.lnxyls.cn

Ruby: a.gcd(b)
来源：http://xv.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sl.szsharing.cn

[N06] 判断回文字符串
来源：http://bq.newstarts.cn

Py:   s == s[::-1]
来源：http://qv.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://uw.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://vf.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://pt.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ak.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ek.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://lw.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fy.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://sd.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rh.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jt.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zu.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://cc.huanxung.cn

Java: // 手写 HashMap
来源：http://mu.nszjky.cn

Go:   // 手写 map[int]int
来源：http://zq.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://tk.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://us.wgjwhj.cn

[N08] 生成全排列
来源：http://gq.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://kc.asd995.cn

PHP:  // 手写递归交换
来源：http://kn.hahajie.cn

JS:   // 手写回溯递归
来源：http://uc.colortex.cn

TS:   // 手写回溯递归
来源：http://vh.panjiajie.cn

Java: // 手写回溯递归
来源：http://hv.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://dk.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://jx.gzmigu.cn

C#:   // 手写回溯递归
来源：http://rn.asd995.cn

[N09] 栈与队列
来源：http://dc.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vc.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://no.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ys.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vn.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tl.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kn.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ch.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fp.szsharing.cn

[N10] 链表节点定义
来源：http://jq.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oe.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kz.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ca.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://jg.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xm.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xd.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wv.521024.cn

[N11] 二叉树中序遍历
来源：http://vx.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eg.shxzskj.cn

PHP:  // 手写递归函数
来源：http://tl.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bj.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zf.colortex.cn

Java: // 手写递归
来源：http://pz.huixinmuqiang.cn

Go:   // 手写递归
来源：http://pf.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gr.huanxung.cn

C#:   // 手写递归
来源：http://fx.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oi.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://de.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wy.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ak.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hp.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gr.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hb.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://is.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qu.colortex.cn

================================================================================
来源：http://vi.hahajie.cn

O. 并发与异步
来源：http://yo.gzmigu.cn

================================================================================
来源：http://jm.asd995.cn

[O01] 启动一个线程
来源：http://lf.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vp.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rt.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qw.shtwfgs.cn

TS:   // 同 JS
来源：http://pm.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://va.lnxyls.cn

Go:   go f()
来源：http://fp.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://yo.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ae.szxytkj.cn

[O02] 使用线程池
来源：http://gs.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xt.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ok.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://pm.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://bh.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xd.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ys.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dk.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://og.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://te.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://px.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://hg.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ph.lnxyls.cn

TS:   // 同 JS
来源：http://ac.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://po.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sx.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gn.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://fj.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://gm.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ki.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dr.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://ac.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mo.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oz.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hj.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qt.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://bn.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://vl.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://yj.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zg.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://kt.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://wx.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ou.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tf.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://fs.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iv.lnxyls.cn

[O06] 使用进程池
来源：http://ou.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qk.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ed.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://hn.colortex.cn

TS:   // child_process / cluster 模块
来源：http://eu.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ew.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qr.lnxyls.cn

Ruby: // fork 块
来源：http://gm.lnxyls.cn

C#:   Parallel.For
来源：http://sz.nicolike.cn

================================================================================
来源：http://wb.huixiangedu.cn

P. 常用工具函数
来源：http://qg.lnxyls.cn

================================================================================
来源：http://xd.hnjuh.cn

[P01] 生成 UUID
来源：http://qa.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://pe.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pj.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://ll.szsharing.cn

TS:   crypto.randomUUID()
来源：http://lp.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://ex.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://iz.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://xk.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://jh.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://pe.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://op.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://en.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bb.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hl.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xn.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mg.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sx.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mo.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://bp.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ye.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vm.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pl.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sf.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://on.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://op.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vh.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kp.nszjky.cn

[P04] 求长度
来源：http://wy.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://so.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vh.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hf.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zc.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://if.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://xp.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://zz.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aj.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://md.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://aw.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jw.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uz.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ng.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ao.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uo.shtwfgs.cn

Ruby: a == b
来源：http://pl.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tb.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gs.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uv.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://ja.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pl.asd995.cn

TS:   if (x == null) {}
来源：http://kn.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kl.jctech888.com.cn

Go:   if x == nil {}
来源：http://pp.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fw.newstarts.cn

C#:   if (x is null) {}
来源：http://sq.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://bc.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://an.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://cw.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lz.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vs.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pr.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zm.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uf.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://dg.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gd.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yr.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ic.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xy.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zv.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bm.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://el.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zq.yuntaijiaju.cn

================================================================================
来源：http://fm.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kc.panjiajie.cn

================================================================================
来源：http://nh.yuexingan06.cn

[Q01] 创建表
来源：http://su.521024.cn

CREATE TABLE users (
来源：http://ax.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oh.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ws.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://qi.huixiangedu.cn


<!-- 参考信息 -->