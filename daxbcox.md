代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oe.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fa.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://hg.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dq.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://kw.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ns.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uj.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://aw.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://mp.haigaiapp.cn

Java: resp.statusCode()
来源：http://ua.hahajie.cn

Go:   resp.StatusCode
来源：http://el.9csxet.cn

Ruby: resp.code.to_i
来源：http://mc.521024.cn

C#:   (int)resp.StatusCode
来源：http://qe.shxzskj.cn

[L08] 并发请求多个地址
来源：http://hp.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nv.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ns.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mb.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dh.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ck.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ze.jctech888.com.cn

================================================================================
来源：http://og.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://hr.nicolike.cn

================================================================================
来源：http://ik.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://qz.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://wo.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://kk.nicolike.cn

JS:   process.argv.slice(2)
来源：http://mx.521024.cn

TS:   process.argv.slice(2)
来源：http://yp.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://vr.newstarts.cn

Go:   os.Args[1:]
来源：http://uu.huixinmuqiang.cn

Ruby: ARGV
来源：http://sm.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://qv.nicolike.cn

[M02] 读取环境变量
来源：http://ki.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://pa.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bu.szsharing.cn

JS:   process.env.HOME
来源：http://qy.colortex.cn

TS:   process.env.HOME
来源：http://ym.asd995.cn

Java: System.getenv("HOME")
来源：http://tr.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qm.asd995.cn

Ruby: ENV["HOME"]
来源：http://nh.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ac.nszjky.cn

[M03] 执行外部命令
来源：http://ra.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ib.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mh.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vc.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ln.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jd.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ku.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gc.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://uy.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://zv.gzmigu.cn

Py:   os.getcwd()
来源：http://ya.lnxyls.cn

PHP:  getcwd();
来源：http://or.jctech888.com.cn

JS:   process.cwd()
来源：http://cn.szsharing.cn

TS:   process.cwd()
来源：http://fv.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ey.bookmarksfly.cn

Go:   os.Getwd()
来源：http://yj.nicolike.cn

Ruby: Dir.pwd
来源：http://ec.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ll.panjiajie.cn

[M05] 设置退出码
来源：http://em.shxzukj.cn

Py:   sys.exit(1)
来源：http://nf.wgjwhj.cn

PHP:  exit(1);
来源：http://ss.521024.cn

JS:   process.exit(1)
来源：http://vs.szsharing.cn

TS:   process.exit(1)
来源：http://ka.shtwfgs.cn

Java: System.exit(1)
来源：http://gj.bjjhwx.cn

Go:   os.Exit(1)
来源：http://qf.szxytkj.cn

Ruby: exit 1
来源：http://kr.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wq.jctech888.com.cn

[M06] 向标准错误输出
来源：http://iv.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://ow.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jo.huixinmuqiang.cn

JS:   console.error("err")
来源：http://mk.nicolike.cn

TS:   console.error("err")
来源：http://zn.nszjky.cn

Java: System.err.println("err")
来源：http://jr.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xh.szxytkj.cn

Ruby: warn "err"
来源：http://vu.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ly.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://pe.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://av.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fb.yuntaijiaju.cn

JS:   require.main === module
来源：http://ep.wgjwhj.cn

TS:   require.main === module
来源：http://dm.hahajie.cn

Java: public static void main(String[] args)
来源：http://ha.panjiajie.cn

Go:   func main()
来源：http://st.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gw.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://eg.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://bu.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://wc.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://mo.hahajie.cn

JS:   process.platform;  process.version
来源：http://gp.nicolike.cn

TS:   process.platform;  process.version
来源：http://iq.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vc.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fd.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://un.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pw.hnjuh.cn

================================================================================
来源：http://vy.9csxet.cn

N. 数据结构与算法
来源：http://gk.asd995.cn

================================================================================
来源：http://ju.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://jb.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yr.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jx.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xz.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nv.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://nu.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ey.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://el.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://wz.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://xt.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sp.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wt.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zk.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hr.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://yq.huixiangedu.cn

Ruby: arr.sort
来源：http://vl.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sy.asd995.cn

[N03] 快速排序（分治示例）
来源：http://tb.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yy.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://zd.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tf.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zk.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://th.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wm.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ik.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zz.hnjuh.cn

