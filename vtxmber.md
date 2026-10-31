代发 wailian999

Ruby: ARGV
来源：http://ol.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://mn.hnjuh.cn

[M02] 读取环境变量
来源：http://nu.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://yh.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dx.asd995.cn

JS:   process.env.HOME
来源：http://wb.asd995.cn

TS:   process.env.HOME
来源：http://ge.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ao.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xg.521024.cn

Ruby: ENV["HOME"]
来源：http://mb.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://za.bjjhwx.cn

[M03] 执行外部命令
来源：http://mv.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jr.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://of.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fs.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nh.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pi.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lj.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zq.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://jx.shxzukj.cn

[M04] 获取当前工作目录
来源：http://up.huixiangedu.cn

Py:   os.getcwd()
来源：http://os.9csxet.cn

PHP:  getcwd();
来源：http://eu.shxzukj.cn

JS:   process.cwd()
来源：http://uz.lnxyls.cn

TS:   process.cwd()
来源：http://kw.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://zm.yuexingan06.cn

Go:   os.Getwd()
来源：http://ln.521024.cn

Ruby: Dir.pwd
来源：http://vv.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://id.521024.cn

[M05] 设置退出码
来源：http://jb.wgjwhj.cn

Py:   sys.exit(1)
来源：http://sx.nicolike.cn

PHP:  exit(1);
来源：http://wf.lnxyls.cn

JS:   process.exit(1)
来源：http://cj.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://su.hahajie.cn

Java: System.exit(1)
来源：http://qf.colortex.cn

Go:   os.Exit(1)
来源：http://hh.szxytkj.cn

Ruby: exit 1
来源：http://pc.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zm.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://iw.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://zs.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ay.huixinmuqiang.cn

JS:   console.error("err")
来源：http://nk.gzmigu.cn

TS:   console.error("err")
来源：http://md.asd995.cn

Java: System.err.println("err")
来源：http://bw.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://em.szxytkj.cn

Ruby: warn "err"
来源：http://ad.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://og.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://eg.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://dt.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hy.bookmarksfly.cn

JS:   require.main === module
来源：http://ik.shxzukj.cn

TS:   require.main === module
来源：http://qo.9csxet.cn

Java: public static void main(String[] args)
来源：http://nr.wgjwhj.cn

Go:   func main()
来源：http://xv.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pz.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://qe.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://sz.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://rg.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://hq.huanxung.cn

JS:   process.platform;  process.version
来源：http://cb.521024.cn

TS:   process.platform;  process.version
来源：http://ff.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ad.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rq.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rn.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mi.jianghongdianzi.cn

================================================================================
来源：http://sd.yuexingan06.cn

N. 数据结构与算法
来源：http://kg.huixiangedu.cn

================================================================================
来源：http://ng.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://re.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jr.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ik.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ic.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bz.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vp.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://cv.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ch.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pk.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://dn.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://wk.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yo.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zc.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vv.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nh.hahajie.cn

Go:   slices.Sort(arr)
来源：http://zm.shtwfgs.cn

Ruby: arr.sort
来源：http://yb.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ie.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://nv.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bg.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://iv.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kk.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hp.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vk.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tf.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nk.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fg.huixiangedu.cn

[N04] 斐波那契数列
来源：http://gp.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tw.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vi.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gk.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lh.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://op.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ni.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://by.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eb.lnxyls.cn

[N05] 最大公约数
来源：http://rn.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://se.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zv.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yc.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tz.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://so.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yy.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://br.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zj.jctech888.com.cn

[N06] 判断回文字符串
来源：http://wa.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://oj.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://nm.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://rv.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://nk.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ew.nszjky.cn

Go:   // 双指针从两端比较
来源：http://uj.chemitech.net.cn

Ruby: s == s.reverse
来源：http://wk.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ii.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://ys.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://py.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hk.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dw.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://pd.521024.cn

Java: // 手写 HashMap
来源：http://ma.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://dw.shxzskj.cn

Ruby: // 手写 Hash
来源：http://pt.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dr.szsharing.cn

