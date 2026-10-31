代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ov.521024.cn

JS:   process.env.HOME
来源：http://wp.newstarts.cn

TS:   process.env.HOME
来源：http://bn.9csxet.cn

Java: System.getenv("HOME")
来源：http://uu.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pq.hahajie.cn

Ruby: ENV["HOME"]
来源：http://dm.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bb.bookmarksfly.cn

[M03] 执行外部命令
来源：http://ux.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oc.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pt.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zs.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aq.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yg.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wh.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ob.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://vn.newstarts.cn

[M04] 获取当前工作目录
来源：http://tg.newstarts.cn

Py:   os.getcwd()
来源：http://st.nszjky.cn

PHP:  getcwd();
来源：http://bt.newstarts.cn

JS:   process.cwd()
来源：http://yt.szsharing.cn

TS:   process.cwd()
来源：http://dm.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://yj.szxytkj.cn

Go:   os.Getwd()
来源：http://zh.huixiangedu.cn

Ruby: Dir.pwd
来源：http://yc.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mc.shxzukj.cn

[M05] 设置退出码
来源：http://ga.shtwfgs.cn

Py:   sys.exit(1)
来源：http://tt.jianghongdianzi.cn

PHP:  exit(1);
来源：http://si.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://dz.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://hh.yuntaijiaju.cn

Java: System.exit(1)
来源：http://cb.szxytkj.cn

Go:   os.Exit(1)
来源：http://yg.huanxung.cn

Ruby: exit 1
来源：http://pk.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rz.nszjky.cn

[M06] 向标准错误输出
来源：http://gz.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://vz.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bc.bjjhwx.cn

JS:   console.error("err")
来源：http://xd.asd995.cn

TS:   console.error("err")
来源：http://vz.lnxyls.cn

Java: System.err.println("err")
来源：http://hl.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zo.shtwfgs.cn

Ruby: warn "err"
来源：http://rg.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://qo.szsharing.cn

[M07] 判断是否为主入口
来源：http://wa.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://sj.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://th.yuntaijiaju.cn

JS:   require.main === module
来源：http://qz.nicolike.cn

TS:   require.main === module
来源：http://tk.newstarts.cn

Java: public static void main(String[] args)
来源：http://ee.newstarts.cn

Go:   func main()
来源：http://jh.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://on.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://ii.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ie.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://gy.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://ej.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://rj.lnxyls.cn

TS:   process.platform;  process.version
来源：http://fs.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qa.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hf.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eh.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yz.szsharing.cn

================================================================================
来源：http://df.huixiangedu.cn

N. 数据结构与算法
来源：http://sb.shtwfgs.cn

================================================================================
来源：http://vw.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://cb.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bc.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yt.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zl.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dq.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yp.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://tf.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cg.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ss.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://my.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://fg.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nq.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://be.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qy.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dy.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://nq.huixinmuqiang.cn

Ruby: arr.sort
来源：http://mb.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uh.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://ps.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nz.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://vy.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ps.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xv.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bk.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ah.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bv.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ux.521024.cn

[N04] 斐波那契数列
来源：http://xs.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ke.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uh.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://th.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hh.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nv.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hu.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bn.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://di.yuexingan06.cn

[N05] 最大公约数
来源：http://ms.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://xe.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ox.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uy.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fu.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pj.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://te.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://kv.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ur.gzmigu.cn

[N06] 判断回文字符串
来源：http://pv.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://ug.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://la.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://nh.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ko.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tx.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ji.colortex.cn

Ruby: s == s.reverse
来源：http://qn.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wu.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://sk.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://me.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gp.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gd.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://yb.jctech888.com.cn

Java: // 手写 HashMap
来源：http://zu.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://tx.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://oy.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hf.shtwfgs.cn

[N08] 生成全排列
来源：http://ig.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://lo.newstarts.cn

PHP:  // 手写递归交换
来源：http://op.szxytkj.cn

JS:   // 手写回溯递归
来源：http://gh.9csxet.cn

TS:   // 手写回溯递归
来源：http://aw.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://qq.nicolike.cn

