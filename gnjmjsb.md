代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://yw.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fi.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hf.colortex.cn

JS:   resp.ok;  resp.status
来源：http://oc.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://xu.shxzskj.cn

Java: resp.statusCode()
来源：http://wu.hahajie.cn

Go:   resp.StatusCode
来源：http://of.asd995.cn

Ruby: resp.code.to_i
来源：http://fy.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://mu.nicolike.cn

[L08] 并发请求多个地址
来源：http://jp.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://az.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://nl.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bb.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bm.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://go.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xf.9csxet.cn

================================================================================
来源：http://aa.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://rj.wgjwhj.cn

================================================================================
来源：http://nk.muxihuayi.cn

[M01] 读取命令行参数
来源：http://lh.nszjky.cn

Py:   sys.argv[1:]
来源：http://la.nicolike.cn

PHP:  $argv;  $argc;
来源：http://go.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://nt.asd995.cn

TS:   process.argv.slice(2)
来源：http://xg.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://gz.nszjky.cn

Go:   os.Args[1:]
来源：http://xc.yuexingan06.cn

Ruby: ARGV
来源：http://kk.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://ni.gzmigu.cn

[M02] 读取环境变量
来源：http://lv.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://zb.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yx.wgjwhj.cn

JS:   process.env.HOME
来源：http://ed.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://ab.colortex.cn

Java: System.getenv("HOME")
来源：http://hq.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ix.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://vt.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uw.bookmarksfly.cn

[M03] 执行外部命令
来源：http://zn.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://en.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yi.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jo.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ia.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fm.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://la.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nf.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://ww.hahajie.cn

[M04] 获取当前工作目录
来源：http://ds.nicolike.cn

Py:   os.getcwd()
来源：http://sa.muxihuayi.cn

PHP:  getcwd();
来源：http://ne.yuexingan06.cn

JS:   process.cwd()
来源：http://vf.shtwfgs.cn

TS:   process.cwd()
来源：http://vm.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://uy.huixiangedu.cn

Go:   os.Getwd()
来源：http://gu.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://yd.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jy.colortex.cn

[M05] 设置退出码
来源：http://eq.colortex.cn

Py:   sys.exit(1)
来源：http://sh.nicolike.cn

PHP:  exit(1);
来源：http://cb.newstarts.cn

JS:   process.exit(1)
来源：http://ud.bookmarksfly.cn

TS:   process.exit(1)
来源：http://in.asd995.cn

Java: System.exit(1)
来源：http://hs.szxytkj.cn

Go:   os.Exit(1)
来源：http://eb.bjjhwx.cn

Ruby: exit 1
来源：http://nq.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tc.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ej.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://io.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cp.gzmigu.cn

JS:   console.error("err")
来源：http://ym.haigaiapp.cn

TS:   console.error("err")
来源：http://vm.asd995.cn

Java: System.err.println("err")
来源：http://cf.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kv.yuntaijiaju.cn

Ruby: warn "err"
来源：http://gd.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://dn.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://zs.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://rm.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oe.hahajie.cn

JS:   require.main === module
来源：http://sl.jianghongdianzi.cn

TS:   require.main === module
来源：http://st.szxytkj.cn

Java: public static void main(String[] args)
来源：http://nz.shxzukj.cn

Go:   func main()
来源：http://zx.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jj.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://on.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://pp.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://rf.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://du.9csxet.cn

JS:   process.platform;  process.version
来源：http://at.newstarts.cn

TS:   process.platform;  process.version
来源：http://dq.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vj.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fo.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sv.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ff.nicolike.cn

================================================================================
来源：http://gq.bjjhwx.cn

N. 数据结构与算法
来源：http://qy.shxzukj.cn

================================================================================
来源：http://wa.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://dv.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kb.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qs.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://je.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nb.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cn.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://qu.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hl.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jt.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://mu.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://os.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ao.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jf.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://no.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gt.szsharing.cn

Go:   slices.Sort(arr)
来源：http://ad.wgjwhj.cn

Ruby: arr.sort
来源：http://dv.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iy.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://nn.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qz.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://io.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ja.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gh.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dq.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aj.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ik.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qg.asd995.cn

[N04] 斐波那契数列
来源：http://wj.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dr.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zf.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ta.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bv.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tr.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vb.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cv.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jm.lnxyls.cn

