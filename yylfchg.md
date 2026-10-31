代发 wailian999

Py:   resp.json()
来源：http://bn.colortex.cn

PHP:  json_decode($body, true);
来源：http://om.muxihuayi.cn

JS:   await resp.json()
来源：http://im.jianghongdianzi.cn

TS:   await resp.json()
来源：http://mq.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ox.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mh.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://iq.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://bo.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ji.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vs.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ke.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://qn.colortex.cn

Java: resp.statusCode()
来源：http://hy.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ig.hahajie.cn

Ruby: resp.code.to_i
来源：http://lv.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://fv.asd995.cn

[L08] 并发请求多个地址
来源：http://hg.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oc.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://do.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ps.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tx.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zo.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zw.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mp.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jz.shtwfgs.cn

================================================================================
来源：http://sz.521024.cn

M. 命令行 / 进程 / 环境
来源：http://zk.nicolike.cn

================================================================================
来源：http://pq.521024.cn

[M01] 读取命令行参数
来源：http://xz.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ym.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ru.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://wu.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://cn.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://xj.hahajie.cn

Go:   os.Args[1:]
来源：http://lh.haigaiapp.cn

Ruby: ARGV
来源：http://ml.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://bg.chemitech.net.cn

[M02] 读取环境变量
来源：http://vt.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://kf.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tq.szsharing.cn

JS:   process.env.HOME
来源：http://jh.9csxet.cn

TS:   process.env.HOME
来源：http://wm.hnjuh.cn

Java: System.getenv("HOME")
来源：http://je.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ds.colortex.cn

Ruby: ENV["HOME"]
来源：http://fo.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ms.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://qw.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qk.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://be.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tt.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xu.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ib.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fe.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lt.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://pv.huanxung.cn

[M04] 获取当前工作目录
来源：http://ez.szxytkj.cn

Py:   os.getcwd()
来源：http://yn.nszjky.cn

PHP:  getcwd();
来源：http://kl.asd995.cn

JS:   process.cwd()
来源：http://iw.szxytkj.cn

TS:   process.cwd()
来源：http://iy.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://hn.asd995.cn

Go:   os.Getwd()
来源：http://bg.colortex.cn

Ruby: Dir.pwd
来源：http://fp.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ad.huixinmuqiang.cn

[M05] 设置退出码
来源：http://ei.shxzukj.cn

Py:   sys.exit(1)
来源：http://vo.jianghongdianzi.cn

PHP:  exit(1);
来源：http://ge.bookmarksfly.cn

JS:   process.exit(1)
来源：http://sp.asd995.cn

TS:   process.exit(1)
来源：http://qv.huixiangedu.cn

Java: System.exit(1)
来源：http://gq.huixiangedu.cn

Go:   os.Exit(1)
来源：http://fm.yuexingan06.cn

Ruby: exit 1
来源：http://fr.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wy.shxzskj.cn

[M06] 向标准错误输出
来源：http://cn.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://hd.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ae.huanxung.cn

JS:   console.error("err")
来源：http://so.panjiajie.cn

TS:   console.error("err")
来源：http://sc.nszjky.cn

Java: System.err.println("err")
来源：http://lu.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xo.9csxet.cn

Ruby: warn "err"
来源：http://on.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://em.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://gk.521024.cn

Py:   if __name__ == "__main__":
来源：http://hh.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hm.bookmarksfly.cn

JS:   require.main === module
来源：http://fo.nszjky.cn

TS:   require.main === module
来源：http://lk.nszjky.cn

Java: public static void main(String[] args)
来源：http://xp.huixiangedu.cn

Go:   func main()
来源：http://ut.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iy.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://cp.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://fn.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://bh.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://sl.nszjky.cn

JS:   process.platform;  process.version
来源：http://jq.521024.cn

TS:   process.platform;  process.version
来源：http://hp.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ba.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gr.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://id.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jb.huanxung.cn

================================================================================
来源：http://qh.huixinmuqiang.cn

N. 数据结构与算法
来源：http://wi.nszjky.cn

================================================================================
来源：http://pj.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://zq.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ma.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://re.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://be.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cm.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ks.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://bl.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uw.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ei.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://nj.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ua.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pt.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wo.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sd.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://se.nicolike.cn

