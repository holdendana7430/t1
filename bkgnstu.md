代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sj.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://em.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gv.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://it.lnxyls.cn

[M04] 获取当前工作目录
来源：http://mm.shtwfgs.cn

Py:   os.getcwd()
来源：http://cp.hnjuh.cn

PHP:  getcwd();
来源：http://cm.szxytkj.cn

JS:   process.cwd()
来源：http://uh.lnxyls.cn

TS:   process.cwd()
来源：http://tk.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://iu.lnxyls.cn

Go:   os.Getwd()
来源：http://un.wgjwhj.cn

Ruby: Dir.pwd
来源：http://kw.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fz.szsharing.cn

[M05] 设置退出码
来源：http://dq.chemitech.net.cn

Py:   sys.exit(1)
来源：http://qo.szsharing.cn

PHP:  exit(1);
来源：http://dn.huixiangedu.cn

JS:   process.exit(1)
来源：http://vx.hnjuh.cn

TS:   process.exit(1)
来源：http://zj.haigaiapp.cn

Java: System.exit(1)
来源：http://qh.chemitech.net.cn

Go:   os.Exit(1)
来源：http://rb.lnxyls.cn

Ruby: exit 1
来源：http://xc.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://go.nicolike.cn

[M06] 向标准错误输出
来源：http://lc.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://tr.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ao.shtwfgs.cn

JS:   console.error("err")
来源：http://zw.lnxyls.cn

TS:   console.error("err")
来源：http://az.yuexingan06.cn

Java: System.err.println("err")
来源：http://uk.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://la.huanxung.cn

Ruby: warn "err"
来源：http://jz.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://sa.nszjky.cn

[M07] 判断是否为主入口
来源：http://om.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://if.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sm.huixinmuqiang.cn

JS:   require.main === module
来源：http://rx.szsharing.cn

TS:   require.main === module
来源：http://bx.szsharing.cn

Java: public static void main(String[] args)
来源：http://fn.huanxung.cn

Go:   func main()
来源：http://pi.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rg.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://cc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://me.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://cp.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://nn.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://wd.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://ps.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rt.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ww.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bm.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pi.szxytkj.cn

================================================================================
来源：http://ua.yuntaijiaju.cn

N. 数据结构与算法
来源：http://fo.bookmarksfly.cn

================================================================================
来源：http://zt.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://qh.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bm.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pe.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fq.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ij.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zd.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bh.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nw.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://oy.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ih.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ib.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gq.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mm.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ez.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://ut.szxytkj.cn

Ruby: arr.sort
来源：http://ny.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cs.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://lz.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hd.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://zk.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ri.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ry.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gb.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yh.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zr.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jr.colortex.cn

[N04] 斐波那契数列
来源：http://zs.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dr.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nx.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kq.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ef.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ca.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wl.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ca.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gb.wgjwhj.cn

[N05] 最大公约数
来源：http://eh.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://eo.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uz.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kl.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hc.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fm.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aj.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ha.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fw.wgjwhj.cn

[N06] 判断回文字符串
来源：http://sg.haigaiapp.cn

Py:   s == s[::-1]
来源：http://eo.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://lt.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://nh.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://wz.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eu.nicolike.cn

Go:   // 双指针从两端比较
来源：http://wp.jctech888.com.cn

Ruby: s == s.reverse
来源：http://ft.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ba.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://xp.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dp.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bw.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hr.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://lk.muxihuayi.cn

Java: // 手写 HashMap
来源：http://ib.colortex.cn

Go:   // 手写 map[int]int
来源：http://xz.szsharing.cn

Ruby: // 手写 Hash
来源：http://fj.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ax.wgjwhj.cn

[N08] 生成全排列
来源：http://ag.asd995.cn

Py:   itertools.permutations(arr)
来源：http://uh.shxzukj.cn

PHP:  // 手写递归交换
来源：http://ra.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ge.nszjky.cn

TS:   // 手写回溯递归
来源：http://ye.newstarts.cn

Java: // 手写回溯递归
来源：http://hl.shxzskj.cn

Go:   // 手写回溯递归
来源：http://yf.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://qt.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://me.szsharing.cn

