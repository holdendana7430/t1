代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rh.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://nf.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wa.shtwfgs.cn

[M03] 执行外部命令
来源：http://mw.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lq.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xs.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oc.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pb.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://um.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vj.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jy.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://vt.asd995.cn

[M04] 获取当前工作目录
来源：http://db.asd995.cn

Py:   os.getcwd()
来源：http://ya.hahajie.cn

PHP:  getcwd();
来源：http://ky.yuntaijiaju.cn

JS:   process.cwd()
来源：http://yn.jctech888.com.cn

TS:   process.cwd()
来源：http://au.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yn.9csxet.cn

Go:   os.Getwd()
来源：http://qc.nicolike.cn

Ruby: Dir.pwd
来源：http://aa.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sp.asd995.cn

[M05] 设置退出码
来源：http://lp.huanxung.cn

Py:   sys.exit(1)
来源：http://wi.bjjhwx.cn

PHP:  exit(1);
来源：http://bu.jctech888.com.cn

JS:   process.exit(1)
来源：http://cs.shtwfgs.cn

TS:   process.exit(1)
来源：http://nl.gzmigu.cn

Java: System.exit(1)
来源：http://wr.huixiangedu.cn

Go:   os.Exit(1)
来源：http://qc.bookmarksfly.cn

Ruby: exit 1
来源：http://zk.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mk.521024.cn

[M06] 向标准错误输出
来源：http://kb.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://xt.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vo.jianghongdianzi.cn

JS:   console.error("err")
来源：http://qn.szxytkj.cn

TS:   console.error("err")
来源：http://ro.muxihuayi.cn

Java: System.err.println("err")
来源：http://qn.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sh.nicolike.cn

Ruby: warn "err"
来源：http://vq.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://vm.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://pu.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://na.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pq.jctech888.com.cn

JS:   require.main === module
来源：http://ku.huanxung.cn

TS:   require.main === module
来源：http://bm.nicolike.cn

Java: public static void main(String[] args)
来源：http://vm.muxihuayi.cn

Go:   func main()
来源：http://uj.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://te.521024.cn

C#:   static void Main(string[] args)
来源：http://bz.asd995.cn

[M08] 获取系统与运行时信息
来源：http://fr.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ns.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://vr.nicolike.cn

JS:   process.platform;  process.version
来源：http://ix.nszjky.cn

TS:   process.platform;  process.version
来源：http://qu.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ob.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ii.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wz.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bj.huixiangedu.cn

================================================================================
来源：http://jf.szsharing.cn

N. 数据结构与算法
来源：http://ax.muxihuayi.cn

================================================================================
来源：http://ig.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://ym.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oq.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xn.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://op.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qg.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rs.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://nh.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zp.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gz.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://tk.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xs.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rj.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hw.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yk.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://az.yuntaijiaju.cn

Ruby: arr.sort
来源：http://iy.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ic.521024.cn

[N03] 快速排序（分治示例）
来源：http://nr.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vh.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://uq.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cm.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eh.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ng.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rn.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://if.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jz.huixiangedu.cn

[N04] 斐波那契数列
来源：http://sj.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ke.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://al.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sr.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ae.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uf.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ln.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mm.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cw.9csxet.cn

[N05] 最大公约数
来源：http://gu.asd995.cn

Py:   math.gcd(a, b)
来源：http://ci.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rt.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jr.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sa.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bp.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ha.panjiajie.cn

Ruby: a.gcd(b)
来源：http://mq.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://am.shtwfgs.cn

[N06] 判断回文字符串
来源：http://bk.yuexingan06.cn

Py:   s == s[::-1]
来源：http://dq.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://nj.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://ah.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://fh.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zk.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://tc.nszjky.cn

Ruby: s == s.reverse
来源：http://rj.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pp.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://al.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dm.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wq.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hx.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://fc.nszjky.cn

Java: // 手写 HashMap
来源：http://yq.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://uf.521024.cn

Ruby: // 手写 Hash
来源：http://sq.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ir.jianghongdianzi.cn

