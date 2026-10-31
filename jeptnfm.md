代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hy.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jk.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pu.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xn.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qj.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wi.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dk.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://lc.hahajie.cn

[M04] 获取当前工作目录
来源：http://ru.newstarts.cn

Py:   os.getcwd()
来源：http://yp.szsharing.cn

PHP:  getcwd();
来源：http://zm.newstarts.cn

JS:   process.cwd()
来源：http://gy.shxzskj.cn

TS:   process.cwd()
来源：http://za.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://kr.szxytkj.cn

Go:   os.Getwd()
来源：http://qu.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ml.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://su.yuntaijiaju.cn

[M05] 设置退出码
来源：http://lo.newstarts.cn

Py:   sys.exit(1)
来源：http://dt.colortex.cn

PHP:  exit(1);
来源：http://qi.muxihuayi.cn

JS:   process.exit(1)
来源：http://zp.newstarts.cn

TS:   process.exit(1)
来源：http://if.huixinmuqiang.cn

Java: System.exit(1)
来源：http://yf.szxytkj.cn

Go:   os.Exit(1)
来源：http://oj.chemitech.net.cn

Ruby: exit 1
来源：http://vf.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lq.muxihuayi.cn

[M06] 向标准错误输出
来源：http://dp.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://bj.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cp.521024.cn

JS:   console.error("err")
来源：http://kp.521024.cn

TS:   console.error("err")
来源：http://rt.huanxung.cn

Java: System.err.println("err")
来源：http://rq.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ll.szxytkj.cn

Ruby: warn "err"
来源：http://vg.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://ha.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://sl.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://uc.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zh.yuexingan06.cn

JS:   require.main === module
来源：http://lk.shtwfgs.cn

TS:   require.main === module
来源：http://al.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://hv.bookmarksfly.cn

Go:   func main()
来源：http://ca.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kz.9csxet.cn

C#:   static void Main(string[] args)
来源：http://lb.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://hv.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://tf.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://pf.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://tb.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://ut.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ka.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ed.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ob.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://op.colortex.cn

================================================================================
来源：http://cn.jianghongdianzi.cn

N. 数据结构与算法
来源：http://go.bjjhwx.cn

================================================================================
来源：http://op.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://pl.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fk.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qh.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xe.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://op.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ts.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://mv.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vk.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qy.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://rc.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://wr.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gg.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uq.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gz.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://to.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://wm.hnjuh.cn

Ruby: arr.sort
来源：http://pt.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bf.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://ke.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qf.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://ci.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ho.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lo.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kw.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yw.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://da.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jt.gzmigu.cn

[N04] 斐波那契数列
来源：http://bj.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sm.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gg.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tp.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sh.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dx.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://df.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tl.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zl.chemitech.net.cn

[N05] 最大公约数
来源：http://dr.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://sm.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tp.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ti.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hs.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ze.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rd.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://yu.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kp.hnjuh.cn

[N06] 判断回文字符串
来源：http://ke.colortex.cn

Py:   s == s[::-1]
来源：http://ss.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://oy.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://cs.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://zj.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fx.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://lf.9csxet.cn

Ruby: s == s.reverse
来源：http://bc.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vp.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://yw.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yq.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vu.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sc.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://uq.9csxet.cn

Java: // 手写 HashMap
来源：http://ua.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://rn.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://ij.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ik.yuntaijiaju.cn

[N08] 生成全排列
来源：http://cq.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://sa.szsharing.cn

PHP:  // 手写递归交换
来源：http://jm.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ml.nszjky.cn

TS:   // 手写回溯递归
来源：http://xt.panjiajie.cn

Java: // 手写回溯递归
来源：http://ln.newstarts.cn

Go:   // 手写回溯递归
来源：http://fy.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://be.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://py.nicolike.cn

[N09] 栈与队列
来源：http://sv.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hu.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tz.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bg.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fw.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gq.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gn.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iv.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lq.jctech888.com.cn

