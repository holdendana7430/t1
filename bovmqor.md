代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cx.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ma.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sm.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://hc.hahajie.cn

[M04] 获取当前工作目录
来源：http://wb.shtwfgs.cn

Py:   os.getcwd()
来源：http://zn.521024.cn

PHP:  getcwd();
来源：http://mk.lnxyls.cn

JS:   process.cwd()
来源：http://zb.huixiangedu.cn

TS:   process.cwd()
来源：http://ca.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://rd.jctech888.com.cn

Go:   os.Getwd()
来源：http://oz.bjjhwx.cn

Ruby: Dir.pwd
来源：http://jh.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wv.huixiangedu.cn

[M05] 设置退出码
来源：http://iz.yuexingan06.cn

Py:   sys.exit(1)
来源：http://wf.9csxet.cn

PHP:  exit(1);
来源：http://ae.asd995.cn

JS:   process.exit(1)
来源：http://wu.yuexingan06.cn

TS:   process.exit(1)
来源：http://tu.huixiangedu.cn

Java: System.exit(1)
来源：http://cj.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://st.huanxung.cn

Ruby: exit 1
来源：http://cc.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://io.szsharing.cn

[M06] 向标准错误输出
来源：http://ew.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://id.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cx.bjjhwx.cn

JS:   console.error("err")
来源：http://ua.newstarts.cn

TS:   console.error("err")
来源：http://xc.szxytkj.cn

Java: System.err.println("err")
来源：http://hl.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ra.bjjhwx.cn

Ruby: warn "err"
来源：http://hv.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://jn.hahajie.cn

[M07] 判断是否为主入口
来源：http://an.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://xg.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jb.9csxet.cn

JS:   require.main === module
来源：http://ci.huanxung.cn

TS:   require.main === module
来源：http://ff.521024.cn

Java: public static void main(String[] args)
来源：http://ek.asd995.cn

Go:   func main()
来源：http://yt.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bo.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://mn.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://ky.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://oh.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://mw.hnjuh.cn

JS:   process.platform;  process.version
来源：http://er.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://wm.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ei.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mw.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gc.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zp.hnjuh.cn

================================================================================
来源：http://cd.gzmigu.cn

N. 数据结构与算法
来源：http://hz.bjjhwx.cn

================================================================================
来源：http://gb.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://lg.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fm.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fa.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rq.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oz.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://jo.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dj.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qt.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://ng.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://gu.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lo.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fl.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ur.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://we.nicolike.cn

Go:   slices.Sort(arr)
来源：http://eq.huixinmuqiang.cn

Ruby: arr.sort
来源：http://xo.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ak.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://ql.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://gc.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vs.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fz.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nq.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tm.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bc.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ut.lnxyls.cn

[N04] 斐波那契数列
来源：http://vy.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://re.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rg.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uv.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ud.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vs.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sr.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ss.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cm.jianghongdianzi.cn

[N05] 最大公约数
来源：http://bm.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://jn.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bv.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pi.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nw.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zh.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nf.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://xp.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://co.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://fc.chemitech.net.cn

Py:   s == s[::-1]
来源：http://yc.9csxet.cn

PHP:  $s === strrev($s);
来源：http://lj.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://xw.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://vh.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yg.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://lq.lnxyls.cn

Ruby: s == s.reverse
来源：http://xq.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://la.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://sw.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iy.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zm.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://al.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ar.wgjwhj.cn

Java: // 手写 HashMap
来源：http://gk.nicolike.cn

Go:   // 手写 map[int]int
来源：http://fp.hahajie.cn

Ruby: // 手写 Hash
来源：http://uv.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ms.shxzukj.cn

[N08] 生成全排列
来源：http://dj.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://yl.newstarts.cn

PHP:  // 手写递归交换
来源：http://mj.panjiajie.cn

JS:   // 手写回溯递归
来源：http://nu.shxzukj.cn

TS:   // 手写回溯递归
来源：http://us.shtwfgs.cn

Java: // 手写回溯递归
来源：http://yc.gzmigu.cn

Go:   // 手写回溯递归
来源：http://kt.521024.cn

Ruby: arr.permutation.to_a
来源：http://en.colortex.cn

C#:   // 手写回溯递归
来源：http://uz.bookmarksfly.cn

