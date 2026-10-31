代发 wailian999

Ruby: ARGV
来源：http://fe.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://zv.szsharing.cn

[M02] 读取环境变量
来源：http://he.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://or.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bc.chemitech.net.cn

JS:   process.env.HOME
来源：http://fm.nicolike.cn

TS:   process.env.HOME
来源：http://wz.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://kr.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ru.521024.cn

Ruby: ENV["HOME"]
来源：http://xl.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wn.szsharing.cn

[M03] 执行外部命令
来源：http://tw.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ay.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ea.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pv.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yi.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bg.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xi.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uh.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://an.szxytkj.cn

[M04] 获取当前工作目录
来源：http://gw.huanxung.cn

Py:   os.getcwd()
来源：http://cr.hahajie.cn

PHP:  getcwd();
来源：http://zy.chemitech.net.cn

JS:   process.cwd()
来源：http://ac.panjiajie.cn

TS:   process.cwd()
来源：http://xx.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://iq.521024.cn

Go:   os.Getwd()
来源：http://wx.newstarts.cn

Ruby: Dir.pwd
来源：http://yy.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aq.szsharing.cn

[M05] 设置退出码
来源：http://ex.wgjwhj.cn

Py:   sys.exit(1)
来源：http://ux.shtwfgs.cn

PHP:  exit(1);
来源：http://ve.gzmigu.cn

JS:   process.exit(1)
来源：http://fu.gzmigu.cn

TS:   process.exit(1)
来源：http://zf.yuexingan06.cn

Java: System.exit(1)
来源：http://hu.szxytkj.cn

Go:   os.Exit(1)
来源：http://cn.9csxet.cn

Ruby: exit 1
来源：http://tu.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pd.newstarts.cn

[M06] 向标准错误输出
来源：http://bg.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://sg.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ay.chemitech.net.cn

JS:   console.error("err")
来源：http://xq.shxzukj.cn

TS:   console.error("err")
来源：http://fr.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://tt.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cw.asd995.cn

Ruby: warn "err"
来源：http://bi.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://lu.hnjuh.cn

[M07] 判断是否为主入口
来源：http://nm.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://on.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qz.shxzskj.cn

JS:   require.main === module
来源：http://yg.hahajie.cn

TS:   require.main === module
来源：http://ou.lnxyls.cn

Java: public static void main(String[] args)
来源：http://vi.szsharing.cn

Go:   func main()
来源：http://li.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://af.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://cv.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://wb.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://ns.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://np.hahajie.cn

JS:   process.platform;  process.version
来源：http://ar.szsharing.cn

TS:   process.platform;  process.version
来源：http://ng.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ot.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qb.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mm.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wm.gzmigu.cn

================================================================================
来源：http://pz.huixiangedu.cn

N. 数据结构与算法
来源：http://rn.jctech888.com.cn

================================================================================
来源：http://mj.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://zi.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lc.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nv.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mz.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bz.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qp.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ta.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pi.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kc.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ui.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ub.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vi.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ou.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oq.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xj.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://aq.huanxung.cn

Ruby: arr.sort
来源：http://cp.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://on.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://kq.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gq.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://fv.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sf.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sy.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ub.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nt.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dk.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ub.521024.cn

[N04] 斐波那契数列
来源：http://zc.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cc.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rh.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vi.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bh.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xi.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oi.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cp.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xr.jianghongdianzi.cn

[N05] 最大公约数
来源：http://nk.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://pf.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bu.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ii.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mz.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sh.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ho.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ct.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://lc.hahajie.cn

Py:   s == s[::-1]
来源：http://ve.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://qf.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://sg.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://rq.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ce.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://ks.gzmigu.cn

Ruby: s == s.reverse
来源：http://nx.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ks.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://dn.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gw.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lk.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://go.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://dr.nszjky.cn

Java: // 手写 HashMap
来源：http://hh.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://yj.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ij.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ln.gzmigu.cn

[N08] 生成全排列
来源：http://jq.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://fa.hnjuh.cn

PHP:  // 手写递归交换
来源：http://ba.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://ua.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://uc.hnjuh.cn

