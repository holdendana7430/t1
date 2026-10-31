代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fe.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zq.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xk.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fa.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sb.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lw.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vs.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://tt.521024.cn

[M04] 获取当前工作目录
来源：http://xo.nicolike.cn

Py:   os.getcwd()
来源：http://xw.colortex.cn

PHP:  getcwd();
来源：http://xu.9csxet.cn

JS:   process.cwd()
来源：http://fa.shtwfgs.cn

TS:   process.cwd()
来源：http://wo.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://yt.nszjky.cn

Go:   os.Getwd()
来源：http://wm.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://oo.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nq.hahajie.cn

[M05] 设置退出码
来源：http://fm.nszjky.cn

Py:   sys.exit(1)
来源：http://if.hnjuh.cn

PHP:  exit(1);
来源：http://jw.szxytkj.cn

JS:   process.exit(1)
来源：http://pq.chemitech.net.cn

TS:   process.exit(1)
来源：http://cd.huixiangedu.cn

Java: System.exit(1)
来源：http://er.shxzukj.cn

Go:   os.Exit(1)
来源：http://jq.gzmigu.cn

Ruby: exit 1
来源：http://bf.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ht.nszjky.cn

[M06] 向标准错误输出
来源：http://zq.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://ga.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wa.huanxung.cn

JS:   console.error("err")
来源：http://zh.9csxet.cn

TS:   console.error("err")
来源：http://dn.huanxung.cn

Java: System.err.println("err")
来源：http://kx.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cz.szsharing.cn

Ruby: warn "err"
来源：http://xv.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://xu.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://dg.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://op.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yb.yuexingan06.cn

JS:   require.main === module
来源：http://vr.colortex.cn

TS:   require.main === module
来源：http://hh.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://kz.shxzskj.cn

Go:   func main()
来源：http://rv.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fc.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://yw.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://vi.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://zu.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://mv.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://rb.shxzukj.cn

TS:   process.platform;  process.version
来源：http://lq.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ch.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gn.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rl.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sr.hahajie.cn

================================================================================
来源：http://gs.muxihuayi.cn

N. 数据结构与算法
来源：http://zm.szsharing.cn

================================================================================
来源：http://li.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://jh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yo.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hx.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://du.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uz.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qr.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://yl.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://th.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gn.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://fx.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://vv.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pc.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pi.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zr.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cr.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://yx.wgjwhj.cn

Ruby: arr.sort
来源：http://sq.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ao.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://go.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ue.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://mt.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ad.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tb.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vd.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lj.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kr.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sn.colortex.cn

[N04] 斐波那契数列
来源：http://ts.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aj.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gl.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yd.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://md.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xt.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ed.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iq.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wa.colortex.cn

[N05] 最大公约数
来源：http://yv.huanxung.cn

Py:   math.gcd(a, b)
来源：http://ky.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mu.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://er.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://an.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jo.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oy.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://jk.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cz.szsharing.cn

[N06] 判断回文字符串
来源：http://oi.muxihuayi.cn

Py:   s == s[::-1]
来源：http://em.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://vx.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://lk.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://ab.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sx.asd995.cn

Go:   // 双指针从两端比较
来源：http://rt.haigaiapp.cn

Ruby: s == s.reverse
来源：http://hw.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cr.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://no.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ff.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nm.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jy.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://kj.huanxung.cn

Java: // 手写 HashMap
来源：http://uh.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ep.szxytkj.cn

Ruby: // 手写 Hash
来源：http://th.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qk.colortex.cn

[N08] 生成全排列
来源：http://ce.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://cp.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://uf.colortex.cn

JS:   // 手写回溯递归
来源：http://ie.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://sy.gzmigu.cn

Java: // 手写回溯递归
来源：http://ys.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://cw.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://uw.gzmigu.cn

C#:   // 手写回溯递归
来源：http://jf.colortex.cn