Ruby: arr.sort
来源：http://hz.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://va.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://fw.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xa.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://uj.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://he.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ui.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yp.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://au.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cj.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uw.gzmigu.cn

[N04] 斐波那契数列
来源：http://nw.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uh.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kk.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eq.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fx.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vy.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kg.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://le.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mo.szsharing.cn

[N05] 最大公约数
来源：http://jz.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://zs.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tm.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vf.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://an.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bv.newstarts.cn

Ruby: a.gcd(b)
来源：http://aq.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://db.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://wk.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://ez.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://uo.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://yp.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://mv.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lb.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://fw.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://hf.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sq.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://qo.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qj.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wk.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wv.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://ye.colortex.cn

Java: // 手写 HashMap
来源：http://yk.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://xc.newstarts.cn

Ruby: // 手写 Hash
来源：http://nm.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sh.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ke.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://gb.colortex.cn

PHP:  // 手写递归交换
来源：http://pl.nicolike.cn

JS:   // 手写回溯递归
来源：http://fh.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://ls.shtwfgs.cn

Java: // 手写回溯递归
来源：http://zm.nicolike.cn

Go:   // 手写回溯递归
来源：http://vs.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://ti.9csxet.cn

C#:   // 手写回溯递归
来源：http://zb.bookmarksfly.cn

[N09] 栈与队列
来源：http://qn.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ct.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ua.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nj.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://au.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dn.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qq.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ew.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rc.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://zg.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hj.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ql.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yn.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lh.asd995.cn

Java: class Node { int v; Node next; }
来源：http://uq.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rt.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hf.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://km.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://zt.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sx.nszjky.cn

PHP:  // 手写递归函数
来源：http://zz.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tg.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ta.lnxyls.cn

Java: // 手写递归
来源：http://ch.nszjky.cn

Go:   // 手写递归
来源：http://mc.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://te.521024.cn

C#:   // 手写递归
来源：http://bo.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vm.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nx.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jh.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vx.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gt.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ro.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://px.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ac.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wu.muxihuayi.cn

================================================================================
来源：http://vg.muxihuayi.cn

O. 并发与异步
来源：http://my.wgjwhj.cn

================================================================================
来源：http://av.hnjuh.cn

[O01] 启动一个线程
来源：http://cf.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ny.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yi.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ib.wgjwhj.cn

TS:   // 同 JS
来源：http://gj.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://ey.jianghongdianzi.cn

Go:   go f()
来源：http://kb.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://db.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://xe.lnxyls.cn

[O02] 使用线程池
来源：http://sh.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yv.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jq.521024.cn

JS:   // worker_threads 线程池
来源：http://nf.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://ej.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pi.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://va.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ke.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://px.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://bn.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ei.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://hn.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yf.yuexingan06.cn

TS:   // 同 JS
来源：http://fy.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://kk.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gj.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rr.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://mh.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ns.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://gc.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vo.9csxet.cn

JS:   async function f() { await g(); }
来源：http://us.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yb.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cj.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xo.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iq.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://iu.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://ih.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://dy.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yq.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://we.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://lc.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gk.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cw.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://ai.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://as.bjjhwx.cn

[O06] 使用进程池
来源：http://sa.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zk.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hs.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://pn.colortex.cn

TS:   // child_process / cluster 模块
来源：http://jw.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rf.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lo.hnjuh.cn

Ruby: // fork 块
来源：http://pq.haigaiapp.cn

C#:   Parallel.For
来源：http://br.lnxyls.cn

================================================================================
来源：http://qv.panjiajie.cn

P. 常用工具函数
来源：http://sb.jctech888.com.cn

================================================================================
来源：http://mr.wgjwhj.cn

[P01] 生成 UUID
来源：http://qn.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://mq.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zm.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://vh.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://mz.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://gl.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://un.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://ne.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://rw.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://gf.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://is.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tr.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ed.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aq.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tn.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rl.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://of.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mv.huanxung.cn

[P03] 生成短随机字符串
来源：http://vs.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ky.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cd.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fe.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lz.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hl.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gh.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rx.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://co.newstarts.cn

[P04] 求长度
来源：http://fa.bookmarksfly.cn


<!-- 参考信息 -->