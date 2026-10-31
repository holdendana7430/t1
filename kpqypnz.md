代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ti.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rr.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://uo.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dm.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://tn.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fy.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ae.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://an.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://mp.newstarts.cn

Java: resp.statusCode()
来源：http://qm.panjiajie.cn

Go:   resp.StatusCode
来源：http://jf.9csxet.cn

Ruby: resp.code.to_i
来源：http://rc.521024.cn

C#:   (int)resp.StatusCode
来源：http://db.lnxyls.cn

[L08] 并发请求多个地址
来源：http://rd.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jc.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://ue.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pz.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://on.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uz.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iv.asd995.cn

================================================================================
来源：http://rq.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://kw.haigaiapp.cn

================================================================================
来源：http://ul.nszjky.cn

[M01] 读取命令行参数
来源：http://lv.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ts.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://rm.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://bb.newstarts.cn

TS:   process.argv.slice(2)
来源：http://aa.asd995.cn

Java: args 数组（main 方法参数）
来源：http://et.huixiangedu.cn

Go:   os.Args[1:]
来源：http://vt.muxihuayi.cn

Ruby: ARGV
来源：http://eo.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://cm.shxzukj.cn

[M02] 读取环境变量
来源：http://aj.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://jp.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jm.newstarts.cn

JS:   process.env.HOME
来源：http://ji.hnjuh.cn

TS:   process.env.HOME
来源：http://jq.hnjuh.cn

Java: System.getenv("HOME")
来源：http://kl.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ip.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://iq.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fg.huanxung.cn

[M03] 执行外部命令
来源：http://ho.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zu.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vo.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hc.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tp.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tv.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fr.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gp.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://is.nszjky.cn

[M04] 获取当前工作目录
来源：http://yb.colortex.cn

Py:   os.getcwd()
来源：http://gd.szxytkj.cn

PHP:  getcwd();
来源：http://ey.colortex.cn

JS:   process.cwd()
来源：http://eb.jctech888.com.cn

TS:   process.cwd()
来源：http://el.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://nl.haigaiapp.cn

Go:   os.Getwd()
来源：http://fn.newstarts.cn

Ruby: Dir.pwd
来源：http://cv.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ia.hnjuh.cn

[M05] 设置退出码
来源：http://pb.haigaiapp.cn

Py:   sys.exit(1)
来源：http://fl.haigaiapp.cn

PHP:  exit(1);
来源：http://cv.wgjwhj.cn

JS:   process.exit(1)
来源：http://xf.nszjky.cn

TS:   process.exit(1)
来源：http://wj.gzmigu.cn

Java: System.exit(1)
来源：http://ys.huixiangedu.cn

Go:   os.Exit(1)
来源：http://za.wgjwhj.cn

Ruby: exit 1
来源：http://xy.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://to.newstarts.cn

[M06] 向标准错误输出
来源：http://cr.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://ek.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ol.muxihuayi.cn

JS:   console.error("err")
来源：http://np.bookmarksfly.cn

TS:   console.error("err")
来源：http://hk.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ue.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://li.shxzskj.cn

Ruby: warn "err"
来源：http://fv.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ig.asd995.cn

[M07] 判断是否为主入口
来源：http://mh.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://vx.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sx.9csxet.cn

JS:   require.main === module
来源：http://ha.huixinmuqiang.cn

TS:   require.main === module
来源：http://sk.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://xv.shxzskj.cn

Go:   func main()
来源：http://iz.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dg.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://ba.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://oq.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://pr.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://sz.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://xq.gzmigu.cn

TS:   process.platform;  process.version
来源：http://tj.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wk.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wh.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jk.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gn.bookmarksfly.cn

================================================================================
来源：http://uy.bookmarksfly.cn

N. 数据结构与算法
来源：http://tt.szsharing.cn

================================================================================
来源：http://fr.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://vf.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://la.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zu.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ej.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vy.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gf.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://no.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://je.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://of.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://cu.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://cy.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bn.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jl.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://it.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hh.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://xj.szxytkj.cn

Ruby: arr.sort
来源：http://xn.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mr.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://jt.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cy.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://yh.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cs.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yg.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ce.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ph.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aj.9csxet.cn

