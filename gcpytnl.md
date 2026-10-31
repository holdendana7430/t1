代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kt.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oa.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://qm.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uh.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://cr.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hj.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nf.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://kz.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://iw.521024.cn

Java: resp.statusCode()
来源：http://el.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ep.hahajie.cn

Ruby: resp.code.to_i
来源：http://lb.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ra.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://pm.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nj.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://al.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kq.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dc.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cm.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://py.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sv.9csxet.cn

================================================================================
来源：http://dt.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://zt.haigaiapp.cn

================================================================================
来源：http://dk.muxihuayi.cn

[M01] 读取命令行参数
来源：http://zd.9csxet.cn

Py:   sys.argv[1:]
来源：http://id.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://tj.newstarts.cn

JS:   process.argv.slice(2)
来源：http://hg.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://nf.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://zs.haigaiapp.cn

Go:   os.Args[1:]
来源：http://nx.yuntaijiaju.cn

Ruby: ARGV
来源：http://ec.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://vk.shxzukj.cn

[M02] 读取环境变量
来源：http://eu.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://zv.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://op.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://mz.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://gj.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ap.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jt.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ff.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.bjjhwx.cn

[M03] 执行外部命令
来源：http://ef.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ib.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pm.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://px.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ym.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ri.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ac.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xa.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://ta.szxytkj.cn

[M04] 获取当前工作目录
来源：http://jp.haigaiapp.cn

Py:   os.getcwd()
来源：http://aw.asd995.cn

PHP:  getcwd();
来源：http://cb.colortex.cn

JS:   process.cwd()
来源：http://vo.szxytkj.cn

TS:   process.cwd()
来源：http://cw.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://qw.shxzskj.cn

Go:   os.Getwd()
来源：http://tl.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://jg.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sv.9csxet.cn

[M05] 设置退出码
来源：http://yx.newstarts.cn

Py:   sys.exit(1)
来源：http://yj.muxihuayi.cn

PHP:  exit(1);
来源：http://cp.bookmarksfly.cn

JS:   process.exit(1)
来源：http://it.newstarts.cn

TS:   process.exit(1)
来源：http://ev.hahajie.cn

Java: System.exit(1)
来源：http://nj.hahajie.cn

Go:   os.Exit(1)
来源：http://rc.hnjuh.cn

Ruby: exit 1
来源：http://xt.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hu.haigaiapp.cn

[M06] 向标准错误输出
来源：http://ls.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://yk.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ye.bookmarksfly.cn

JS:   console.error("err")
来源：http://ot.colortex.cn

TS:   console.error("err")
来源：http://ex.huanxung.cn

Java: System.err.println("err")
来源：http://el.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ty.gzmigu.cn

Ruby: warn "err"
来源：http://dx.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ap.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://qt.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://zg.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sn.yuntaijiaju.cn

JS:   require.main === module
来源：http://yr.gzmigu.cn

TS:   require.main === module
来源：http://xt.hahajie.cn

Java: public static void main(String[] args)
来源：http://sy.yuexingan06.cn

Go:   func main()
来源：http://qg.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jo.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://hg.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://cg.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://ds.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://cy.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://pf.huanxung.cn

TS:   process.platform;  process.version
来源：http://yh.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xa.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zj.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jy.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ly.huanxung.cn

================================================================================
来源：http://zg.bjjhwx.cn

N. 数据结构与算法
来源：http://fj.szxytkj.cn

================================================================================
来源：http://zw.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://cm.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fb.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hm.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://me.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rn.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yh.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://hy.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eq.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mp.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://kp.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ur.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://at.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qc.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oy.szsharing.cn

Go:   slices.Sort(arr)
来源：http://vu.hnjuh.cn

Ruby: arr.sort
来源：http://oy.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xo.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://ke.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hb.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://sd.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://um.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fv.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gf.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iy.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xa.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vl.huanxung.cn

[N04] 斐波那契数列
来源：http://vx.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ga.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vy.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pp.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://az.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wr.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lf.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qd.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hj.lnxyls.cn

[N05] 最大公约数
来源：http://ba.nszjky.cn

