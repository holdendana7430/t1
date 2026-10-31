代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hr.9csxet.cn

Java: resp.statusCode()
来源：http://nc.jctech888.com.cn

Go:   resp.StatusCode
来源：http://cg.shxzukj.cn

Ruby: resp.code.to_i
来源：http://rl.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://uw.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://kk.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://da.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://fw.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vk.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lv.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yy.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zk.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pg.shxzukj.cn

================================================================================
来源：http://ze.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://sx.9csxet.cn

================================================================================
来源：http://qx.nszjky.cn

[M01] 读取命令行参数
来源：http://ak.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://da.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://iq.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://oo.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://vr.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://nw.shxzukj.cn

Go:   os.Args[1:]
来源：http://bd.9csxet.cn

Ruby: ARGV
来源：http://kj.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ll.muxihuayi.cn

[M02] 读取环境变量
来源：http://qa.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://yl.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xp.szxytkj.cn

JS:   process.env.HOME
来源：http://bw.szsharing.cn

TS:   process.env.HOME
来源：http://ke.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://un.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hm.hahajie.cn

Ruby: ENV["HOME"]
来源：http://oa.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mq.newstarts.cn

[M03] 执行外部命令
来源：http://lq.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://db.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xn.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ug.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ca.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cr.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eh.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nc.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://ut.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://vu.shtwfgs.cn

Py:   os.getcwd()
来源：http://mp.bookmarksfly.cn

PHP:  getcwd();
来源：http://gk.chemitech.net.cn

JS:   process.cwd()
来源：http://lp.newstarts.cn

TS:   process.cwd()
来源：http://to.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://hd.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://un.shtwfgs.cn

Ruby: Dir.pwd
来源：http://pe.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fu.hnjuh.cn

[M05] 设置退出码
来源：http://cr.shxzukj.cn

Py:   sys.exit(1)
来源：http://yl.gzmigu.cn

PHP:  exit(1);
来源：http://xi.muxihuayi.cn

JS:   process.exit(1)
来源：http://nz.szsharing.cn

TS:   process.exit(1)
来源：http://hs.chemitech.net.cn

Java: System.exit(1)
来源：http://jn.panjiajie.cn

Go:   os.Exit(1)
来源：http://br.nszjky.cn

Ruby: exit 1
来源：http://lu.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://at.wgjwhj.cn

[M06] 向标准错误输出
来源：http://av.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://mu.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zq.bjjhwx.cn

JS:   console.error("err")
来源：http://pk.gzmigu.cn

TS:   console.error("err")
来源：http://vy.hahajie.cn

Java: System.err.println("err")
来源：http://ur.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gj.colortex.cn

Ruby: warn "err"
来源：http://ba.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://pd.shxzukj.cn

[M07] 判断是否为主入口
来源：http://ef.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://oc.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gg.521024.cn

JS:   require.main === module
来源：http://xs.szsharing.cn

TS:   require.main === module
来源：http://uc.gzmigu.cn

Java: public static void main(String[] args)
来源：http://iw.panjiajie.cn

Go:   func main()
来源：http://ec.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gz.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://ak.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://jq.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://oh.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ad.shxzskj.cn

JS:   process.platform;  process.version
来源：http://yk.nszjky.cn

TS:   process.platform;  process.version
来源：http://ye.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sk.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nt.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://le.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ju.colortex.cn

================================================================================
来源：http://oy.bjjhwx.cn

N. 数据结构与算法
来源：http://lp.shxzskj.cn

================================================================================
来源：http://ed.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://kw.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lr.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pb.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lf.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xm.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jz.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://au.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zw.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kz.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://dm.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://yl.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://az.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mx.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jp.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://of.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ra.jctech888.com.cn

Ruby: arr.sort
来源：http://dq.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wq.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://xq.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fb.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://yp.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uh.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yk.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iz.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://en.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sc.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sz.panjiajie.cn

[N04] 斐波那契数列
来源：http://vy.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rz.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hi.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cz.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aj.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vr.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tg.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zp.gzmigu.cn

[N05] 最大公约数
来源：http://bn.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ci.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sg.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jn.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pv.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cz.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://se.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ti.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rh.jctech888.com.cn

[N06] 判断回文字符串
来源：http://uy.shxzskj.cn

