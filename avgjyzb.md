代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xo.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://hk.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://py.panjiajie.cn

[M03] 执行外部命令
来源：http://rb.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pg.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mz.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eg.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cb.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rg.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dp.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gp.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://lg.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://yp.bjjhwx.cn

Py:   os.getcwd()
来源：http://pe.nicolike.cn

PHP:  getcwd();
来源：http://wv.asd995.cn

JS:   process.cwd()
来源：http://aa.jctech888.com.cn

TS:   process.cwd()
来源：http://rg.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://jw.bookmarksfly.cn

Go:   os.Getwd()
来源：http://cp.hahajie.cn

Ruby: Dir.pwd
来源：http://vr.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://au.chemitech.net.cn

[M05] 设置退出码
来源：http://ak.huanxung.cn

Py:   sys.exit(1)
来源：http://bs.huixinmuqiang.cn

PHP:  exit(1);
来源：http://zm.yuexingan06.cn

JS:   process.exit(1)
来源：http://sx.szxytkj.cn

TS:   process.exit(1)
来源：http://gt.wgjwhj.cn

Java: System.exit(1)
来源：http://kr.newstarts.cn

Go:   os.Exit(1)
来源：http://hz.lnxyls.cn

Ruby: exit 1
来源：http://zx.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cc.hnjuh.cn

[M06] 向标准错误输出
来源：http://os.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://kk.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lw.yuntaijiaju.cn

JS:   console.error("err")
来源：http://uf.yuntaijiaju.cn

TS:   console.error("err")
来源：http://sf.szsharing.cn

Java: System.err.println("err")
来源：http://dk.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wz.jianghongdianzi.cn

Ruby: warn "err"
来源：http://nt.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://zo.huanxung.cn

[M07] 判断是否为主入口
来源：http://fx.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://rv.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xa.nszjky.cn

JS:   require.main === module
来源：http://ej.muxihuayi.cn

TS:   require.main === module
来源：http://uv.hahajie.cn

Java: public static void main(String[] args)
来源：http://kc.gzmigu.cn

Go:   func main()
来源：http://vt.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ro.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://cz.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://hj.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://be.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://jz.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://lw.shxzukj.cn

TS:   process.platform;  process.version
来源：http://vw.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mo.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wc.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wt.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vn.huixiangedu.cn

================================================================================
来源：http://bt.asd995.cn

N. 数据结构与算法
来源：http://mb.yuexingan06.cn

================================================================================
来源：http://yc.asd995.cn

[N01] 二分查找（有序数组）
来源：http://xc.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oz.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://my.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ud.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nn.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://nw.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cq.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ob.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://zc.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zm.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rw.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wa.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ju.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sb.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://us.huixiangedu.cn

Ruby: arr.sort
来源：http://om.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kg.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://py.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jv.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://rz.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ks.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qp.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ri.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aq.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eg.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ti.shxzskj.cn

[N04] 斐波那契数列
来源：http://ij.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dr.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gu.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pu.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oj.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qj.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mb.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wk.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ve.yuexingan06.cn

[N05] 最大公约数
来源：http://he.huanxung.cn

Py:   math.gcd(a, b)
来源：http://ke.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vs.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://av.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mr.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ns.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cd.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://uh.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://un.asd995.cn

[N06] 判断回文字符串
来源：http://mn.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://qr.nszjky.cn

PHP:  $s === strrev($s);
来源：http://cq.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://ew.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://xx.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sd.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://yz.asd995.cn

Ruby: s == s.reverse
来源：http://yz.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://es.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://hv.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://as.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ua.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://je.521024.cn

TS:   // 手写 Map<string, number>
来源：http://eg.wgjwhj.cn

Java: // 手写 HashMap
来源：http://tm.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://jj.nicolike.cn

Ruby: // 手写 Hash
来源：http://dr.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tx.huixiangedu.cn

[N08] 生成全排列
来源：http://sg.asd995.cn

Py:   itertools.permutations(arr)
来源：http://jj.newstarts.cn

PHP:  // 手写递归交换
来源：http://no.newstarts.cn