[N09] 栈与队列
来源：http://qp.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://et.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lq.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tv.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pq.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lz.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ta.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wo.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yh.bjjhwx.cn

[N10] 链表节点定义
来源：http://km.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qt.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mk.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fh.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qs.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://tq.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vy.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gd.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lk.asd995.cn

[N11] 二叉树中序遍历
来源：http://pj.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://er.9csxet.cn

PHP:  // 手写递归函数
来源：http://ta.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ht.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kc.shxzukj.cn

Java: // 手写递归
来源：http://mf.newstarts.cn

Go:   // 手写递归
来源：http://zg.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qt.szsharing.cn

C#:   // 手写递归
来源：http://kc.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://al.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ue.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qd.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zq.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zs.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bh.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ih.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rn.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dg.haigaiapp.cn

================================================================================
来源：http://fo.lnxyls.cn

O. 并发与异步
来源：http://ns.hahajie.cn

================================================================================
来源：http://jw.shxzukj.cn

[O01] 启动一个线程
来源：http://rp.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fz.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ew.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ug.yuexingan06.cn

TS:   // 同 JS
来源：http://ns.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://qt.lnxyls.cn

Go:   go f()
来源：http://zy.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://qn.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://cg.asd995.cn

[O02] 使用线程池
来源：http://rf.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hg.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qi.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://ad.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://wa.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kv.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sq.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ea.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ln.asd995.cn

[O03] 加锁保护共享数据
来源：http://vi.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://od.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://uw.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rf.jctech888.com.cn

TS:   // 同 JS
来源：http://bb.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://gf.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lq.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qo.521024.cn

C#:   lock (gate) { shared++; }
来源：http://wz.szsharing.cn

[O04] 定义异步函数并等待
来源：http://nk.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://cf.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://he.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://ib.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ay.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wo.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wn.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pk.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://kz.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://qx.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://tk.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kv.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://kr.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://th.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bk.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xj.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://tj.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ug.panjiajie.cn

[O06] 使用进程池
来源：http://vs.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fp.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qp.colortex.cn

JS:   // child_process / cluster 模块
来源：http://kj.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://jk.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yu.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ho.colortex.cn

Ruby: // fork 块
来源：http://mr.colortex.cn

C#:   Parallel.For
来源：http://ne.shxzukj.cn

================================================================================
来源：http://cg.bjjhwx.cn

P. 常用工具函数
来源：http://md.jctech888.com.cn

================================================================================
来源：http://mg.szxytkj.cn

[P01] 生成 UUID
来源：http://su.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://qx.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://da.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://sb.hahajie.cn

TS:   crypto.randomUUID()
来源：http://gg.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://hx.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://io.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://lo.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://es.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ar.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bp.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yi.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bg.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yi.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tv.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://go.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dz.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ys.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://ch.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mf.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ld.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ne.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gq.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ah.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zm.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vd.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hw.nszjky.cn

[P04] 求长度
来源：http://dl.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mm.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ne.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hh.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aj.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://to.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://gh.9csxet.cn

Ruby: x.length;  x.size
来源：http://ff.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eg.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://xp.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lv.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qc.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xo.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zu.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jh.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ec.hahajie.cn

Ruby: a == b
来源：http://da.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xh.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dl.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://il.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://aw.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mj.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://lq.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jt.nszjky.cn

Go:   if x == nil {}
来源：http://wy.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://no.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://bx.panjiajie.cn

[P07] 防抖与节流
来源：http://da.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pk.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://sz.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dg.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dq.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://na.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kd.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ap.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jw.colortex.cn

[P08] 处理浮点精度问题
来源：http://sy.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ty.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mv.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xf.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://br.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cq.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gi.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rl.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vi.jianghongdianzi.cn

================================================================================
来源：http://wm.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zw.huanxung.cn

================================================================================
来源：http://dm.haigaiapp.cn

[Q01] 创建表
来源：http://jq.nicolike.cn

CREATE TABLE users (
来源：http://ij.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tq.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://yn.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://xe.yuntaijiaju.cn


<!-- 参考信息 -->