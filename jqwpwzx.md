代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sg.nszjky.cn

Ruby: ENV["HOME"]
来源：http://zs.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tn.muxihuayi.cn

[M03] 执行外部命令
来源：http://jy.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ii.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oj.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qd.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jo.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sx.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bz.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hf.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://ea.panjiajie.cn

[M04] 获取当前工作目录
来源：http://ie.shxzskj.cn

Py:   os.getcwd()
来源：http://vr.yuexingan06.cn

PHP:  getcwd();
来源：http://ob.panjiajie.cn

JS:   process.cwd()
来源：http://ny.shxzskj.cn

TS:   process.cwd()
来源：http://ft.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://hq.yuexingan06.cn

Go:   os.Getwd()
来源：http://yj.nszjky.cn

Ruby: Dir.pwd
来源：http://fp.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nm.colortex.cn

[M05] 设置退出码
来源：http://nv.jctech888.com.cn

Py:   sys.exit(1)
来源：http://ik.shxzukj.cn

PHP:  exit(1);
来源：http://nj.9csxet.cn

JS:   process.exit(1)
来源：http://ey.szxytkj.cn

TS:   process.exit(1)
来源：http://io.muxihuayi.cn

Java: System.exit(1)
来源：http://jv.newstarts.cn

Go:   os.Exit(1)
来源：http://oe.521024.cn

Ruby: exit 1
来源：http://sy.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wk.9csxet.cn

[M06] 向标准错误输出
来源：http://tw.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yg.bookmarksfly.cn

JS:   console.error("err")
来源：http://ip.bjjhwx.cn

TS:   console.error("err")
来源：http://ev.szxytkj.cn

Java: System.err.println("err")
来源：http://tn.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ht.hnjuh.cn

Ruby: warn "err"
来源：http://of.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://vm.szxytkj.cn

[M07] 判断是否为主入口
来源：http://xk.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://st.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cy.huixiangedu.cn

JS:   require.main === module
来源：http://fo.newstarts.cn

TS:   require.main === module
来源：http://oe.nszjky.cn

Java: public static void main(String[] args)
来源：http://ta.szxytkj.cn

Go:   func main()
来源：http://ru.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lw.521024.cn

C#:   static void Main(string[] args)
来源：http://ia.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://mm.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://bx.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://yq.shxzskj.cn

JS:   process.platform;  process.version
来源：http://os.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://tf.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wg.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mm.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wu.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nt.hahajie.cn

================================================================================
来源：http://bv.colortex.cn

N. 数据结构与算法
来源：http://zo.colortex.cn

================================================================================
来源：http://ol.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://zp.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ry.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bw.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://su.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://so.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iu.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ro.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mo.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://go.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://vj.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://gf.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yv.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qk.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hc.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tg.newstarts.cn

Go:   slices.Sort(arr)
来源：http://la.9csxet.cn

Ruby: arr.sort
来源：http://tk.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hq.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://rt.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ss.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://oz.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ho.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ux.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rq.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ch.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gp.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dc.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://dp.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tl.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uu.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lb.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yc.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ud.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aa.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yc.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kn.muxihuayi.cn

[N05] 最大公约数
来源：http://at.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://be.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wn.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://va.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ib.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://br.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://bu.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zw.szxytkj.cn

[N06] 判断回文字符串
来源：http://lp.muxihuayi.cn

Py:   s == s[::-1]
来源：http://bw.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://kr.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://kp.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://xs.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jj.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://pp.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://fk.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://op.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://bh.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mt.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rn.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://he.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://cn.shxzukj.cn

Java: // 手写 HashMap
来源：http://ko.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ry.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://id.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jz.haigaiapp.cn

[N08] 生成全排列
来源：http://zc.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://bm.nszjky.cn

PHP:  // 手写递归交换
来源：http://gg.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://xe.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://eq.colortex.cn

Java: // 手写回溯递归
来源：http://vr.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://xu.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://hl.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://is.huixiangedu.cn

[N09] 栈与队列
来源：http://yn.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nf.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fx.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qp.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ts.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://di.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fg.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qs.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ex.jctech888.com.cn

[N10] 链表节点定义
来源：http://zj.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kl.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kx.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iv.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uk.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://sy.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vv.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://aw.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kk.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://tb.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bc.shxzukj.cn

PHP:  // 手写递归函数
来源：http://kg.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://is.9csxet.cn

Java: // 手写递归
来源：http://qr.panjiajie.cn

Go:   // 手写递归
来源：http://li.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hx.szxytkj.cn

C#:   // 手写递归
来源：http://cn.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qk.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://du.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bg.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gw.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kl.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ig.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pk.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ve.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lx.shxzskj.cn

================================================================================
来源：http://nx.9csxet.cn

O. 并发与异步
来源：http://xq.yuntaijiaju.cn

================================================================================
来源：http://xo.hahajie.cn

[O01] 启动一个线程
来源：http://kc.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bj.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zv.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cm.huixiangedu.cn

TS:   // 同 JS
来源：http://wu.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://zl.yuexingan06.cn

Go:   go f()
来源：http://nh.asd995.cn

Ruby: Thread.new { f }
来源：http://gi.szsharing.cn

C#:   Task.Run(() => F());
来源：http://si.panjiajie.cn

[O02] 使用线程池
来源：http://tt.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bh.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://va.colortex.cn

JS:   // worker_threads 线程池
来源：http://cl.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://ay.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oz.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pq.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://az.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hn.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ho.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://yx.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://pz.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xj.jianghongdianzi.cn

TS:   // 同 JS
来源：http://xj.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://bq.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lj.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mr.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://dz.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ne.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://vl.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eb.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://ic.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://je.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rq.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lb.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wo.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://jp.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://pm.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://jx.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xc.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://rb.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://dq.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ot.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oo.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ky.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gh.shxzukj.cn

[O06] 使用进程池
来源：http://nl.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wy.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://an.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://dv.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://kh.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jw.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fy.shxzukj.cn

Ruby: // fork 块
来源：http://ff.9csxet.cn

C#:   Parallel.For
来源：http://pb.chemitech.net.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

P. 常用工具函数
来源：http://mr.hnjuh.cn

================================================================================
来源：http://tq.jctech888.com.cn

[P01] 生成 UUID
来源：http://rs.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ts.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ua.colortex.cn

JS:   crypto.randomUUID()
来源：http://gx.szsharing.cn

TS:   crypto.randomUUID()
来源：http://zf.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://gf.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://rd.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://nm.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://er.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://dx.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xs.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://us.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mx.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hf.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oq.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zm.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://re.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ce.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://dk.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ye.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bx.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yw.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nw.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://id.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hd.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lu.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lo.haigaiapp.cn

[P04] 求长度
来源：http://ry.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://di.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tc.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rg.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://ul.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://sg.nszjky.cn

Ruby: x.length;  x.size
来源：http://wx.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wr.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://pb.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uq.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ow.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hx.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kb.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mb.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fp.panjiajie.cn

Ruby: a == b
来源：http://su.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wc.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qm.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rw.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://mk.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lj.haigaiapp.cn

TS:   if (x == null) {}
来源：http://th.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xt.bjjhwx.cn

Go:   if x == nil {}
来源：http://gg.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://un.colortex.cn

C#:   if (x is null) {}
来源：http://me.panjiajie.cn

[P07] 防抖与节流
来源：http://ng.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qh.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://rr.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cn.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://in.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gp.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://au.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yo.colortex.cn

[P08] 处理浮点精度问题
来源：http://lg.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zj.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iv.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://on.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xa.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ff.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nq.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hc.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kk.colortex.cn


<!-- 参考信息 -->