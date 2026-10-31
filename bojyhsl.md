代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pu.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cg.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://tp.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rf.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://zr.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jl.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bk.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://gl.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://om.asd995.cn

Java: resp.statusCode()
来源：http://pv.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ty.newstarts.cn

Ruby: resp.code.to_i
来源：http://yh.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://fb.huanxung.cn

[L08] 并发请求多个地址
来源：http://ug.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://du.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://ym.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wh.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dz.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ez.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cm.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xd.shtwfgs.cn

================================================================================
来源：http://mv.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://yl.huixiangedu.cn

================================================================================
来源：http://tl.szsharing.cn

[M01] 读取命令行参数
来源：http://qo.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://yz.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://uq.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://jh.newstarts.cn

TS:   process.argv.slice(2)
来源：http://rb.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://pf.huixiangedu.cn

Go:   os.Args[1:]
来源：http://uk.hnjuh.cn

Ruby: ARGV
来源：http://ix.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://tg.wgjwhj.cn

[M02] 读取环境变量
来源：http://wz.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://ni.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nw.shtwfgs.cn

JS:   process.env.HOME
来源：http://pj.nszjky.cn

TS:   process.env.HOME
来源：http://gx.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://vp.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hn.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://jj.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qp.colortex.cn

[M03] 执行外部命令
来源：http://no.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tg.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tw.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vo.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gv.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dv.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sp.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ud.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://kw.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://lt.newstarts.cn

Py:   os.getcwd()
来源：http://zi.gzmigu.cn

PHP:  getcwd();
来源：http://df.newstarts.cn

JS:   process.cwd()
来源：http://cw.521024.cn

TS:   process.cwd()
来源：http://rv.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://lc.lnxyls.cn

Go:   os.Getwd()
来源：http://jo.yuexingan06.cn

Ruby: Dir.pwd
来源：http://ww.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ko.nszjky.cn

[M05] 设置退出码
来源：http://qe.bjjhwx.cn

Py:   sys.exit(1)
来源：http://nl.shxzukj.cn

PHP:  exit(1);
来源：http://jx.bookmarksfly.cn

JS:   process.exit(1)
来源：http://un.newstarts.cn

TS:   process.exit(1)
来源：http://sq.huixiangedu.cn

Java: System.exit(1)
来源：http://jk.huixiangedu.cn

Go:   os.Exit(1)
来源：http://wm.panjiajie.cn

Ruby: exit 1
来源：http://az.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jx.hnjuh.cn

[M06] 向标准错误输出
来源：http://mb.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://qt.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tc.colortex.cn

JS:   console.error("err")
来源：http://gz.chemitech.net.cn

TS:   console.error("err")
来源：http://bn.bjjhwx.cn

Java: System.err.println("err")
来源：http://hr.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://do.huixiangedu.cn

Ruby: warn "err"
来源：http://mz.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://rk.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://dz.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://td.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bt.panjiajie.cn

JS:   require.main === module
来源：http://yw.gzmigu.cn

TS:   require.main === module
来源：http://gx.hnjuh.cn

Java: public static void main(String[] args)
来源：http://qe.newstarts.cn

Go:   func main()
来源：http://uv.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wp.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://hj.colortex.cn

[M08] 获取系统与运行时信息
来源：http://qy.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://je.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://jj.lnxyls.cn

JS:   process.platform;  process.version
来源：http://tm.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://cc.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ci.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ut.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ly.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fu.wgjwhj.cn

================================================================================
来源：http://ze.yuntaijiaju.cn

N. 数据结构与算法
来源：http://gr.muxihuayi.cn

================================================================================
来源：http://wq.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://ea.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ic.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nx.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wj.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kw.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://de.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://ij.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gv.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jr.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://mv.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://as.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gt.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yy.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uv.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nf.nszjky.cn

Go:   slices.Sort(arr)
来源：http://yj.chemitech.net.cn

Ruby: arr.sort
来源：http://ah.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kg.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://vw.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oo.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://lp.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ln.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gv.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fz.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pj.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sz.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ic.bjjhwx.cn

[N04] 斐波那契数列
来源：http://yx.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kz.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zv.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rd.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://te.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ff.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cf.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zg.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qy.shxzskj.cn