[N08] 生成全排列
来源：http://sh.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://hl.nicolike.cn

PHP:  // 手写递归交换
来源：http://fw.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://qw.newstarts.cn

TS:   // 手写回溯递归
来源：http://id.muxihuayi.cn

Java: // 手写回溯递归
来源：http://ub.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://mu.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://zl.hahajie.cn

C#:   // 手写回溯递归
来源：http://hq.gzmigu.cn

[N09] 栈与队列
来源：http://ej.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rz.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://az.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sn.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rq.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://id.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hv.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qc.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ad.colortex.cn

[N10] 链表节点定义
来源：http://le.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jf.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iv.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vx.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lk.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://yy.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ds.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xx.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bg.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://mp.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jq.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://jx.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cg.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vk.nicolike.cn

Java: // 手写递归
来源：http://lt.szxytkj.cn

Go:   // 手写递归
来源：http://xk.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qg.gzmigu.cn

C#:   // 手写递归
来源：http://zw.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kd.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yn.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gb.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tq.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ml.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fy.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jf.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kt.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wf.huixiangedu.cn

================================================================================
来源：http://db.panjiajie.cn

O. 并发与异步
来源：http://kq.shtwfgs.cn

================================================================================
来源：http://ik.wgjwhj.cn

[O01] 启动一个线程
来源：http://ie.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hb.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://df.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ss.jianghongdianzi.cn

TS:   // 同 JS
来源：http://iw.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ng.shtwfgs.cn

Go:   go f()
来源：http://ta.hnjuh.cn

Ruby: Thread.new { f }
来源：http://cs.nicolike.cn

C#:   Task.Run(() => F());
来源：http://ro.shxzukj.cn

[O02] 使用线程池
来源：http://sp.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fo.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hb.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://uv.asd995.cn

TS:   // worker_threads 线程池
来源：http://jo.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lt.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ka.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pe.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ox.521024.cn

[O03] 加锁保护共享数据
来源：http://yc.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://yp.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://vg.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mx.jianghongdianzi.cn

TS:   // 同 JS
来源：http://yt.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://gl.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gk.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://by.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://oy.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ep.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://ap.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yq.newstarts.cn

JS:   async function f() { await g(); }
来源：http://zo.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qx.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ny.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wf.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://de.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://oy.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://di.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://nu.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ow.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://hy.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://lo.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uq.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bj.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://ft.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zn.shtwfgs.cn

[O06] 使用进程池
来源：http://ih.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tt.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hs.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://sp.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://xo.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ol.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ia.wgjwhj.cn

Ruby: // fork 块
来源：http://zf.gzmigu.cn

C#:   Parallel.For
来源：http://xu.szsharing.cn

================================================================================
来源：http://zf.521024.cn

P. 常用工具函数
来源：http://sb.jctech888.com.cn

================================================================================
来源：http://gv.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://yn.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://lh.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bl.szsharing.cn

JS:   crypto.randomUUID()
来源：http://ht.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://kc.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://fk.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://sd.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ee.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://nf.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://aq.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nv.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ke.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bz.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ym.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ux.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vy.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fu.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fl.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://jk.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vb.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nf.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tx.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://li.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kz.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ol.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://he.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://et.huixiangedu.cn

[P04] 求长度
来源：http://sf.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xw.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eb.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gs.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qk.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://xv.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://vi.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ca.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yl.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ob.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uj.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://up.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pr.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://my.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ys.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://th.colortex.cn

Ruby: a == b
来源：http://zy.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kg.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jd.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xm.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://qo.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jo.huixiangedu.cn

TS:   if (x == null) {}
来源：http://oh.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ze.huanxung.cn

Go:   if x == nil {}
来源：http://rl.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bv.hnjuh.cn

C#:   if (x is null) {}
来源：http://iz.nicolike.cn

[P07] 防抖与节流
来源：http://ei.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ii.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://oy.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dh.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zc.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://il.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://if.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yb.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://cm.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://po.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cz.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ka.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wx.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sq.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wf.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nj.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ja.shxzskj.cn


<!-- 参考信息 -->