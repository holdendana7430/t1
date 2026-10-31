代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mw.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://si.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://zs.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://if.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://zm.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dc.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xu.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://gw.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://mx.hnjuh.cn

Java: resp.statusCode()
来源：http://dx.nicolike.cn

Go:   resp.StatusCode
来源：http://hv.newstarts.cn

Ruby: resp.code.to_i
来源：http://rd.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://bt.szsharing.cn

[L08] 并发请求多个地址
来源：http://sn.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bh.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://gx.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ty.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tc.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ad.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hl.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tm.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rj.szsharing.cn

================================================================================
来源：http://uw.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://bl.panjiajie.cn

================================================================================
来源：http://nx.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://dm.szsharing.cn

Py:   sys.argv[1:]
来源：http://gu.newstarts.cn

PHP:  $argv;  $argc;
来源：http://jt.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://bs.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ta.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://kc.wgjwhj.cn

Go:   os.Args[1:]
来源：http://rv.nszjky.cn

Ruby: ARGV
来源：http://nr.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://cm.asd995.cn

[M02] 读取环境变量
来源：http://sp.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://bj.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cd.colortex.cn

JS:   process.env.HOME
来源：http://fs.asd995.cn

TS:   process.env.HOME
来源：http://ia.9csxet.cn

Java: System.getenv("HOME")
来源：http://sw.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sj.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://ev.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jl.hahajie.cn

[M03] 执行外部命令
来源：http://gq.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wk.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mo.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tc.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uh.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ow.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ka.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://el.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://gs.huanxung.cn

[M04] 获取当前工作目录
来源：http://fn.muxihuayi.cn

Py:   os.getcwd()
来源：http://ko.bjjhwx.cn

PHP:  getcwd();
来源：http://oc.haigaiapp.cn

JS:   process.cwd()
来源：http://oe.nszjky.cn

TS:   process.cwd()
来源：http://iy.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://yo.huanxung.cn

Go:   os.Getwd()
来源：http://gn.nszjky.cn

Ruby: Dir.pwd
来源：http://bk.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yy.szsharing.cn

[M05] 设置退出码
来源：http://cv.lnxyls.cn

Py:   sys.exit(1)
来源：http://lb.bjjhwx.cn

PHP:  exit(1);
来源：http://md.bjjhwx.cn

JS:   process.exit(1)
来源：http://qv.huixiangedu.cn

TS:   process.exit(1)
来源：http://zi.shtwfgs.cn

Java: System.exit(1)
来源：http://ne.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://tq.huixinmuqiang.cn

Ruby: exit 1
来源：http://jw.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jr.haigaiapp.cn

[M06] 向标准错误输出
来源：http://wb.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://au.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qo.newstarts.cn

JS:   console.error("err")
来源：http://yc.chemitech.net.cn

TS:   console.error("err")
来源：http://hg.bookmarksfly.cn

Java: System.err.println("err")
来源：http://cz.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://co.gzmigu.cn

Ruby: warn "err"
来源：http://jc.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://xj.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://dz.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://gs.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://os.panjiajie.cn

JS:   require.main === module
来源：http://jg.521024.cn

TS:   require.main === module
来源：http://zj.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://fa.lnxyls.cn

Go:   func main()
来源：http://br.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kn.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://go.asd995.cn

[M08] 获取系统与运行时信息
来源：http://qv.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://cw.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://gh.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://fm.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://gj.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mu.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sx.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bn.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gx.colortex.cn

================================================================================
来源：http://rh.chemitech.net.cn

N. 数据结构与算法
来源：http://vg.yuexingan06.cn

================================================================================
来源：http://ab.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://tz.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tp.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fp.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jz.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://td.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ka.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://lb.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ws.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wf.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://sb.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ey.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yp.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gd.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ki.newstarts.cn

Go:   slices.Sort(arr)
来源：http://bw.9csxet.cn

Ruby: arr.sort
来源：http://yu.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zh.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://gb.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pl.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://qg.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sj.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bk.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ps.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cf.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zn.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kg.newstarts.cn

[N04] 斐波那契数列
来源：http://oo.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xj.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xc.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pw.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://su.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://en.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cz.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ht.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ko.gzmigu.cn