Py:   s == s[::-1]
来源：http://fu.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://sx.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://ci.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://sq.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yl.szsharing.cn

Go:   // 双指针从两端比较
来源：http://id.bjjhwx.cn

Ruby: s == s.reverse
来源：http://au.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dk.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://vf.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ha.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dl.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fo.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://rn.hnjuh.cn

Java: // 手写 HashMap
来源：http://ar.asd995.cn

Go:   // 手写 map[int]int
来源：http://kb.nszjky.cn

Ruby: // 手写 Hash
来源：http://te.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hz.521024.cn

[N08] 生成全排列
来源：http://iw.asd995.cn

Py:   itertools.permutations(arr)
来源：http://em.hahajie.cn

PHP:  // 手写递归交换
来源：http://yx.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://rf.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://xj.yuexingan06.cn

Java: // 手写回溯递归
来源：http://vi.lnxyls.cn

Go:   // 手写回溯递归
来源：http://on.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://ib.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://ml.wgjwhj.cn

[N09] 栈与队列
来源：http://ik.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eo.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tg.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://as.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rx.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gl.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vg.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ua.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mz.lnxyls.cn

[N10] 链表节点定义
来源：http://sb.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://td.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yv.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xg.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kg.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://ar.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fc.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xx.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mh.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://fn.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xd.szsharing.cn

PHP:  // 手写递归函数
来源：http://ye.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lm.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ci.hnjuh.cn

Java: // 手写递归
来源：http://dx.colortex.cn

Go:   // 手写递归
来源：http://pf.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tj.shxzskj.cn

C#:   // 手写递归
来源：http://mq.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fs.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ft.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vr.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bo.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nk.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ej.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ib.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zk.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mr.huixiangedu.cn

================================================================================
来源：http://gx.jianghongdianzi.cn

O. 并发与异步
来源：http://vz.hahajie.cn

================================================================================
来源：http://xt.yuexingan06.cn

[O01] 启动一个线程
来源：http://ie.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wh.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wo.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ft.huixinmuqiang.cn

TS:   // 同 JS
来源：http://nv.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://qy.szxytkj.cn

Go:   go f()
来源：http://mk.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://xm.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://fp.gzmigu.cn

[O02] 使用线程池
来源：http://az.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bx.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fh.9csxet.cn

JS:   // worker_threads 线程池
来源：http://uz.huanxung.cn

TS:   // worker_threads 线程池
来源：http://hv.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ba.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ld.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ix.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qr.colortex.cn

[O03] 加锁保护共享数据
来源：http://od.gzmigu.cn

Py:   with lock: shared += 1
来源：http://tf.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ks.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lf.haigaiapp.cn

TS:   // 同 JS
来源：http://eo.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ks.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kl.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fo.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://dv.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://mp.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://kz.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jt.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://be.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pp.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gc.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bg.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ki.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://fs.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://cm.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://hw.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rn.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://fb.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://cr.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ps.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jp.asd995.cn

Ruby: threads.map(&:join)
来源：http://cz.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zk.colortex.cn

[O06] 使用进程池
来源：http://ju.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vd.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ps.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://vw.asd995.cn

TS:   // child_process / cluster 模块
来源：http://hp.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rq.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kf.nszjky.cn

Ruby: // fork 块
来源：http://rm.bookmarksfly.cn

C#:   Parallel.For
来源：http://tj.lnxyls.cn

================================================================================
来源：http://ll.szxytkj.cn

P. 常用工具函数
来源：http://kw.yuexingan06.cn

================================================================================
来源：http://oh.chemitech.net.cn

[P01] 生成 UUID
来源：http://gf.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://mo.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qd.hahajie.cn

JS:   crypto.randomUUID()
来源：http://do.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://vo.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://iu.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://tn.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://vp.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://gk.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://xf.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wh.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qx.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uc.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xl.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mr.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jk.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aq.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pr.nszjky.cn

[P03] 生成短随机字符串
来源：http://zg.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pt.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ia.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fj.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tx.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ih.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ui.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xi.lnxyls.cn

[P04] 求长度
来源：http://qa.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dw.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kd.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vm.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dp.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://ld.asd995.cn

Go:   len(arr);  len(m)
来源：http://df.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://pu.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rk.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://qk.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yy.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ld.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qp.szxytkj.cn


<!-- 参考信息 -->