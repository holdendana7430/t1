代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xu.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://az.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dj.asd995.cn

[M03] 执行外部命令
来源：http://xt.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xw.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ua.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ev.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://op.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fl.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jr.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bz.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://gy.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://sq.szsharing.cn

Py:   os.getcwd()
来源：http://ml.shtwfgs.cn

PHP:  getcwd();
来源：http://jj.huixinmuqiang.cn

JS:   process.cwd()
来源：http://nv.shxzskj.cn

TS:   process.cwd()
来源：http://ff.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://iq.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://op.asd995.cn

Ruby: Dir.pwd
来源：http://vc.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://op.gzmigu.cn

[M05] 设置退出码
来源：http://ih.lnxyls.cn

Py:   sys.exit(1)
来源：http://lr.chemitech.net.cn

PHP:  exit(1);
来源：http://zt.9csxet.cn

JS:   process.exit(1)
来源：http://ko.shxzskj.cn

TS:   process.exit(1)
来源：http://vf.colortex.cn

Java: System.exit(1)
来源：http://cq.panjiajie.cn

Go:   os.Exit(1)
来源：http://qk.shxzukj.cn

Ruby: exit 1
来源：http://tr.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uh.jctech888.com.cn

[M06] 向标准错误输出
来源：http://bz.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://rz.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pe.hahajie.cn

JS:   console.error("err")
来源：http://it.bjjhwx.cn

TS:   console.error("err")
来源：http://ue.bookmarksfly.cn

Java: System.err.println("err")
来源：http://gu.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yt.hnjuh.cn

Ruby: warn "err"
来源：http://og.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ot.hnjuh.cn

[M07] 判断是否为主入口
来源：http://vq.521024.cn

Py:   if __name__ == "__main__":
来源：http://zb.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xi.gzmigu.cn

JS:   require.main === module
来源：http://ui.521024.cn

TS:   require.main === module
来源：http://ab.newstarts.cn

Java: public static void main(String[] args)
来源：http://at.jctech888.com.cn

Go:   func main()
来源：http://im.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gl.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://dy.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://xv.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://yr.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://wn.newstarts.cn

JS:   process.platform;  process.version
来源：http://ht.hahajie.cn

TS:   process.platform;  process.version
来源：http://dk.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://os.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pv.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dt.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pv.lnxyls.cn

================================================================================
来源：http://hs.muxihuayi.cn

N. 数据结构与算法
来源：http://ok.haigaiapp.cn

================================================================================
来源：http://mw.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://gd.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dm.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vi.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cu.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eu.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ir.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://js.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rs.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ff.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://ee.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://bu.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gj.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ix.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oe.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ht.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://gv.lnxyls.cn

Ruby: arr.sort
来源：http://ti.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jh.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://dl.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://te.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://uh.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yc.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kp.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ai.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ox.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://os.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dz.nszjky.cn

[N04] 斐波那契数列
来源：http://jh.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bw.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kw.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wo.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bg.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mo.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ks.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sw.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bk.panjiajie.cn

[N05] 最大公约数
来源：http://cg.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://vt.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rj.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qr.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sb.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lg.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pj.hnjuh.cn

Ruby: a.gcd(b)
来源：http://qg.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vp.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://me.hahajie.cn

Py:   s == s[::-1]
来源：http://se.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://ks.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://ib.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://fd.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yq.asd995.cn

Go:   // 双指针从两端比较
来源：http://mt.haigaiapp.cn

Ruby: s == s.reverse
来源：http://wq.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pb.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://yj.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fi.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aa.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fj.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://tq.shxzukj.cn

Java: // 手写 HashMap
来源：http://dk.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://rb.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://xp.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ld.nicolike.cn

[N08] 生成全排列
来源：http://ph.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://vf.huanxung.cn

PHP:  // 手写递归交换
来源：http://je.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://bv.9csxet.cn

TS:   // 手写回溯递归
来源：http://go.chemitech.net.cn

Java: // 手写回溯递归
来源：http://jm.panjiajie.cn