Go:   // 手写回溯递归
来源：http://ig.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://ea.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://re.hnjuh.cn

[N09] 栈与队列
来源：http://op.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fc.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xl.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rl.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sp.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fx.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ov.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mk.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yi.haigaiapp.cn

[N10] 链表节点定义
来源：http://qf.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bx.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ty.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yo.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pf.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://xt.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hw.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mb.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xd.nszjky.cn

[N11] 二叉树中序遍历
来源：http://gp.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xr.521024.cn

PHP:  // 手写递归函数
来源：http://xj.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vx.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gd.nszjky.cn

Java: // 手写递归
来源：http://ln.asd995.cn

Go:   // 手写递归
来源：http://at.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://je.shtwfgs.cn

C#:   // 手写递归
来源：http://pd.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uz.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tu.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zt.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ov.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zk.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ao.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vc.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bn.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xu.nicolike.cn

================================================================================
来源：http://dp.huixinmuqiang.cn

O. 并发与异步
来源：http://te.shxzskj.cn

================================================================================
来源：http://ge.bookmarksfly.cn

[O01] 启动一个线程
来源：http://iz.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uz.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oq.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oe.shtwfgs.cn

TS:   // 同 JS
来源：http://cn.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://nv.yuntaijiaju.cn

Go:   go f()
来源：http://eu.9csxet.cn

Ruby: Thread.new { f }
来源：http://ty.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://yv.gzmigu.cn

[O02] 使用线程池
来源：http://tz.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kn.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rr.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ak.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://yv.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://je.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://al.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://he.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nt.huanxung.cn

[O03] 加锁保护共享数据
来源：http://du.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://mb.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://gz.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gw.szxytkj.cn

TS:   // 同 JS
来源：http://nv.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://kq.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bk.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pw.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://pq.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://qk.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://ic.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zc.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://sz.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zl.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wr.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oy.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bw.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://iu.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://jb.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://bo.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jk.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://rc.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://gz.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://er.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lh.521024.cn

Ruby: threads.map(&:join)
来源：http://on.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qb.shxzskj.cn

[O06] 使用进程池
来源：http://te.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://un.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eu.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://nz.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://xj.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bd.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ul.bjjhwx.cn

Ruby: // fork 块
来源：http://lc.muxihuayi.cn

C#:   Parallel.For
来源：http://ga.lnxyls.cn

================================================================================
来源：http://tu.yuntaijiaju.cn

P. 常用工具函数
来源：http://gu.521024.cn

================================================================================
来源：http://jg.lnxyls.cn

[P01] 生成 UUID
来源：http://mz.521024.cn

Py:   str(uuid.uuid4())
来源：http://rr.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://th.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://gm.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://up.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://xc.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://jq.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://qk.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ey.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://wp.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ds.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uo.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ic.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ow.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jt.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mg.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zf.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ar.hnjuh.cn

[P03] 生成短随机字符串
来源：http://os.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vt.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zy.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ik.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yk.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://or.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qb.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vg.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ij.szsharing.cn

[P04] 求长度
来源：http://ap.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uo.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xm.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gf.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ft.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://mb.hahajie.cn

Go:   len(arr);  len(m)
来源：http://an.newstarts.cn

Ruby: x.length;  x.size
来源：http://eh.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nk.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://qh.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hx.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fw.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jc.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iy.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fi.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ff.haigaiapp.cn

Ruby: a == b
来源：http://ue.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ip.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lz.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tt.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://ch.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uo.muxihuayi.cn

TS:   if (x == null) {}
来源：http://lf.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ar.wgjwhj.cn

Go:   if x == nil {}
来源：http://sz.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pw.lnxyls.cn

C#:   if (x is null) {}
来源：http://wp.wgjwhj.cn

[P07] 防抖与节流
来源：http://yk.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://me.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://lx.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hg.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cu.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ov.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://io.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mo.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hf.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://hb.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://da.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tt.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bf.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ly.bookmarksfly.cn


<!-- 参考信息 -->