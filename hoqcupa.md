代发 wailian999

Ruby: ARGV
来源：http://qa.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://rs.szxytkj.cn

[M02] 读取环境变量
来源：http://fk.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://gz.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rs.nicolike.cn

JS:   process.env.HOME
来源：http://qz.hahajie.cn

TS:   process.env.HOME
来源：http://eu.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://ty.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tq.newstarts.cn

Ruby: ENV["HOME"]
来源：http://nu.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hb.hnjuh.cn

[M03] 执行外部命令
来源：http://yx.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ei.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yn.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oi.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yp.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cw.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mu.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vb.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://jb.gzmigu.cn

[M04] 获取当前工作目录
来源：http://hu.huanxung.cn

Py:   os.getcwd()
来源：http://mq.huanxung.cn

PHP:  getcwd();
来源：http://en.yuexingan06.cn

JS:   process.cwd()
来源：http://ck.lnxyls.cn

TS:   process.cwd()
来源：http://iz.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://zi.nszjky.cn

Go:   os.Getwd()
来源：http://kk.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ri.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tb.yuexingan06.cn

[M05] 设置退出码
来源：http://cb.nszjky.cn

Py:   sys.exit(1)
来源：http://bx.521024.cn

PHP:  exit(1);
来源：http://km.colortex.cn

JS:   process.exit(1)
来源：http://oy.nszjky.cn

TS:   process.exit(1)
来源：http://nb.hahajie.cn

Java: System.exit(1)
来源：http://et.szsharing.cn

Go:   os.Exit(1)
来源：http://ub.9csxet.cn

Ruby: exit 1
来源：http://lg.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://im.szsharing.cn

[M06] 向标准错误输出
来源：http://pp.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://tp.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vb.yuntaijiaju.cn

JS:   console.error("err")
来源：http://dq.huixiangedu.cn

TS:   console.error("err")
来源：http://xo.huixiangedu.cn

Java: System.err.println("err")
来源：http://zg.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yl.colortex.cn

Ruby: warn "err"
来源：http://nm.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://md.shxzukj.cn

[M07] 判断是否为主入口
来源：http://qr.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://qe.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mt.hnjuh.cn

JS:   require.main === module
来源：http://dy.521024.cn

TS:   require.main === module
来源：http://po.szsharing.cn

Java: public static void main(String[] args)
来源：http://jn.jianghongdianzi.cn

Go:   func main()
来源：http://xg.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zn.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://zi.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://pk.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://ct.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://tm.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://tn.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://ne.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zs.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oe.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oz.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iy.bjjhwx.cn

================================================================================
来源：http://ap.521024.cn

N. 数据结构与算法
来源：http://vf.huixiangedu.cn

================================================================================
来源：http://dg.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://cz.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cn.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vf.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gg.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nu.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ul.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://xx.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ub.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rk.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://fi.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://kc.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jw.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ru.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jm.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wu.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://nb.huanxung.cn

Ruby: arr.sort
来源：http://vr.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sr.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://dp.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://er.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://tk.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cx.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dn.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dy.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://by.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://be.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ug.panjiajie.cn

[N04] 斐波那契数列
来源：http://ls.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://so.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hm.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xm.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yq.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ol.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://br.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vg.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iu.muxihuayi.cn

[N05] 最大公约数
来源：http://zy.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://uu.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://an.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jg.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uo.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zi.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wt.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://re.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sw.wgjwhj.cn

[N06] 判断回文字符串
来源：http://oj.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://tz.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://mn.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://tz.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://cf.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lh.newstarts.cn

Go:   // 双指针从两端比较
来源：http://fk.colortex.cn

Ruby: s == s.reverse
来源：http://cl.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nc.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://kg.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ay.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yh.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ug.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://mi.shxzukj.cn

Java: // 手写 HashMap
来源：http://rk.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://vz.newstarts.cn

Ruby: // 手写 Hash
来源：http://ns.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uz.panjiajie.cn

[N08] 生成全排列
来源：http://ez.521024.cn

Py:   itertools.permutations(arr)
来源：http://kl.asd995.cn

PHP:  // 手写递归交换
来源：http://dk.szsharing.cn