Go:   // 手写回溯递归
来源：http://wz.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ru.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://fa.colortex.cn

[N09] 栈与队列
来源：http://fs.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zh.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vo.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yt.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nn.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lr.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://na.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nt.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xs.hahajie.cn

[N10] 链表节点定义
来源：http://bf.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vn.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://un.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xp.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ux.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://sh.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sb.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kn.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fc.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://wp.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://to.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ca.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ru.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qm.asd995.cn

Java: // 手写递归
来源：http://ge.jctech888.com.cn

Go:   // 手写递归
来源：http://ai.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bd.jctech888.com.cn

C#:   // 手写递归
来源：http://wr.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xg.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://te.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nr.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vc.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nu.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wf.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rr.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kq.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sc.521024.cn

================================================================================
来源：http://wp.521024.cn

O. 并发与异步
来源：http://py.521024.cn

================================================================================
来源：http://vx.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://xk.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xa.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ne.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yz.nszjky.cn

TS:   // 同 JS
来源：http://dy.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://jb.colortex.cn

Go:   go f()
来源：http://jl.lnxyls.cn

Ruby: Thread.new { f }
来源：http://wg.colortex.cn

C#:   Task.Run(() => F());
来源：http://na.huanxung.cn

[O02] 使用线程池
来源：http://rk.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fh.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sa.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ho.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://yr.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ay.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yf.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lg.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gf.szsharing.cn

[O03] 加锁保护共享数据
来源：http://ln.9csxet.cn

Py:   with lock: shared += 1
来源：http://wo.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://jj.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ga.chemitech.net.cn

TS:   // 同 JS
来源：http://pi.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://th.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xv.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ke.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://oj.nszjky.cn

[O04] 定义异步函数并等待
来源：http://yc.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://wt.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uj.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://og.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bq.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ve.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hv.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gi.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://wz.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ed.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ol.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gs.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://qa.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://tk.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rg.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qz.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://wt.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qb.bjjhwx.cn

[O06] 使用进程池
来源：http://xi.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yj.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jk.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://kz.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://li.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://te.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mc.yuntaijiaju.cn

Ruby: // fork 块
来源：http://rr.newstarts.cn

C#:   Parallel.For
来源：http://po.shtwfgs.cn

================================================================================
来源：http://ay.hnjuh.cn

P. 常用工具函数
来源：http://uf.huixinmuqiang.cn

================================================================================
来源：http://ot.muxihuayi.cn

[P01] 生成 UUID
来源：http://ze.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://iy.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xt.newstarts.cn

JS:   crypto.randomUUID()
来源：http://ca.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://xn.521024.cn

Java: UUID.randomUUID().toString()
来源：http://bi.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://qy.asd995.cn

Ruby: SecureRandom.uuid
来源：http://gv.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://dd.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://uy.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ad.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vi.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bs.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ko.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cu.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://po.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jy.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fd.szxytkj.cn

[P03] 生成短随机字符串
来源：http://ap.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dz.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ef.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lk.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iz.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fb.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tm.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mk.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ng.lnxyls.cn

[P04] 求长度
来源：http://ac.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pz.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ln.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ae.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vw.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://nt.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://nc.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ts.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hq.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://rv.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cn.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zj.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pq.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ji.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mj.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hm.szsharing.cn

Ruby: a == b
来源：http://nh.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://be.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ar.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bc.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://pq.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dh.shxzskj.cn

TS:   if (x == null) {}
来源：http://lz.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xe.yuexingan06.cn

Go:   if x == nil {}
来源：http://na.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sd.9csxet.cn

C#:   if (x is null) {}
来源：http://uy.asd995.cn

[P07] 防抖与节流
来源：http://zj.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wf.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://qg.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://be.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://to.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://er.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jj.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dm.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rw.hahajie.cn

[P08] 处理浮点精度问题
来源：http://jr.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ca.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dw.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qc.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yi.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://am.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jg.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vi.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ng.gzmigu.cn


<!-- 参考信息 -->