代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cp.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uu.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://jz.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hi.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://wk.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jd.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lr.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://st.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ux.9csxet.cn

Java: resp.statusCode()
来源：http://au.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://tj.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://oe.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ku.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ib.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fh.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://vm.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hl.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ay.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ly.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dv.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pb.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yk.szxytkj.cn

================================================================================
来源：http://as.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://eh.panjiajie.cn

================================================================================
来源：http://wh.nszjky.cn

[M01] 读取命令行参数
来源：http://cj.asd995.cn

Py:   sys.argv[1:]
来源：http://hl.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://xf.nszjky.cn

JS:   process.argv.slice(2)
来源：http://md.nicolike.cn

TS:   process.argv.slice(2)
来源：http://oa.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://rq.huanxung.cn

Go:   os.Args[1:]
来源：http://sm.newstarts.cn

Ruby: ARGV
来源：http://gb.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://oy.nicolike.cn

[M02] 读取环境变量
来源：http://aq.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://gz.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hb.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://ta.chemitech.net.cn

TS:   process.env.HOME
来源：http://xv.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://im.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ot.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://we.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bm.jctech888.com.cn

[M03] 执行外部命令
来源：http://bu.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yl.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ir.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ad.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qr.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tt.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fb.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://ph.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://py.yuexingan06.cn

Py:   os.getcwd()
来源：http://pd.nicolike.cn

PHP:  getcwd();
来源：http://vt.colortex.cn

JS:   process.cwd()
来源：http://wb.lnxyls.cn

TS:   process.cwd()
来源：http://fe.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://de.521024.cn

Go:   os.Getwd()
来源：http://pm.panjiajie.cn

Ruby: Dir.pwd
来源：http://kq.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jj.nszjky.cn

[M05] 设置退出码
来源：http://ze.9csxet.cn

Py:   sys.exit(1)
来源：http://qr.hahajie.cn

PHP:  exit(1);
来源：http://fe.haigaiapp.cn

JS:   process.exit(1)
来源：http://mb.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ql.shtwfgs.cn

Java: System.exit(1)
来源：http://uw.szsharing.cn

Go:   os.Exit(1)
来源：http://dq.gzmigu.cn

Ruby: exit 1
来源：http://rt.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://de.szsharing.cn

[M06] 向标准错误输出
来源：http://fo.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://bz.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ri.asd995.cn

JS:   console.error("err")
来源：http://fg.lnxyls.cn

TS:   console.error("err")
来源：http://ln.lnxyls.cn

Java: System.err.println("err")
来源：http://hi.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qd.asd995.cn

Ruby: warn "err"
来源：http://eb.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://tr.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://ge.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://jt.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tw.haigaiapp.cn

JS:   require.main === module
来源：http://tc.shxzskj.cn

TS:   require.main === module
来源：http://yx.shxzukj.cn

Java: public static void main(String[] args)
来源：http://pk.huixiangedu.cn

Go:   func main()
来源：http://tc.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ib.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://xe.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://fg.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://aj.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://bv.asd995.cn

JS:   process.platform;  process.version
来源：http://qw.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://qh.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ol.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uu.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ar.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lc.gzmigu.cn

================================================================================
来源：http://dt.huixiangedu.cn

N. 数据结构与算法
来源：http://jl.panjiajie.cn

================================================================================
来源：http://ls.521024.cn

[N01] 二分查找（有序数组）
来源：http://iq.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zg.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wr.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mz.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ls.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fk.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://qs.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ux.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sk.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://fp.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dj.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yh.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yw.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nr.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jw.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://tn.szxytkj.cn

Ruby: arr.sort
来源：http://ea.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cv.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://qe.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pr.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://hs.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pw.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ef.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oa.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dk.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hs.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qt.shxzukj.cn

[N04] 斐波那契数列
来源：http://jx.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gd.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nm.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ce.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ye.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hl.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nz.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bk.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ao.haigaiapp.cn