[N08] 生成全排列
来源：http://nd.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://fo.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://yz.huanxung.cn

JS:   // 手写回溯递归
来源：http://dz.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://gy.lnxyls.cn

Java: // 手写回溯递归
来源：http://sk.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://ma.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://nw.nicolike.cn

C#:   // 手写回溯递归
来源：http://ji.hnjuh.cn

[N09] 栈与队列
来源：http://km.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fh.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fl.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uv.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lw.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yz.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kn.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://id.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wj.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://pw.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yp.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ye.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tb.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rb.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://xc.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xp.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ip.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yl.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://vl.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wr.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://yy.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ls.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yb.yuntaijiaju.cn

Java: // 手写递归
来源：http://hu.newstarts.cn

Go:   // 手写递归
来源：http://lw.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bn.szsharing.cn

C#:   // 手写递归
来源：http://fd.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bs.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vl.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hr.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sx.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wk.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jf.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xa.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zj.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wu.jianghongdianzi.cn

================================================================================
来源：http://so.shtwfgs.cn

O. 并发与异步
来源：http://zx.hahajie.cn

================================================================================
来源：http://gv.9csxet.cn

[O01] 启动一个线程
来源：http://wb.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ng.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://se.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fk.muxihuayi.cn

TS:   // 同 JS
来源：http://aq.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://bf.nicolike.cn

Go:   go f()
来源：http://uo.newstarts.cn

Ruby: Thread.new { f }
来源：http://lc.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://mf.wgjwhj.cn

[O02] 使用线程池
来源：http://ce.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ko.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hf.9csxet.cn

JS:   // worker_threads 线程池
来源：http://js.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://rk.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hm.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bq.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ll.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://of.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://zl.asd995.cn

Py:   with lock: shared += 1
来源：http://ft.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://hp.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yh.asd995.cn

TS:   // 同 JS
来源：http://wh.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://hr.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ip.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fn.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://dj.nszjky.cn

[O04] 定义异步函数并等待
来源：http://gh.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://xt.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iy.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://ri.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://km.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vh.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zw.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zz.asd995.cn

C#:   async Task F() { await G(); }
来源：http://vk.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://ep.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://gy.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ed.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://et.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://wp.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gj.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vt.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://gv.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qp.yuntaijiaju.cn

[O06] 使用进程池
来源：http://ma.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zg.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pk.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://mk.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://hu.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jw.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vy.huanxung.cn

Ruby: // fork 块
来源：http://bq.wgjwhj.cn

C#:   Parallel.For
来源：http://rk.bookmarksfly.cn

================================================================================
来源：http://pn.asd995.cn

P. 常用工具函数
来源：http://xe.colortex.cn

================================================================================
来源：http://te.bookmarksfly.cn

[P01] 生成 UUID
来源：http://pu.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://up.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wa.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://tb.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://ua.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://sh.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://af.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://nj.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://zc.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://vb.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fl.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oo.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hv.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zk.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oj.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kf.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vy.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xh.nicolike.cn

[P03] 生成短随机字符串
来源：http://km.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tx.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://so.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ar.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tj.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ok.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qc.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gq.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fe.yuexingan06.cn

[P04] 求长度
来源：http://et.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rx.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://st.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xy.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ew.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://bi.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://ci.newstarts.cn

Ruby: x.length;  x.size
来源：http://dn.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gr.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://ic.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pj.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ai.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ej.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oa.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xj.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gs.szsharing.cn

Ruby: a == b
来源：http://zg.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wu.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xs.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://du.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://cd.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mg.bjjhwx.cn

TS:   if (x == null) {}
来源：http://hi.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hu.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://sr.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wb.huixiangedu.cn

C#:   if (x is null) {}
来源：http://pj.shxzukj.cn

[P07] 防抖与节流
来源：http://zy.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ea.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://mt.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qi.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sg.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rx.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xb.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fe.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sx.521024.cn

[P08] 处理浮点精度问题
来源：http://uq.chemitech.net.cn


<!-- 参考信息 -->