[N04] 斐波那契数列
来源：http://ru.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ph.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://au.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://du.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lz.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fi.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gw.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fe.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uy.hahajie.cn

[N05] 最大公约数
来源：http://lt.nszjky.cn

Py:   math.gcd(a, b)
来源：http://is.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ec.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://af.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lo.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ip.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tj.shxzukj.cn

Ruby: a.gcd(b)
来源：http://tf.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fu.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://rl.muxihuayi.cn

Py:   s == s[::-1]
来源：http://wb.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://tp.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://jb.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://ij.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mr.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ka.newstarts.cn

Ruby: s == s.reverse
来源：http://eu.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rv.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://yb.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vs.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://of.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ac.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://to.huanxung.cn

Java: // 手写 HashMap
来源：http://lp.9csxet.cn

Go:   // 手写 map[int]int
来源：http://bh.szxytkj.cn

Ruby: // 手写 Hash
来源：http://iu.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nw.yuntaijiaju.cn

[N08] 生成全排列
来源：http://ix.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://iv.hnjuh.cn

PHP:  // 手写递归交换
来源：http://py.lnxyls.cn

JS:   // 手写回溯递归
来源：http://pd.9csxet.cn

TS:   // 手写回溯递归
来源：http://nk.yuexingan06.cn

Java: // 手写回溯递归
来源：http://ba.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://qx.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://qk.newstarts.cn

C#:   // 手写回溯递归
来源：http://tf.521024.cn

[N09] 栈与队列
来源：http://zs.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jx.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uu.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xm.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pw.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nj.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jo.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pl.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mg.shxzskj.cn

[N10] 链表节点定义
来源：http://ms.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ip.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ks.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qs.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ri.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://sc.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ql.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xe.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gh.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://vw.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://va.9csxet.cn

PHP:  // 手写递归函数
来源：http://cc.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lz.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rt.nszjky.cn

Java: // 手写递归
来源：http://vb.huanxung.cn

Go:   // 手写递归
来源：http://pu.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ce.newstarts.cn

C#:   // 手写递归
来源：http://di.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jk.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qi.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zd.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xt.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://az.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aj.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zl.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ja.jianghongdianzi.cn

================================================================================
来源：http://yn.gzmigu.cn

O. 并发与异步
来源：http://ft.gzmigu.cn

================================================================================
来源：http://gc.gzmigu.cn

[O01] 启动一个线程
来源：http://jw.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iz.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ek.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zn.9csxet.cn

TS:   // 同 JS
来源：http://qd.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://aq.szxytkj.cn

Go:   go f()
来源：http://kb.521024.cn

Ruby: Thread.new { f }
来源：http://rz.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://qe.shxzskj.cn

[O02] 使用线程池
来源：http://vm.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gi.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dy.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://kv.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://rn.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tg.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gp.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kj.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pl.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://jl.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://cr.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://mw.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ya.shtwfgs.cn

TS:   // 同 JS
来源：http://xj.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://yl.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dy.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xr.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://zy.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://mr.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ah.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qc.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://fo.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vz.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sj.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ti.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dq.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://oz.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://mh.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://jx.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xq.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://io.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://db.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hg.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kb.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://bv.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gf.521024.cn

[O06] 使用进程池
来源：http://nz.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ap.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ei.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://el.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://tg.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yo.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ne.panjiajie.cn

Ruby: // fork 块
来源：http://aj.muxihuayi.cn

C#:   Parallel.For
来源：http://kw.9csxet.cn

================================================================================
来源：http://zz.haigaiapp.cn

P. 常用工具函数
来源：http://vg.colortex.cn

================================================================================
来源：http://ql.huixiangedu.cn

[P01] 生成 UUID
来源：http://rh.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://bb.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rz.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://zv.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://sx.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://vp.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://ee.asd995.cn

Ruby: SecureRandom.uuid
来源：http://td.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://su.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://nl.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dq.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ze.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://so.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fc.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wq.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ut.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gq.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ei.shxzukj.cn

[P03] 生成短随机字符串
来源：http://qs.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ro.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fy.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yu.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kn.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kg.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ez.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mp.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qi.nszjky.cn

[P04] 求长度
来源：http://gt.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gz.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rr.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oy.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oq.chemitech.net.cn


<!-- 参考信息 -->