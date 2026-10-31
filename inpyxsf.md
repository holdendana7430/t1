代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://do.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nw.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ge.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://jp.colortex.cn

TS:   resp.ok;  resp.status
来源：http://cd.haigaiapp.cn

Java: resp.statusCode()
来源：http://qg.newstarts.cn

Go:   resp.StatusCode
来源：http://wg.colortex.cn

Ruby: resp.code.to_i
来源：http://ng.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://fb.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://vk.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://to.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://mi.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xz.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ty.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ux.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://la.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ti.muxihuayi.cn

================================================================================
来源：http://vi.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://jh.newstarts.cn

================================================================================
来源：http://rq.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://pw.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://st.colortex.cn

PHP:  $argv;  $argc;
来源：http://px.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://dm.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ug.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://wr.panjiajie.cn

Go:   os.Args[1:]
来源：http://qq.yuexingan06.cn

Ruby: ARGV
来源：http://om.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://aq.szsharing.cn

[M02] 读取环境变量
来源：http://py.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://hw.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pt.lnxyls.cn

JS:   process.env.HOME
来源：http://kd.szxytkj.cn

TS:   process.env.HOME
来源：http://yk.nszjky.cn

Java: System.getenv("HOME")
来源：http://fk.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://so.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://px.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wm.nszjky.cn

[M03] 执行外部命令
来源：http://bq.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ta.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ff.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hy.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ny.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gz.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xq.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rr.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ei.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://va.wgjwhj.cn

Py:   os.getcwd()
来源：http://cy.nszjky.cn

PHP:  getcwd();
来源：http://kb.huixinmuqiang.cn

JS:   process.cwd()
来源：http://um.panjiajie.cn

TS:   process.cwd()
来源：http://eh.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://em.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ep.bjjhwx.cn

Ruby: Dir.pwd
来源：http://iy.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sz.huixiangedu.cn

[M05] 设置退出码
来源：http://uz.hnjuh.cn

Py:   sys.exit(1)
来源：http://up.huanxung.cn

PHP:  exit(1);
来源：http://yp.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ua.szsharing.cn

TS:   process.exit(1)
来源：http://tk.szsharing.cn

Java: System.exit(1)
来源：http://sp.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://jg.nicolike.cn

Ruby: exit 1
来源：http://ur.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sk.chemitech.net.cn

[M06] 向标准错误输出
来源：http://hk.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://yq.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ao.newstarts.cn

JS:   console.error("err")
来源：http://ri.colortex.cn

TS:   console.error("err")
来源：http://dl.nicolike.cn

Java: System.err.println("err")
来源：http://mv.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wp.chemitech.net.cn

Ruby: warn "err"
来源：http://gb.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://cd.asd995.cn

[M07] 判断是否为主入口
来源：http://ur.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://gg.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zn.lnxyls.cn

JS:   require.main === module
来源：http://dy.szxytkj.cn

TS:   require.main === module
来源：http://ps.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://fb.hnjuh.cn

Go:   func main()
来源：http://on.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rw.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://dc.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ll.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://cg.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://ot.hnjuh.cn

JS:   process.platform;  process.version
来源：http://af.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://ll.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rx.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dg.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://os.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ti.huixiangedu.cn

================================================================================
来源：http://vq.wgjwhj.cn

N. 数据结构与算法
来源：http://ei.haigaiapp.cn

================================================================================
来源：http://vt.521024.cn

[N01] 二分查找（有序数组）
来源：http://vc.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ei.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kt.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ou.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iq.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yy.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://df.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iv.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qg.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ss.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sw.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jp.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vg.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://os.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ul.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://ea.yuexingan06.cn

Ruby: arr.sort
来源：http://np.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tl.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://jy.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gt.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://gs.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nb.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nj.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rd.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ak.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yd.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jh.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://uo.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iz.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ve.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lx.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yd.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://il.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tu.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wc.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tt.huanxung.cn