[N09] 栈与队列
来源：http://qj.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gh.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uz.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hd.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dm.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ou.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ey.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ad.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cy.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ve.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cp.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nq.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rg.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zm.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://iy.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fq.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uw.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hv.nszjky.cn

[N11] 二叉树中序遍历
来源：http://es.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ia.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://xn.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qf.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yu.hahajie.cn

Java: // 手写递归
来源：http://ua.wgjwhj.cn

Go:   // 手写递归
来源：http://ei.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://td.521024.cn

C#:   // 手写递归
来源：http://nd.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pg.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qy.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ui.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cq.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vb.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ss.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://di.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tv.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jw.muxihuayi.cn

================================================================================
来源：http://zx.lnxyls.cn

O. 并发与异步
来源：http://rs.wgjwhj.cn

================================================================================
来源：http://tb.bookmarksfly.cn

[O01] 启动一个线程
来源：http://kt.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iz.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zw.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://he.muxihuayi.cn

TS:   // 同 JS
来源：http://kv.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://ep.huixiangedu.cn

Go:   go f()
来源：http://cx.gzmigu.cn

Ruby: Thread.new { f }
来源：http://uq.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://gt.szsharing.cn

[O02] 使用线程池
来源：http://on.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vd.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uk.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://jk.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://bz.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ns.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qd.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cd.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qi.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ty.colortex.cn

Py:   with lock: shared += 1
来源：http://su.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ru.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ty.muxihuayi.cn

TS:   // 同 JS
来源：http://vu.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://ba.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ne.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yi.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://ri.9csxet.cn

[O04] 定义异步函数并等待
来源：http://bt.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://sc.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gr.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://vo.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uc.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pg.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hh.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://uc.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://gu.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://jb.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yz.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ve.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://ez.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mo.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mg.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://wh.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mz.9csxet.cn

[O06] 使用进程池
来源：http://ee.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oj.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ko.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://fy.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://fk.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oa.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tb.nszjky.cn

Ruby: // fork 块
来源：http://lu.colortex.cn

C#:   Parallel.For
来源：http://as.newstarts.cn

================================================================================
来源：http://lx.jctech888.com.cn

P. 常用工具函数
来源：http://cc.gzmigu.cn

================================================================================
来源：http://lt.bjjhwx.cn

[P01] 生成 UUID
来源：http://jz.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://kz.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://af.9csxet.cn

JS:   crypto.randomUUID()
来源：http://cw.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://nb.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://yt.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://nq.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://ro.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://nf.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://ez.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pr.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xd.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ux.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bn.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uo.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rg.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nq.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jw.szsharing.cn

[P03] 生成短随机字符串
来源：http://nu.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sc.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://um.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pi.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://db.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fh.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://od.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wn.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kx.gzmigu.cn

[P04] 求长度
来源：http://mv.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qn.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hs.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wu.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://aj.szsharing.cn

Go:   len(arr);  len(m)
来源：http://lr.newstarts.cn

Ruby: x.length;  x.size
来源：http://ls.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://db.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://hl.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zr.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qm.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fc.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fa.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ql.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ou.jianghongdianzi.cn

Ruby: a == b
来源：http://ug.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bb.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wm.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oj.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://ck.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pt.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://tq.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bh.colortex.cn

Go:   if x == nil {}
来源：http://ku.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uk.huanxung.cn

C#:   if (x is null) {}
来源：http://ih.nszjky.cn

[P07] 防抖与节流
来源：http://qp.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ri.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://vs.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pa.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://et.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ob.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qg.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sf.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sg.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://rl.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ga.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://le.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kb.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uc.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cj.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ik.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ly.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yt.bookmarksfly.cn

================================================================================
来源：http://qy.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bn.huanxung.cn

================================================================================
来源：http://dz.shxzukj.cn

[Q01] 创建表
来源：http://zl.haigaiapp.cn


<!-- 参考信息 -->