[N05] 最大公约数
来源：http://nr.huanxung.cn

Py:   math.gcd(a, b)
来源：http://kx.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://df.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ii.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sx.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rl.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://ux.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zi.lnxyls.cn

[N06] 判断回文字符串
来源：http://bn.haigaiapp.cn

Py:   s == s[::-1]
来源：http://qc.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://qh.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://to.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://fe.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eq.9csxet.cn

Go:   // 双指针从两端比较
来源：http://rj.szsharing.cn

Ruby: s == s.reverse
来源：http://yu.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kl.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://jq.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ne.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kp.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ls.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://of.wgjwhj.cn

Java: // 手写 HashMap
来源：http://ee.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://ev.panjiajie.cn

Ruby: // 手写 Hash
来源：http://au.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kc.yuntaijiaju.cn

[N08] 生成全排列
来源：http://kk.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://rs.gzmigu.cn

PHP:  // 手写递归交换
来源：http://gw.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://zh.hahajie.cn

TS:   // 手写回溯递归
来源：http://ge.huixiangedu.cn

Java: // 手写回溯递归
来源：http://de.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://sc.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://zs.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://zq.yuexingan06.cn

[N09] 栈与队列
来源：http://xf.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wh.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wo.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rk.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lu.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vs.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kn.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oy.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ua.nicolike.cn

[N10] 链表节点定义
来源：http://bn.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ra.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jg.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zf.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ez.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://mi.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oh.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ip.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://na.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://tg.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aa.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://pb.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ne.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bb.yuexingan06.cn

Java: // 手写递归
来源：http://pi.asd995.cn

Go:   // 手写递归
来源：http://be.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ij.huixiangedu.cn

C#:   // 手写递归
来源：http://dg.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fh.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rj.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pa.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://do.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zx.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uy.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rw.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ih.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zs.hnjuh.cn

================================================================================
来源：http://cp.szsharing.cn

O. 并发与异步
来源：http://hc.yuntaijiaju.cn

================================================================================
来源：http://xt.jctech888.com.cn

[O01] 启动一个线程
来源：http://ta.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mf.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nm.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://un.szsharing.cn

TS:   // 同 JS
来源：http://us.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://zp.colortex.cn

Go:   go f()
来源：http://im.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://jv.521024.cn

C#:   Task.Run(() => F());
来源：http://ah.shtwfgs.cn

[O02] 使用线程池
来源：http://ob.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ns.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ek.9csxet.cn

JS:   // worker_threads 线程池
来源：http://wl.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://yc.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nf.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rk.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wu.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gd.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://hu.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ch.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://eh.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://do.nicolike.cn

TS:   // 同 JS
来源：http://um.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://xn.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zf.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://up.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://xr.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://pn.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://ox.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bk.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://th.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bd.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://om.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ze.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wg.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://vs.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://ch.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://yx.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lv.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://dd.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://at.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ng.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hm.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://xg.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rc.huanxung.cn

[O06] 使用进程池
来源：http://cf.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://um.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zt.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://ur.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://ji.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yb.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bw.9csxet.cn

Ruby: // fork 块
来源：http://tu.9csxet.cn

C#:   Parallel.For
来源：http://mi.bjjhwx.cn

================================================================================
来源：http://ad.nicolike.cn

P. 常用工具函数
来源：http://sr.asd995.cn

================================================================================
来源：http://wh.asd995.cn

[P01] 生成 UUID
来源：http://dk.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://bv.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fq.nszjky.cn

JS:   crypto.randomUUID()
来源：http://iw.521024.cn

TS:   crypto.randomUUID()
来源：http://zl.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://aj.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://vn.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://zs.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://th.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://ij.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ih.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mu.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tf.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://he.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ww.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ig.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://br.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gk.lnxyls.cn

[P03] 生成短随机字符串
来源：http://kb.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dp.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vq.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ay.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hu.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://au.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gc.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gb.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mf.colortex.cn

[P04] 求长度
来源：http://pm.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nd.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kk.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hr.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iu.9csxet.cn


<!-- 参考信息 -->