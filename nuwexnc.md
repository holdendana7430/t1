代发 wailian999

JS:   process.argv.slice(2)
来源：http://eb.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://kq.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://hl.shxzukj.cn

Go:   os.Args[1:]
来源：http://xp.521024.cn

Ruby: ARGV
来源：http://tu.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ck.huixiangedu.cn

[M02] 读取环境变量
来源：http://vq.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://mx.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vt.9csxet.cn

JS:   process.env.HOME
来源：http://vo.muxihuayi.cn

TS:   process.env.HOME
来源：http://tf.nicolike.cn

Java: System.getenv("HOME")
来源：http://kl.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gi.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vc.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pm.panjiajie.cn

[M03] 执行外部命令
来源：http://cp.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jq.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kv.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kv.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yg.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lw.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xf.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sh.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://bm.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://gh.bookmarksfly.cn

Py:   os.getcwd()
来源：http://oj.yuexingan06.cn

PHP:  getcwd();
来源：http://yw.szsharing.cn

JS:   process.cwd()
来源：http://fg.hahajie.cn

TS:   process.cwd()
来源：http://tb.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ze.shxzskj.cn

Go:   os.Getwd()
来源：http://ko.haigaiapp.cn

Ruby: Dir.pwd
来源：http://yi.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hc.newstarts.cn

[M05] 设置退出码
来源：http://qy.szxytkj.cn

Py:   sys.exit(1)
来源：http://yk.gzmigu.cn

PHP:  exit(1);
来源：http://pk.colortex.cn

JS:   process.exit(1)
来源：http://qw.haigaiapp.cn

TS:   process.exit(1)
来源：http://jn.newstarts.cn

Java: System.exit(1)
来源：http://si.jctech888.com.cn

Go:   os.Exit(1)
来源：http://cr.yuexingan06.cn

Ruby: exit 1
来源：http://na.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://od.panjiajie.cn

[M06] 向标准错误输出
来源：http://co.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mg.szxytkj.cn

JS:   console.error("err")
来源：http://ed.shtwfgs.cn

TS:   console.error("err")
来源：http://os.bookmarksfly.cn

Java: System.err.println("err")
来源：http://hc.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vx.yuntaijiaju.cn

Ruby: warn "err"
来源：http://jl.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://za.newstarts.cn

[M07] 判断是否为主入口
来源：http://sk.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://nq.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fm.muxihuayi.cn

JS:   require.main === module
来源：http://qt.huixinmuqiang.cn

TS:   require.main === module
来源：http://rv.colortex.cn

Java: public static void main(String[] args)
来源：http://pt.jianghongdianzi.cn

Go:   func main()
来源：http://cb.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lk.nszjky.cn

C#:   static void Main(string[] args)
来源：http://fe.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://vh.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ov.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://co.szsharing.cn

JS:   process.platform;  process.version
来源：http://wg.9csxet.cn

TS:   process.platform;  process.version
来源：http://nb.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ek.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zo.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bb.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rk.huixinmuqiang.cn

================================================================================
来源：http://aj.521024.cn

N. 数据结构与算法
来源：http://rf.521024.cn

================================================================================
来源：http://lj.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://cp.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jk.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ay.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fa.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ru.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hj.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://wh.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wf.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pp.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://bx.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://vu.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oo.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wz.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://du.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.szsharing.cn

Go:   slices.Sort(arr)
来源：http://ke.hnjuh.cn

Ruby: arr.sort
来源：http://gp.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fp.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://zy.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yy.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://vg.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ym.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ol.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mf.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://px.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cr.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zj.szxytkj.cn

[N04] 斐波那契数列
来源：http://sn.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mt.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wi.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dv.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://px.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aj.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ch.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nn.9csxet.cn

[N05] 最大公约数
来源：http://xz.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://bx.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ld.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xp.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rb.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://su.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dg.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://zm.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eh.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://cn.huixiangedu.cn

Py:   s == s[::-1]
来源：http://dd.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://nr.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://yg.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://vw.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ob.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://lk.bjjhwx.cn

Ruby: s == s.reverse
来源：http://wr.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://re.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ho.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lz.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xe.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dq.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://yt.szsharing.cn