JS:   // 手写回溯递归
来源：http://sv.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://rs.szsharing.cn

Java: // 手写回溯递归
来源：http://rb.lnxyls.cn

Go:   // 手写回溯递归
来源：http://bz.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://nd.panjiajie.cn

C#:   // 手写回溯递归
来源：http://km.jianghongdianzi.cn

[N09] 栈与队列
来源：http://ne.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yk.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vj.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ln.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tf.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://un.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ta.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://li.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hs.colortex.cn

[N10] 链表节点定义
来源：http://bf.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jn.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tv.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wh.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uc.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://gf.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ot.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iz.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vl.nicolike.cn

[N11] 二叉树中序遍历
来源：http://xu.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pu.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://ee.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://je.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mf.jianghongdianzi.cn

Java: // 手写递归
来源：http://wr.asd995.cn

Go:   // 手写递归
来源：http://uw.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oj.szsharing.cn

C#:   // 手写递归
来源：http://qf.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wm.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yy.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xm.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nm.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gl.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fl.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sp.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xs.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jx.colortex.cn

================================================================================
来源：http://dh.wgjwhj.cn

O. 并发与异步
来源：http://iy.hnjuh.cn

================================================================================
来源：http://ro.shxzskj.cn

[O01] 启动一个线程
来源：http://dk.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ha.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aa.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://li.shxzukj.cn

TS:   // 同 JS
来源：http://zh.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://gy.wgjwhj.cn

Go:   go f()
来源：http://tr.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://jj.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://kf.shtwfgs.cn

[O02] 使用线程池
来源：http://yr.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://no.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rt.szsharing.cn

JS:   // worker_threads 线程池
来源：http://tp.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://ht.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hv.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://no.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xa.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bs.nszjky.cn

[O03] 加锁保护共享数据
来源：http://az.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://gz.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://xd.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dh.gzmigu.cn

TS:   // 同 JS
来源：http://xe.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://tz.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ie.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cj.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://xw.hahajie.cn

[O04] 定义异步函数并等待
来源：http://my.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://jb.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://us.nicolike.cn

JS:   async function f() { await g(); }
来源：http://vv.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ex.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dz.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hp.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pz.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://dp.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://jm.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://gw.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qe.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://sm.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://bo.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://om.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gc.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://hd.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eq.shtwfgs.cn

[O06] 使用进程池
来源：http://eg.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jt.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cn.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://xl.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://by.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rf.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rs.colortex.cn

Ruby: // fork 块
来源：http://nx.hahajie.cn

C#:   Parallel.For
来源：http://ot.newstarts.cn

================================================================================
来源：http://ig.hnjuh.cn

P. 常用工具函数
来源：http://fe.newstarts.cn

================================================================================
来源：http://mk.lnxyls.cn

[P01] 生成 UUID
来源：http://kh.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://dy.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://re.huanxung.cn

JS:   crypto.randomUUID()
来源：http://wv.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://hx.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://hk.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://jx.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://jv.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://lw.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://zi.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ye.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qz.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fd.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://et.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kk.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ys.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gv.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kk.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://gn.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iv.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jo.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lz.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ie.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mc.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nu.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xl.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fd.9csxet.cn

[P04] 求长度
来源：http://qv.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ho.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://np.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ha.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xu.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://hx.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://gj.9csxet.cn

Ruby: x.length;  x.size
来源：http://qc.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xd.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://dl.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qn.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ox.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qm.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eh.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lr.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gk.shxzskj.cn

Ruby: a == b
来源：http://ci.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zy.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kq.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sc.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://sn.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kh.shxzukj.cn

TS:   if (x == null) {}
来源：http://zm.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tl.shxzskj.cn

Go:   if x == nil {}
来源：http://jc.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rz.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://jz.9csxet.cn

[P07] 防抖与节流
来源：http://mk.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kj.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://qp.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ip.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pr.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ia.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bs.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iw.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nx.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://cu.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ai.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ee.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zb.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kc.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zg.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lj.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mf.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ik.asd995.cn


<!-- 参考信息 -->