[N05] 最大公约数
来源：http://sa.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://oy.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jt.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iz.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oe.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cr.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ou.colortex.cn

Ruby: a.gcd(b)
来源：http://tx.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wv.muxihuayi.cn

[N06] 判断回文字符串
来源：http://zt.chemitech.net.cn

Py:   s == s[::-1]
来源：http://ba.szsharing.cn

PHP:  $s === strrev($s);
来源：http://ya.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://db.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://vl.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cr.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://mz.chemitech.net.cn

Ruby: s == s.reverse
来源：http://uy.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://du.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://tp.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ld.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wi.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dk.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://cw.9csxet.cn

Java: // 手写 HashMap
来源：http://iv.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://af.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ze.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://si.asd995.cn

[N08] 生成全排列
来源：http://jw.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://gc.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://di.szsharing.cn

JS:   // 手写回溯递归
来源：http://yv.9csxet.cn

TS:   // 手写回溯递归
来源：http://pb.shxzukj.cn

Java: // 手写回溯递归
来源：http://bk.9csxet.cn

Go:   // 手写回溯递归
来源：http://op.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://yh.szsharing.cn

C#:   // 手写回溯递归
来源：http://as.panjiajie.cn

[N09] 栈与队列
来源：http://gv.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ob.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cu.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gc.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xz.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dn.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cs.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://le.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wf.szxytkj.cn

[N10] 链表节点定义
来源：http://ja.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lm.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hd.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ch.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://by.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://nx.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jt.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gd.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xz.newstarts.cn

[N11] 二叉树中序遍历
来源：http://nx.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ao.9csxet.cn

PHP:  // 手写递归函数
来源：http://sk.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://th.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bd.huanxung.cn

Java: // 手写递归
来源：http://gs.haigaiapp.cn

Go:   // 手写递归
来源：http://xo.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ag.huixiangedu.cn

C#:   // 手写递归
来源：http://nl.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xw.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lp.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kf.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ue.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jz.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ti.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wl.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vp.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bn.wgjwhj.cn

================================================================================
来源：http://ww.chemitech.net.cn

O. 并发与异步
来源：http://ne.521024.cn

================================================================================
来源：http://kd.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://sw.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tc.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xz.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pk.jctech888.com.cn

TS:   // 同 JS
来源：http://ii.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://ni.huanxung.cn

Go:   go f()
来源：http://oh.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://qv.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://lg.nicolike.cn

[O02] 使用线程池
来源：http://ox.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ja.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://td.szsharing.cn

JS:   // worker_threads 线程池
来源：http://hs.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://dc.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iw.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dv.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lb.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zi.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://fz.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://nz.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ie.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vg.9csxet.cn

TS:   // 同 JS
来源：http://jv.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://bv.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://at.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mk.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://fn.9csxet.cn

[O04] 定义异步函数并等待
来源：http://nu.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://tf.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rf.huanxung.cn

JS:   async function f() { await g(); }
来源：http://gt.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ra.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gf.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uh.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yb.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://qd.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://hr.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ny.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xw.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://ts.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://ac.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pp.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qp.asd995.cn

Ruby: threads.map(&:join)
来源：http://kc.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fj.lnxyls.cn

[O06] 使用进程池
来源：http://ak.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rv.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tm.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://it.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://hv.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bg.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aq.521024.cn

Ruby: // fork 块
来源：http://kj.shxzskj.cn

C#:   Parallel.For
来源：http://nm.gzmigu.cn

================================================================================
来源：http://fj.muxihuayi.cn

P. 常用工具函数
来源：http://ld.haigaiapp.cn

================================================================================
来源：http://rt.asd995.cn

[P01] 生成 UUID
来源：http://wy.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://aw.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ed.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://gl.colortex.cn

TS:   crypto.randomUUID()
来源：http://ks.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://na.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://mw.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://ow.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://au.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://zc.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pl.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vd.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nj.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uq.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bd.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ed.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bz.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zu.nszjky.cn

[P03] 生成短随机字符串
来源：http://dq.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xm.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nl.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ec.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dh.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://az.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qi.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xx.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://on.jctech888.com.cn

[P04] 求长度
来源：http://fq.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lj.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://to.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xh.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vd.lnxyls.cn


<!-- 参考信息 -->