Java: // 手写回溯递归
来源：http://ax.hahajie.cn

Go:   // 手写回溯递归
来源：http://jn.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://lf.asd995.cn

C#:   // 手写回溯递归
来源：http://in.nszjky.cn

[N09] 栈与队列
来源：http://yc.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fz.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ga.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vj.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wf.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rl.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://us.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ui.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fa.szsharing.cn

[N10] 链表节点定义
来源：http://al.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ca.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fp.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zf.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ka.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://tc.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bu.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fg.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uw.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://wo.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xi.gzmigu.cn

PHP:  // 手写递归函数
来源：http://ae.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yr.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rp.wgjwhj.cn

Java: // 手写递归
来源：http://iv.haigaiapp.cn

Go:   // 手写递归
来源：http://ab.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mo.huanxung.cn

C#:   // 手写递归
来源：http://oj.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lg.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ut.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yh.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ia.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ur.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ef.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uh.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jc.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oi.shxzskj.cn

================================================================================
来源：http://wn.muxihuayi.cn

O. 并发与异步
来源：http://xs.lnxyls.cn

================================================================================
来源：http://am.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://tk.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ld.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pn.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lz.shtwfgs.cn

TS:   // 同 JS
来源：http://wa.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://ym.asd995.cn

Go:   go f()
来源：http://sa.521024.cn

Ruby: Thread.new { f }
来源：http://cx.hahajie.cn

C#:   Task.Run(() => F());
来源：http://qr.wgjwhj.cn

[O02] 使用线程池
来源：http://ol.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://te.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rt.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://bw.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://or.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nj.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ud.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dq.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kx.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://da.shxzukj.cn

Py:   with lock: shared += 1
来源：http://gn.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://vu.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xj.chemitech.net.cn

TS:   // 同 JS
来源：http://ut.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://ww.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pm.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cq.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ci.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://yn.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://gt.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ij.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://pn.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ej.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mt.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zw.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ex.asd995.cn

C#:   async Task F() { await G(); }
来源：http://px.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://mq.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ar.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zv.asd995.cn

JS:   await Promise.all(tasks)
来源：http://el.asd995.cn

TS:   await Promise.all(tasks)
来源：http://tu.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wh.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://do.newstarts.cn

Ruby: threads.map(&:join)
来源：http://gn.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ei.nszjky.cn

[O06] 使用进程池
来源：http://vc.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jc.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://my.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://yn.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://lw.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sn.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ss.haigaiapp.cn

Ruby: // fork 块
来源：http://is.gzmigu.cn

C#:   Parallel.For
来源：http://iq.wgjwhj.cn

================================================================================
来源：http://ru.hahajie.cn

P. 常用工具函数
来源：http://zr.bjjhwx.cn

================================================================================
来源：http://gr.asd995.cn

[P01] 生成 UUID
来源：http://gc.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://if.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fs.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://ob.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://lw.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://if.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ub.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://sk.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://lf.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://dw.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://io.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vk.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://op.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rm.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qj.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cm.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oo.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nb.hahajie.cn

[P03] 生成短随机字符串
来源：http://ff.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ax.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gl.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kw.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://am.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tj.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fe.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ao.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jm.muxihuayi.cn

[P04] 求长度
来源：http://sr.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hm.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cq.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kw.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vi.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://zw.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://io.szxytkj.cn

Ruby: x.length;  x.size
来源：http://an.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cn.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ws.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ag.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ke.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gt.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qa.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ny.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ey.hahajie.cn

Ruby: a == b
来源：http://tr.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bh.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nk.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gj.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://un.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gu.colortex.cn

TS:   if (x == null) {}
来源：http://lf.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fs.shxzskj.cn

Go:   if x == nil {}
来源：http://ei.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xu.shtwfgs.cn

C#:   if (x is null) {}
来源：http://ro.wgjwhj.cn

[P07] 防抖与节流
来源：http://kk.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vx.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://fz.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pg.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://og.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ur.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ip.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://co.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ey.bjjhwx.cn


<!-- 参考信息 -->