Java: // 手写 HashMap
来源：http://pf.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://mf.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://yz.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://du.521024.cn

[N08] 生成全排列
来源：http://dg.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://al.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://fe.panjiajie.cn

JS:   // 手写回溯递归
来源：http://jn.panjiajie.cn

TS:   // 手写回溯递归
来源：http://gb.nszjky.cn

Java: // 手写回溯递归
来源：http://fc.521024.cn

Go:   // 手写回溯递归
来源：http://yq.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://yg.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://nu.jctech888.com.cn

[N09] 栈与队列
来源：http://yb.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ly.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vm.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jn.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ve.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://te.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cc.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ex.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kk.panjiajie.cn

[N10] 链表节点定义
来源：http://em.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xw.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qa.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lp.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://js.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://fn.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kl.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jm.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gx.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://es.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zq.szsharing.cn

PHP:  // 手写递归函数
来源：http://gs.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ah.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cq.huanxung.cn

Java: // 手写递归
来源：http://lh.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ze.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gv.asd995.cn

C#:   // 手写递归
来源：http://ap.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sv.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ql.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cr.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kk.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://at.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sa.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vu.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mh.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://al.chemitech.net.cn

================================================================================
来源：http://fg.panjiajie.cn

O. 并发与异步
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://mc.muxihuayi.cn

[O01] 启动一个线程
来源：http://ec.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ci.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kh.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kl.yuntaijiaju.cn

TS:   // 同 JS
来源：http://vp.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://uz.bookmarksfly.cn

Go:   go f()
来源：http://zn.nszjky.cn

Ruby: Thread.new { f }
来源：http://fp.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://xk.nicolike.cn

[O02] 使用线程池
来源：http://py.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qc.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wk.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://sd.nicolike.cn

TS:   // worker_threads 线程池
来源：http://da.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rs.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iz.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xj.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dl.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://cp.shxzukj.cn

Py:   with lock: shared += 1
来源：http://sy.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://oo.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mt.jianghongdianzi.cn

TS:   // 同 JS
来源：http://qu.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://xi.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://is.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jr.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://gt.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://xb.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://pl.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wb.huanxung.cn

JS:   async function f() { await g(); }
来源：http://vm.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qx.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ws.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dl.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lb.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://tw.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://qn.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://cy.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qp.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://jw.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://nd.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vd.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vb.hahajie.cn

Ruby: threads.map(&:join)
来源：http://tt.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ce.panjiajie.cn

[O06] 使用进程池
来源：http://kx.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://co.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://py.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://kz.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://pq.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vh.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ki.gzmigu.cn

Ruby: // fork 块
来源：http://kw.szxytkj.cn

C#:   Parallel.For
来源：http://tv.asd995.cn

================================================================================
来源：http://fo.9csxet.cn

P. 常用工具函数
来源：http://zx.shtwfgs.cn

================================================================================
来源：http://wi.bjjhwx.cn

[P01] 生成 UUID
来源：http://jy.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://tx.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://la.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://az.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://uz.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://tx.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://bb.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ff.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://hl.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://us.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jh.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ib.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://su.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vx.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bn.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cw.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ys.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yz.gzmigu.cn

[P03] 生成短随机字符串
来源：http://dr.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wn.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dm.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qk.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dy.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tj.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ni.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://by.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iz.9csxet.cn

[P04] 求长度
来源：http://lu.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pw.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fj.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ol.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ya.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ay.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://nq.nicolike.cn

Ruby: x.length;  x.size
来源：http://gd.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fk.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://xg.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xh.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ve.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cf.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xp.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cr.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://km.colortex.cn

Ruby: a == b
来源：http://hq.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ze.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tt.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zf.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://dp.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gb.9csxet.cn

TS:   if (x == null) {}
来源：http://mc.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zq.yuexingan06.cn

Go:   if x == nil {}
来源：http://ag.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://az.asd995.cn

C#:   if (x is null) {}
来源：http://th.lnxyls.cn

[P07] 防抖与节流
来源：http://xa.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ba.521024.cn

PHP:  // 手写时间戳比较
来源：http://vr.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sc.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iq.shtwfgs.cn


<!-- 参考信息 -->