[N05] 最大公约数
来源：http://dj.nszjky.cn

Py:   math.gcd(a, b)
来源：http://dj.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fg.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lo.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tk.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ba.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pj.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://rv.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ab.bjjhwx.cn

[N06] 判断回文字符串
来源：http://fu.yuexingan06.cn

Py:   s == s[::-1]
来源：http://ye.9csxet.cn

PHP:  $s === strrev($s);
来源：http://an.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://tk.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://yl.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://id.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://rq.shtwfgs.cn

Ruby: s == s.reverse
来源：http://hp.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://av.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://bx.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lr.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sg.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vk.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://xi.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://do.colortex.cn

Go:   // 手写 map[int]int
来源：http://xr.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ll.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yy.shxzukj.cn

[N08] 生成全排列
来源：http://tj.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://pa.colortex.cn

PHP:  // 手写递归交换
来源：http://fk.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://kw.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://jc.521024.cn

Java: // 手写回溯递归
来源：http://yw.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://zl.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://be.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ea.newstarts.cn

[N09] 栈与队列
来源：http://di.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nb.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lm.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pe.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hs.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zj.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gu.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fg.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wr.521024.cn

[N10] 链表节点定义
来源：http://qq.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jw.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hp.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cx.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yv.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://nf.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mg.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ct.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uo.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://dw.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ws.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://jf.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zt.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sk.yuntaijiaju.cn

Java: // 手写递归
来源：http://ak.yuexingan06.cn

Go:   // 手写递归
来源：http://ps.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dq.nszjky.cn

C#:   // 手写递归
来源：http://ug.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yx.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vy.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hc.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tg.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xn.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fz.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vb.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://si.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ct.asd995.cn

================================================================================
来源：http://hc.chemitech.net.cn

O. 并发与异步
来源：http://bm.colortex.cn

================================================================================
来源：http://ic.huixiangedu.cn

[O01] 启动一个线程
来源：http://xt.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nh.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cn.gzmigu.cn

TS:   // 同 JS
来源：http://zd.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://hd.muxihuayi.cn

Go:   go f()
来源：http://dw.9csxet.cn

Ruby: Thread.new { f }
来源：http://ac.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://go.9csxet.cn

[O02] 使用线程池
来源：http://vt.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nf.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tm.newstarts.cn

JS:   // worker_threads 线程池
来源：http://kc.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://ym.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fd.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://du.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ms.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xv.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://bg.521024.cn

Py:   with lock: shared += 1
来源：http://vi.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ac.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tv.yuntaijiaju.cn

TS:   // 同 JS
来源：http://uo.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://qi.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xp.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qr.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://ez.newstarts.cn

[O04] 定义异步函数并等待
来源：http://wy.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://nd.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://na.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://uk.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cf.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xg.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://di.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cc.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://db.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://ey.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ry.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ea.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://dw.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://el.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://za.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ba.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://hb.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bf.jctech888.com.cn

[O06] 使用进程池
来源：http://rs.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ql.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hq.colortex.cn

JS:   // child_process / cluster 模块
来源：http://mr.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://ju.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ql.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yk.chemitech.net.cn

Ruby: // fork 块
来源：http://yo.yuntaijiaju.cn

C#:   Parallel.For
来源：http://qo.hahajie.cn

================================================================================
来源：http://ko.bjjhwx.cn

P. 常用工具函数
来源：http://yq.shxzukj.cn

================================================================================
来源：http://bu.chemitech.net.cn

[P01] 生成 UUID
来源：http://xa.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://tp.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://td.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ot.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://bo.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://uc.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://qx.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://eg.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://mm.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://st.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://te.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://es.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ka.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ys.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ck.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ya.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://an.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lg.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://nb.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bu.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ii.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iq.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yf.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bv.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pc.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wl.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rl.szsharing.cn

[P04] 求长度
来源：http://dx.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rz.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://en.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uz.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.521024.cn


<!-- 参考信息 -->