JS:   // 手写回溯递归
来源：http://di.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://vc.nszjky.cn

Java: // 手写回溯递归
来源：http://oj.panjiajie.cn

Go:   // 手写回溯递归
来源：http://cv.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://nu.nicolike.cn

C#:   // 手写回溯递归
来源：http://xa.521024.cn

[N09] 栈与队列
来源：http://jp.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gz.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nq.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ep.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ey.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ad.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://al.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://av.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qn.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://zf.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://io.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pa.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lo.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pw.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://vu.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lu.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gj.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yw.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://mb.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ym.lnxyls.cn

PHP:  // 手写递归函数
来源：http://br.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ln.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fi.panjiajie.cn

Java: // 手写递归
来源：http://dj.chemitech.net.cn

Go:   // 手写递归
来源：http://vn.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uc.bjjhwx.cn

C#:   // 手写递归
来源：http://mk.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tf.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mk.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hr.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lz.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ey.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mu.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ki.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.bookmarksfly.cn

================================================================================
来源：http://ei.9csxet.cn

O. 并发与异步
来源：http://ci.nszjky.cn

================================================================================
来源：http://hi.haigaiapp.cn

[O01] 启动一个线程
来源：http://tf.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ib.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rn.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ye.hahajie.cn

TS:   // 同 JS
来源：http://me.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://yg.lnxyls.cn

Go:   go f()
来源：http://jj.panjiajie.cn

Ruby: Thread.new { f }
来源：http://mk.hahajie.cn

C#:   Task.Run(() => F());
来源：http://na.bjjhwx.cn

[O02] 使用线程池
来源：http://wi.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://co.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gc.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://dm.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://em.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kx.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fq.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mu.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pu.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://ze.nicolike.cn

Py:   with lock: shared += 1
来源：http://es.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://wr.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://va.gzmigu.cn

TS:   // 同 JS
来源：http://en.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://hj.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eo.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rp.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://fq.nszjky.cn

[O04] 定义异步函数并等待
来源：http://iq.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://pz.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zq.newstarts.cn

JS:   async function f() { await g(); }
来源：http://jh.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vt.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vd.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://va.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hd.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://dg.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://zb.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://zl.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ii.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://yh.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://gh.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qz.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aw.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://kx.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://si.hahajie.cn

[O06] 使用进程池
来源：http://dt.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ec.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gt.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://up.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://cj.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://co.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iw.chemitech.net.cn

Ruby: // fork 块
来源：http://hy.hnjuh.cn

C#:   Parallel.For
来源：http://zl.521024.cn

================================================================================
来源：http://ev.shxzskj.cn

P. 常用工具函数
来源：http://po.gzmigu.cn

================================================================================
来源：http://qs.muxihuayi.cn

[P01] 生成 UUID
来源：http://fa.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://pz.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vq.9csxet.cn

JS:   crypto.randomUUID()
来源：http://vh.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://gw.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://tr.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://lk.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://hp.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://av.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://cf.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kg.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://al.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ks.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tg.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rw.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fs.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cx.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zs.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://za.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fx.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sv.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://og.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sq.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kz.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tr.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ea.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ph.wgjwhj.cn

[P04] 求长度
来源：http://wr.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zw.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ob.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ew.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gi.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://nq.nicolike.cn

Go:   len(arr);  len(m)
来源：http://mn.newstarts.cn

Ruby: x.length;  x.size
来源：http://zd.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zl.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://jt.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ut.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yo.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xr.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sp.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sg.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xo.szsharing.cn

Ruby: a == b
来源：http://dz.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rn.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zp.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hs.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://fh.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ez.shtwfgs.cn

TS:   if (x == null) {}
来源：http://in.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kr.haigaiapp.cn

Go:   if x == nil {}
来源：http://up.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yr.chemitech.net.cn

C#:   if (x is null) {}
来源：http://zp.yuexingan06.cn

[P07] 防抖与节流
来源：http://xd.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ui.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://rx.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eu.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xk.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eg.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://to.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xj.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ts.521024.cn

[P08] 处理浮点精度问题
来源：http://fs.nszjky.cn


<!-- 参考信息 -->