[N09] 栈与队列
来源：http://ib.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pl.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cd.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sk.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://py.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yn.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ac.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iq.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sc.bjjhwx.cn

[N10] 链表节点定义
来源：http://bf.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ha.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://la.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ao.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pf.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://vt.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ro.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hf.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gf.9csxet.cn

[N11] 二叉树中序遍历
来源：http://oe.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xx.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://pj.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xn.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ey.shxzskj.cn

Java: // 手写递归
来源：http://iv.huanxung.cn

Go:   // 手写递归
来源：http://cs.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ga.huixiangedu.cn

C#:   // 手写递归
来源：http://wq.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kg.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eu.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bl.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://av.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://op.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ov.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ke.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xs.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sx.shtwfgs.cn

================================================================================
来源：http://oc.asd995.cn

O. 并发与异步
来源：http://rn.hahajie.cn

================================================================================
来源：http://tn.hnjuh.cn

[O01] 启动一个线程
来源：http://qy.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ne.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bw.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vs.nicolike.cn

TS:   // 同 JS
来源：http://zm.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://fy.hnjuh.cn

Go:   go f()
来源：http://zx.lnxyls.cn

Ruby: Thread.new { f }
来源：http://sh.9csxet.cn

C#:   Task.Run(() => F());
来源：http://mr.asd995.cn

[O02] 使用线程池
来源：http://fw.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nu.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cv.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ok.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://nl.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uc.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yj.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ta.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://av.newstarts.cn

[O03] 加锁保护共享数据
来源：http://nm.gzmigu.cn

Py:   with lock: shared += 1
来源：http://wp.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ow.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ko.newstarts.cn

TS:   // 同 JS
来源：http://cq.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://wy.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nf.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ax.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://sb.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://sl.asd995.cn

Py:   async def f():⏎    await g()
来源：http://dh.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dw.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://xm.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://de.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vy.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wz.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tc.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://kd.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://na.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://lx.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mo.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://ep.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://kq.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gb.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pe.521024.cn

Ruby: threads.map(&:join)
来源：http://td.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qw.jianghongdianzi.cn

[O06] 使用进程池
来源：http://tz.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tb.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xd.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://rx.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ky.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vv.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sj.bjjhwx.cn

Ruby: // fork 块
来源：http://cq.chemitech.net.cn

C#:   Parallel.For
来源：http://dp.newstarts.cn

================================================================================
来源：http://km.521024.cn

P. 常用工具函数
来源：http://gf.lnxyls.cn

================================================================================
来源：http://he.shxzukj.cn

[P01] 生成 UUID
来源：http://eu.colortex.cn

Py:   str(uuid.uuid4())
来源：http://ww.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://om.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://cl.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://nc.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://nk.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://bp.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://ss.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://wk.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://py.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://id.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lh.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ux.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bt.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yu.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dt.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zu.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xe.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://pw.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pk.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zs.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bj.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ai.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zx.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fo.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nb.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cc.szsharing.cn

[P04] 求长度
来源：http://gs.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://st.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sk.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rf.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zk.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://aq.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://fn.shxzukj.cn

Ruby: x.length;  x.size
来源：http://ra.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ej.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://as.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dk.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zq.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ls.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wg.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qa.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uv.huixinmuqiang.cn

Ruby: a == b
来源：http://dn.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uj.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ue.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xa.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://cu.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jz.szxytkj.cn

TS:   if (x == null) {}
来源：http://ng.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yk.jctech888.com.cn

Go:   if x == nil {}
来源：http://sv.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jr.haigaiapp.cn

C#:   if (x is null) {}
来源：http://nr.lnxyls.cn

[P07] 防抖与节流
来源：http://dy.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://of.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://su.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ko.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cu.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mk.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yr.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bd.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://sc.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hh.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xe.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qg.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ty.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pf.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gt.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eb.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vm.yuexingan06.cn

================================================================================
来源：http://rf.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xj.9csxet.cn

================================================================================
来源：http://cx.gzmigu.cn

[Q01] 创建表
来源：http://ao.jianghongdianzi.cn

CREATE TABLE users (
来源：http://gq.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mv.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://xe.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://oa.wgjwhj.cn


<!-- 参考信息 -->