[N05] 最大公约数
来源：http://zi.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://pk.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://um.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uc.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tg.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nl.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qj.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://gg.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pn.9csxet.cn

[N06] 判断回文字符串
来源：http://md.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://xk.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://ur.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://dg.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://hg.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ek.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://fs.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://zd.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lw.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://dr.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gw.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lj.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ug.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://zs.jctech888.com.cn

Java: // 手写 HashMap
来源：http://yo.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://ha.asd995.cn

Ruby: // 手写 Hash
来源：http://tz.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://co.jianghongdianzi.cn

[N08] 生成全排列
来源：http://zg.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ya.asd995.cn

PHP:  // 手写递归交换
来源：http://tv.huanxung.cn

JS:   // 手写回溯递归
来源：http://il.9csxet.cn

TS:   // 手写回溯递归
来源：http://vq.jctech888.com.cn

Java: // 手写回溯递归
来源：http://dx.521024.cn

Go:   // 手写回溯递归
来源：http://ss.colortex.cn

Ruby: arr.permutation.to_a
来源：http://em.colortex.cn

C#:   // 手写回溯递归
来源：http://do.shxzskj.cn

[N09] 栈与队列
来源：http://eg.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ry.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nw.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pd.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nt.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://on.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zj.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ch.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lo.huanxung.cn

[N10] 链表节点定义
来源：http://lh.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jt.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cr.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kv.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hh.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://sp.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bv.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zo.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wl.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ba.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sv.521024.cn

PHP:  // 手写递归函数
来源：http://bw.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lh.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ji.huixinmuqiang.cn

Java: // 手写递归
来源：http://uz.huixiangedu.cn

Go:   // 手写递归
来源：http://ft.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kp.szsharing.cn

C#:   // 手写递归
来源：http://tb.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sy.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rx.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gr.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://du.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vl.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ku.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://te.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://db.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nt.panjiajie.cn

================================================================================
来源：http://oj.nszjky.cn

O. 并发与异步
来源：http://er.jianghongdianzi.cn

================================================================================
来源：http://sk.szsharing.cn

[O01] 启动一个线程
来源：http://nc.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jl.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rr.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dg.nszjky.cn

TS:   // 同 JS
来源：http://gr.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://sn.haigaiapp.cn

Go:   go f()
来源：http://qz.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://mb.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://hy.shxzukj.cn

[O02] 使用线程池
来源：http://kx.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fq.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yj.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://tx.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://ei.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xe.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zy.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hx.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ua.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://tt.shxzskj.cn

Py:   with lock: shared += 1
来源：http://cz.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://th.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hr.colortex.cn

TS:   // 同 JS
来源：http://kf.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://km.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xu.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nt.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://gb.hahajie.cn

[O04] 定义异步函数并等待
来源：http://dd.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://dv.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ah.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://ez.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lb.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dd.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wi.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fa.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://hs.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://bs.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ow.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cs.521024.cn

JS:   await Promise.all(tasks)
来源：http://zt.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://jx.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ug.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qk.colortex.cn

Ruby: threads.map(&:join)
来源：http://dd.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cb.huanxung.cn

[O06] 使用进程池
来源：http://mb.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ut.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bx.colortex.cn

JS:   // child_process / cluster 模块
来源：http://xd.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://ps.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wl.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ba.szsharing.cn

Ruby: // fork 块
来源：http://gi.yuexingan06.cn

C#:   Parallel.For
来源：http://en.haigaiapp.cn

================================================================================
来源：http://tv.hnjuh.cn

P. 常用工具函数
来源：http://xk.nicolike.cn

================================================================================
来源：http://jb.nicolike.cn

[P01] 生成 UUID
来源：http://ge.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://hw.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hc.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://ud.9csxet.cn

TS:   crypto.randomUUID()
来源：http://bl.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://zj.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://hj.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://hn.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://qk.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://du.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hn.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://co.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sw.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qp.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bf.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tc.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pd.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zv.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://gm.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bf.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yl.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yt.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zz.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nv.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://om.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://de.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vc.panjiajie.cn

[P04] 求长度
来源：http://yo.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ib.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lo.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cv.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://it.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://in.521024.cn

Go:   len(arr);  len(m)
来源：http://rm.nszjky.cn

Ruby: x.length;  x.size
来源：http://eb.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kx.shtwfgs.cn


<!-- 参考信息 -->