Py:   math.gcd(a, b)
来源：http://ju.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zs.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bo.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mw.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ig.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hh.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://rl.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ce.chemitech.net.cn

[N06] 判断回文字符串
来源：http://kj.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://dj.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://jr.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://wp.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://nk.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rn.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://cj.hahajie.cn

Ruby: s == s.reverse
来源：http://dd.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uv.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://kg.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://if.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ag.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sm.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://pc.shxzskj.cn

Java: // 手写 HashMap
来源：http://bt.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://go.asd995.cn

Ruby: // 手写 Hash
来源：http://ql.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tv.521024.cn

[N08] 生成全排列
来源：http://rv.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://er.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://yi.9csxet.cn

JS:   // 手写回溯递归
来源：http://ey.shxzukj.cn

TS:   // 手写回溯递归
来源：http://zv.szxytkj.cn

Java: // 手写回溯递归
来源：http://eq.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://gu.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://kv.521024.cn

C#:   // 手写回溯递归
来源：http://pz.shxzskj.cn

[N09] 栈与队列
来源：http://cn.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kf.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yy.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://db.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ea.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://as.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hl.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ru.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iw.yuexingan06.cn

[N10] 链表节点定义
来源：http://pb.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nc.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ja.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wi.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sz.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://sa.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ua.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jo.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nc.asd995.cn

[N11] 二叉树中序遍历
来源：http://fb.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jo.lnxyls.cn

PHP:  // 手写递归函数
来源：http://fe.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pk.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hp.hahajie.cn

Java: // 手写递归
来源：http://cn.hahajie.cn

Go:   // 手写递归
来源：http://nk.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rr.521024.cn

C#:   // 手写递归
来源：http://me.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ub.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yv.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ta.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ej.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qx.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ji.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xs.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bf.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yk.jctech888.com.cn

================================================================================
来源：http://la.asd995.cn

O. 并发与异步
来源：http://vj.hahajie.cn

================================================================================
来源：http://pr.newstarts.cn

[O01] 启动一个线程
来源：http://qu.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ls.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ns.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pr.nszjky.cn

TS:   // 同 JS
来源：http://vh.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://xz.yuntaijiaju.cn

Go:   go f()
来源：http://yq.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://wc.hahajie.cn

C#:   Task.Run(() => F());
来源：http://bj.huixinmuqiang.cn

[O02] 使用线程池
来源：http://ui.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iw.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ln.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://my.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://zl.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mf.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wm.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qw.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rb.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://sq.hahajie.cn

Py:   with lock: shared += 1
来源：http://yh.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://dg.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fw.nicolike.cn

TS:   // 同 JS
来源：http://ag.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://vj.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nl.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mu.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://wi.colortex.cn

[O04] 定义异步函数并等待
来源：http://dz.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://aq.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ye.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://nz.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hm.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xg.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sd.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pb.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://cx.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://rv.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://sq.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pt.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://fd.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://ti.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ei.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ks.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://ya.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cx.asd995.cn

[O06] 使用进程池
来源：http://os.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ly.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ps.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://qm.colortex.cn

TS:   // child_process / cluster 模块
来源：http://tu.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mc.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dv.shxzukj.cn

Ruby: // fork 块
来源：http://ye.muxihuayi.cn

C#:   Parallel.For
来源：http://ib.bjjhwx.cn

================================================================================
来源：http://hb.jianghongdianzi.cn

P. 常用工具函数
来源：http://yq.panjiajie.cn

================================================================================
来源：http://yq.huanxung.cn

[P01] 生成 UUID
来源：http://sn.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://bu.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ld.huanxung.cn

JS:   crypto.randomUUID()
来源：http://er.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://rl.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://of.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://qo.colortex.cn

Ruby: SecureRandom.uuid
来源：http://iw.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://bu.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://qx.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cm.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hu.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lb.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ef.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://op.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mf.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rm.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pa.panjiajie.cn

[P03] 生成短随机字符串
来源：http://bw.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kx.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ed.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zb.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hw.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yv.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ox.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vz.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bt.9csxet.cn

[P04] 求长度
来源：http://cw.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://da.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kl.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qy.newstarts.cn


<!-- 参考信息 -->