[N04] 斐波那契数列
来源：http://dw.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://im.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dz.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vj.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eg.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ni.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jp.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pk.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fp.lnxyls.cn

[N05] 最大公约数
来源：http://nr.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ga.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://it.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oj.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pm.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lq.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gu.lnxyls.cn

Ruby: a.gcd(b)
来源：http://xb.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gy.jctech888.com.cn

[N06] 判断回文字符串
来源：http://fw.muxihuayi.cn

Py:   s == s[::-1]
来源：http://ro.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://eq.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://wp.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://qm.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sj.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ao.jctech888.com.cn

Ruby: s == s.reverse
来源：http://hl.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ky.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://zy.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cq.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jy.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pk.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://qb.colortex.cn

Java: // 手写 HashMap
来源：http://ad.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://kk.lnxyls.cn

Ruby: // 手写 Hash
来源：http://rt.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://za.shtwfgs.cn

[N08] 生成全排列
来源：http://av.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://jw.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://rv.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://qe.hnjuh.cn

TS:   // 手写回溯递归
来源：http://rw.szsharing.cn

Java: // 手写回溯递归
来源：http://ht.szsharing.cn

Go:   // 手写回溯递归
来源：http://ao.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://si.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://qx.wgjwhj.cn

[N09] 栈与队列
来源：http://xk.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xg.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rt.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rp.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kv.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hv.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gx.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rf.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://je.shxzskj.cn

[N10] 链表节点定义
来源：http://ns.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ip.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://di.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lp.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qw.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://ru.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bb.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vu.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pj.hahajie.cn

[N11] 二叉树中序遍历
来源：http://aa.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gj.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://zu.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nn.jianghongdianzi.cn

Java: // 手写递归
来源：http://ja.huixiangedu.cn

Go:   // 手写递归
来源：http://fk.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ff.yuntaijiaju.cn

C#:   // 手写递归
来源：http://od.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jg.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jo.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ac.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vs.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dp.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ok.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dx.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ck.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.yuexingan06.cn

================================================================================
来源：http://eo.bookmarksfly.cn

O. 并发与异步
来源：http://yd.yuexingan06.cn

================================================================================
来源：http://ei.lnxyls.cn

[O01] 启动一个线程
来源：http://wg.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dh.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://he.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sy.wgjwhj.cn

TS:   // 同 JS
来源：http://xv.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://in.newstarts.cn

Go:   go f()
来源：http://po.nszjky.cn

Ruby: Thread.new { f }
来源：http://pe.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://to.9csxet.cn

[O02] 使用线程池
来源：http://fh.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ql.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lz.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://lm.newstarts.cn

TS:   // worker_threads 线程池
来源：http://rt.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lj.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cs.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ng.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hp.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://uy.szxytkj.cn

Py:   with lock: shared += 1
来源：http://xc.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://jr.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sj.muxihuayi.cn

TS:   // 同 JS
来源：http://ql.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://xd.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wi.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kd.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://my.newstarts.cn

[O04] 定义异步函数并等待
来源：http://fy.colortex.cn

Py:   async def f():⏎    await g()
来源：http://bp.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ir.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://yq.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cs.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oh.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mp.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bs.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://tb.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://ct.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://sm.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hl.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://on.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://sn.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rh.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://be.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://bg.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oo.asd995.cn

[O06] 使用进程池
来源：http://dd.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ov.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sc.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://yi.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://da.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xl.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aw.bjjhwx.cn

Ruby: // fork 块
来源：http://mc.yuexingan06.cn

C#:   Parallel.For
来源：http://ql.muxihuayi.cn

================================================================================
来源：http://th.chemitech.net.cn

P. 常用工具函数
来源：http://ph.shtwfgs.cn

================================================================================
来源：http://mk.nicolike.cn

[P01] 生成 UUID
来源：http://ck.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://qf.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bo.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://ok.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://my.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://vz.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://oe.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://ty.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://hl.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://id.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cj.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tn.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://co.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lw.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hj.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eb.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fv.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ez.hahajie.cn

[P03] 生成短随机字符串
来源：http://sl.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ii.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nb.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wy.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xb.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://te.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rd.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fm.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fo.yuntaijiaju.cn

[P04] 求长度
来源：http://me.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yq.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tg.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xf.nicolike.cn


<!-- 参考信息 -->