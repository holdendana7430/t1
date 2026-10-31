代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vl.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://vk.huixiangedu.cn

TS:   process.env.HOME
来源：http://cv.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://zp.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ei.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://pp.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fw.jctech888.com.cn

[M03] 执行外部命令
来源：http://dl.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sp.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mc.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ro.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pa.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eb.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hx.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jv.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://sm.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://wf.jctech888.com.cn

Py:   os.getcwd()
来源：http://sa.chemitech.net.cn

PHP:  getcwd();
来源：http://en.bookmarksfly.cn

JS:   process.cwd()
来源：http://fc.panjiajie.cn

TS:   process.cwd()
来源：http://dt.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://qe.asd995.cn

Go:   os.Getwd()
来源：http://oc.panjiajie.cn

Ruby: Dir.pwd
来源：http://dp.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://az.nszjky.cn

[M05] 设置退出码
来源：http://ui.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://vd.yuexingan06.cn

PHP:  exit(1);
来源：http://js.yuexingan06.cn

JS:   process.exit(1)
来源：http://ii.muxihuayi.cn

TS:   process.exit(1)
来源：http://jp.bjjhwx.cn

Java: System.exit(1)
来源：http://pp.szsharing.cn

Go:   os.Exit(1)
来源：http://gu.haigaiapp.cn

Ruby: exit 1
来源：http://ha.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ur.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://rg.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://wy.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cv.shxzskj.cn

JS:   console.error("err")
来源：http://mn.bjjhwx.cn

TS:   console.error("err")
来源：http://ec.lnxyls.cn

Java: System.err.println("err")
来源：http://nx.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xi.muxihuayi.cn

Ruby: warn "err"
来源：http://rx.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://rp.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://ks.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://do.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fq.newstarts.cn

JS:   require.main === module
来源：http://dp.wgjwhj.cn

TS:   require.main === module
来源：http://ys.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://rx.jctech888.com.cn

Go:   func main()
来源：http://cr.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fb.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://fo.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://ga.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://dw.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://xe.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ih.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://lg.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ld.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ae.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://od.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wq.yuntaijiaju.cn

================================================================================
来源：http://yu.lnxyls.cn

N. 数据结构与算法
来源：http://rv.muxihuayi.cn

================================================================================
来源：http://vr.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://km.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://en.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sj.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yn.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kz.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bq.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://qt.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ks.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xa.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://sj.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://bj.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kg.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cx.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qt.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rv.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://az.muxihuayi.cn

Ruby: arr.sort
来源：http://qc.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cb.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://dd.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gi.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://hp.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vy.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ta.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sf.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://my.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lf.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qw.colortex.cn

[N04] 斐波那契数列
来源：http://gu.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://as.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dj.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sj.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://br.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wo.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fy.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xd.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nc.shxzukj.cn

[N05] 最大公约数
来源：http://du.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://mi.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jn.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ph.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://da.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://no.gzmigu.cn

Ruby: a.gcd(b)
来源：http://fr.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hw.huanxung.cn

[N06] 判断回文字符串
来源：http://mg.9csxet.cn

Py:   s == s[::-1]
来源：http://xq.nicolike.cn

PHP:  $s === strrev($s);
来源：http://fl.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://qm.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://lm.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gl.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://zz.bjjhwx.cn

Ruby: s == s.reverse
来源：http://uo.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://su.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://ln.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gp.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jk.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ab.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://do.gzmigu.cn

Java: // 手写 HashMap
来源：http://pi.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://bg.szxytkj.cn

Ruby: // 手写 Hash
来源：http://hx.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qn.bjjhwx.cn

[N08] 生成全排列
来源：http://zn.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://ng.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://hb.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://xg.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://qm.huixiangedu.cn

Java: // 手写回溯递归
来源：http://ib.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://ah.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://xi.szxytkj.cn

C#:   // 手写回溯递归
来源：http://pk.newstarts.cn

[N09] 栈与队列
来源：http://uf.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lq.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mn.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jh.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ke.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yc.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dl.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fn.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sx.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ot.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mh.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ok.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lv.521024.cn

Java: class Node { int v; Node next; }
来源：http://hv.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ml.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://va.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://db.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://yw.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dx.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://zu.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nd.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dd.chemitech.net.cn

Java: // 手写递归
来源：http://vm.newstarts.cn

Go:   // 手写递归
来源：http://ga.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fg.wgjwhj.cn

C#:   // 手写递归
来源：http://zl.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xe.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xk.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fk.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yh.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hk.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bh.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pp.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pa.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jy.huixiangedu.cn

================================================================================
来源：http://yb.szsharing.cn

O. 并发与异步
来源：http://au.bookmarksfly.cn

================================================================================
来源：http://bx.szsharing.cn

[O01] 启动一个线程
来源：http://lz.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qc.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dw.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gb.colortex.cn

TS:   // 同 JS
来源：http://ye.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://rj.szsharing.cn

Go:   go f()
来源：http://ix.szxytkj.cn

Ruby: Thread.new { f }
来源：http://as.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://wm.huanxung.cn

[O02] 使用线程池
来源：http://zc.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uo.newstarts.cn

JS:   // worker_threads 线程池
来源：http://in.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://pq.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cw.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ae.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://li.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rs.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://wu.shxzukj.cn

Py:   with lock: shared += 1
来源：http://bm.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://ft.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mh.jctech888.com.cn

TS:   // 同 JS
来源：http://gy.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://fw.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nm.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vv.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://ug.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://tr.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://ze.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pz.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://vn.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://li.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jn.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dc.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bh.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://cb.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://gn.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://bh.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rx.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://aj.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://kl.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xx.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ab.521024.cn

Ruby: threads.map(&:join)
来源：http://kg.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qk.hnjuh.cn

[O06] 使用进程池
来源：http://mu.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zl.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rh.colortex.cn

JS:   // child_process / cluster 模块
来源：http://sv.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://gn.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hq.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ef.nszjky.cn

Ruby: // fork 块
来源：http://vu.panjiajie.cn

C#:   Parallel.For
来源：http://zd.shxzskj.cn

================================================================================
来源：http://op.colortex.cn

P. 常用工具函数
来源：http://zv.lnxyls.cn

================================================================================
来源：http://et.huanxung.cn

[P01] 生成 UUID
来源：http://jn.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://da.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hf.newstarts.cn

JS:   crypto.randomUUID()
来源：http://xz.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://oa.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://oa.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ep.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://si.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://yb.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://mo.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bc.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qq.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gx.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ln.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gu.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yo.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dr.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yk.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://hr.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bo.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mw.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cd.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jr.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://or.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uk.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://au.bjjhwx.cn

[P04] 求长度
来源：http://fn.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ju.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wu.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dd.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jf.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://fe.9csxet.cn

Go:   len(arr);  len(m)
来源：http://lu.asd995.cn

Ruby: x.length;  x.size
来源：http://ih.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ht.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://zm.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oi.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fm.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jq.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oe.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jr.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jn.shxzskj.cn

Ruby: a == b
来源：http://oj.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bk.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xt.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xf.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://au.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zi.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://pi.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zl.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://tf.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ie.szsharing.cn

C#:   if (x is null) {}
来源：http://yi.shxzskj.cn

[P07] 防抖与节流
来源：http://py.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bw.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://lj.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ip.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mq.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ql.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hq.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ba.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://mm.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mh.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ul.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lt.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pd.bookmarksfly.cn


<!-- 参考信息 -->