[N05] 最大公约数
来源：http://nc.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://px.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://is.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dx.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sp.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wx.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gk.521024.cn

Ruby: a.gcd(b)
来源：http://uu.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nc.lnxyls.cn

[N06] 判断回文字符串
来源：http://fy.newstarts.cn

Py:   s == s[::-1]
来源：http://pb.hahajie.cn

PHP:  $s === strrev($s);
来源：http://xz.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://lb.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://vk.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bk.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://mb.jctech888.com.cn

Ruby: s == s.reverse
来源：http://fb.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kz.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://fo.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wy.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xl.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://of.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ye.newstarts.cn

Java: // 手写 HashMap
来源：http://nb.hahajie.cn

Go:   // 手写 map[int]int
来源：http://qi.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ym.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://do.szxytkj.cn

[N08] 生成全排列
来源：http://ir.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://vy.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://vx.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://lb.521024.cn

TS:   // 手写回溯递归
来源：http://ai.szxytkj.cn

Java: // 手写回溯递归
来源：http://gr.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://mr.colortex.cn

Ruby: arr.permutation.to_a
来源：http://uw.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://nl.nicolike.cn

[N09] 栈与队列
来源：http://ve.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ae.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zt.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ay.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mi.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fc.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nj.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.huanxung.cn

[N10] 链表节点定义
来源：http://yb.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yb.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uz.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ft.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lb.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://su.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ua.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kb.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://en.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://gh.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ls.asd995.cn

PHP:  // 手写递归函数
来源：http://ch.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ye.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ig.shxzskj.cn

Java: // 手写递归
来源：http://ni.szsharing.cn

Go:   // 手写递归
来源：http://bd.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dq.chemitech.net.cn

C#:   // 手写递归
来源：http://xv.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tr.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dw.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fh.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bk.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ie.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sz.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tc.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wc.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kr.shtwfgs.cn

================================================================================
来源：http://ll.yuntaijiaju.cn

O. 并发与异步
来源：http://gs.bookmarksfly.cn

================================================================================
来源：http://vr.panjiajie.cn

[O01] 启动一个线程
来源：http://tn.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://if.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cv.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xf.shtwfgs.cn

TS:   // 同 JS
来源：http://ra.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://ik.shxzukj.cn

Go:   go f()
来源：http://on.lnxyls.cn

Ruby: Thread.new { f }
来源：http://sg.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://iq.9csxet.cn

[O02] 使用线程池
来源：http://by.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vf.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jw.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://xh.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://cb.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yo.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ne.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nv.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yi.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://hr.panjiajie.cn

Py:   with lock: shared += 1
来源：http://ty.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://it.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ev.wgjwhj.cn

TS:   // 同 JS
来源：http://bw.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://un.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ts.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ga.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://lg.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://qv.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://dt.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ki.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ch.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qc.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gt.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ar.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ko.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://jn.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://bb.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://gi.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tx.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://nh.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://oi.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fp.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mk.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://vz.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sj.chemitech.net.cn

[O06] 使用进程池
来源：http://ke.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dw.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ns.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://wo.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://aq.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zd.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dm.wgjwhj.cn

Ruby: // fork 块
来源：http://ca.jianghongdianzi.cn

C#:   Parallel.For
来源：http://tj.hnjuh.cn

================================================================================
来源：http://xx.szxytkj.cn

P. 常用工具函数
来源：http://hu.jianghongdianzi.cn

================================================================================
来源：http://dh.panjiajie.cn

[P01] 生成 UUID
来源：http://mo.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://ch.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lc.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://fb.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://tn.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://vq.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://dn.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ho.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://va.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://dv.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bg.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pf.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gf.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kq.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dw.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dm.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hu.hahajie.cn

[P03] 生成短随机字符串
来源：http://dh.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://af.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://if.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ow.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vk.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vj.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sm.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vl.newstarts.cn

[P04] 求长度
来源：http://nl.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cb.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cl.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://gt.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ae.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://kj.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hn.muxihuayi.cn


<!-- 参考信息 -->