[N10] 链表节点定义
来源：http://ta.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nu.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lt.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mx.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iu.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://ao.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ko.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ig.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tl.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://jq.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gj.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ms.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jh.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ak.chemitech.net.cn

Java: // 手写递归
来源：http://kp.nszjky.cn

Go:   // 手写递归
来源：http://kt.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vq.szsharing.cn

C#:   // 手写递归
来源：http://wc.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ws.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bz.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qs.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://is.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vu.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zb.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sd.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kk.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ly.9csxet.cn

================================================================================
来源：http://qz.bjjhwx.cn

O. 并发与异步
来源：http://ye.huixinmuqiang.cn

================================================================================
来源：http://fz.nszjky.cn

[O01] 启动一个线程
来源：http://cd.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qf.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ap.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ek.colortex.cn

TS:   // 同 JS
来源：http://gz.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://pb.shtwfgs.cn

Go:   go f()
来源：http://vy.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://ws.newstarts.cn

C#:   Task.Run(() => F());
来源：http://jt.newstarts.cn

[O02] 使用线程池
来源：http://wf.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ar.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kn.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://sq.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://vc.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wq.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bh.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wa.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rq.huanxung.cn

[O03] 加锁保护共享数据
来源：http://fn.panjiajie.cn

Py:   with lock: shared += 1
来源：http://lw.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://kh.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://be.jianghongdianzi.cn

TS:   // 同 JS
来源：http://xu.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://xi.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mn.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ou.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://bz.nszjky.cn

[O04] 定义异步函数并等待
来源：http://bd.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://uo.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ud.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://fv.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wm.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bg.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ib.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ab.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://ta.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://yb.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://it.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tc.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://hx.colortex.cn

TS:   await Promise.all(tasks)
来源：http://fl.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ou.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zx.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://kv.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bi.colortex.cn

[O06] 使用进程池
来源：http://ih.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yl.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vw.colortex.cn

JS:   // child_process / cluster 模块
来源：http://zx.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://sc.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qa.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uz.jctech888.com.cn

Ruby: // fork 块
来源：http://ov.shxzukj.cn

C#:   Parallel.For
来源：http://ft.nicolike.cn

================================================================================
来源：http://ks.nszjky.cn

P. 常用工具函数
来源：http://ik.haigaiapp.cn

================================================================================
来源：http://sg.panjiajie.cn

[P01] 生成 UUID
来源：http://xq.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://ga.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jq.hahajie.cn

JS:   crypto.randomUUID()
来源：http://jz.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://oh.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://ba.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://bg.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://ek.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://bz.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://ai.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bm.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ue.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yf.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gc.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lr.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ev.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://na.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://we.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://up.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ah.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zl.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fm.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qq.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ih.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rb.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wy.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ey.wgjwhj.cn

[P04] 求长度
来源：http://ex.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://go.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hj.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lv.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gq.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://cl.nszjky.cn

Go:   len(arr);  len(m)
来源：http://zr.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://yn.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tb.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://rf.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kq.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://he.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eu.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rr.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uw.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uj.shtwfgs.cn

Ruby: a == b
来源：http://dm.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uq.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lj.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iq.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ff.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cj.asd995.cn

TS:   if (x == null) {}
来源：http://js.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mh.shxzukj.cn

Go:   if x == nil {}
来源：http://wt.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uh.shxzukj.cn

C#:   if (x is null) {}
来源：http://pl.szxytkj.cn

[P07] 防抖与节流
来源：http://om.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wi.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://dz.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sz.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vb.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vq.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jh.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zl.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oz.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://fb.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ta.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vq.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pf.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ly.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vd.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xe.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://br.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ik.521024.cn

================================================================================
来源：http://be.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mt.chemitech.net.cn

================================================================================
来源：http://sf.panjiajie.cn

[Q01] 创建表
来源：http://db.9csxet.cn


<!-- 参考信息 -->