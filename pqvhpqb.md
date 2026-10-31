代发 wailian999

TS:   resp.ok;  resp.status
来源：http://tq.szxytkj.cn

Java: resp.statusCode()
来源：http://ft.newstarts.cn

Go:   resp.StatusCode
来源：http://eo.newstarts.cn

Ruby: resp.code.to_i
来源：http://tx.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://np.gzmigu.cn

[L08] 并发请求多个地址
来源：http://yg.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oc.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://gr.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ra.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://en.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ug.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fp.hnjuh.cn

================================================================================
来源：http://kw.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://fx.jianghongdianzi.cn

================================================================================
来源：http://yb.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://bu.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://xh.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://ed.newstarts.cn

JS:   process.argv.slice(2)
来源：http://rm.colortex.cn

TS:   process.argv.slice(2)
来源：http://ay.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://wx.yuexingan06.cn

Go:   os.Args[1:]
来源：http://cw.colortex.cn

Ruby: ARGV
来源：http://lv.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://gh.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://vg.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://et.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cb.szxytkj.cn

JS:   process.env.HOME
来源：http://nt.huanxung.cn

TS:   process.env.HOME
来源：http://ap.szxytkj.cn

Java: System.getenv("HOME")
来源：http://yr.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jd.huanxung.cn

Ruby: ENV["HOME"]
来源：http://gz.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tz.huixiangedu.cn

[M03] 执行外部命令
来源：http://nf.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mp.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hd.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pv.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yb.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wi.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hv.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://br.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://fs.hnjuh.cn

Py:   os.getcwd()
来源：http://ur.521024.cn

PHP:  getcwd();
来源：http://gr.nicolike.cn

JS:   process.cwd()
来源：http://th.asd995.cn

TS:   process.cwd()
来源：http://mv.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://st.asd995.cn

Go:   os.Getwd()
来源：http://jy.colortex.cn

Ruby: Dir.pwd
来源：http://rg.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ep.bjjhwx.cn

[M05] 设置退出码
来源：http://ow.nszjky.cn

Py:   sys.exit(1)
来源：http://lw.huixiangedu.cn

PHP:  exit(1);
来源：http://dk.colortex.cn

JS:   process.exit(1)
来源：http://ry.bookmarksfly.cn

TS:   process.exit(1)
来源：http://sj.muxihuayi.cn

Java: System.exit(1)
来源：http://pf.521024.cn

Go:   os.Exit(1)
来源：http://sq.lnxyls.cn

Ruby: exit 1
来源：http://mi.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tt.colortex.cn

[M06] 向标准错误输出
来源：http://vj.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wa.shxzukj.cn

JS:   console.error("err")
来源：http://hs.lnxyls.cn

TS:   console.error("err")
来源：http://xz.newstarts.cn

Java: System.err.println("err")
来源：http://za.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tx.asd995.cn

Ruby: warn "err"
来源：http://pu.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ef.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://rm.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://li.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bv.shxzskj.cn

JS:   require.main === module
来源：http://wf.hahajie.cn

TS:   require.main === module
来源：http://dt.lnxyls.cn

Java: public static void main(String[] args)
来源：http://yz.muxihuayi.cn

Go:   func main()
来源：http://mx.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ym.asd995.cn

C#:   static void Main(string[] args)
来源：http://jx.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://pt.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://tp.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://dk.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://rz.colortex.cn

TS:   process.platform;  process.version
来源：http://mw.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nq.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mb.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ao.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oi.jctech888.com.cn

================================================================================
来源：http://je.yuexingan06.cn

N. 数据结构与算法
来源：http://fz.colortex.cn

================================================================================
来源：http://ql.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ya.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ia.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ae.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wr.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kx.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://hj.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lp.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hc.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ta.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dr.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tc.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ib.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ks.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://op.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ir.haigaiapp.cn

Ruby: arr.sort
来源：http://up.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://en.colortex.cn

[N03] 快速排序（分治示例）
来源：http://ep.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yn.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://mr.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://we.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ty.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rf.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zb.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uz.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mk.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://mo.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://is.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sm.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://md.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qb.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pm.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wm.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://re.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ze.huixiangedu.cn

[N05] 最大公约数
来源：http://kv.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://fy.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ya.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ds.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mj.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vo.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cl.huanxung.cn

Ruby: a.gcd(b)
来源：http://bu.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://np.szsharing.cn

[N06] 判断回文字符串
来源：http://fl.shxzukj.cn

Py:   s == s[::-1]
来源：http://ct.521024.cn

PHP:  $s === strrev($s);
来源：http://xu.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://xn.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://il.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oo.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://fe.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://wd.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wh.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://zn.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zb.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rp.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qh.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://hj.nicolike.cn

Java: // 手写 HashMap
来源：http://kr.521024.cn

Go:   // 手写 map[int]int
来源：http://ku.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://ep.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vy.szxytkj.cn

[N08] 生成全排列
来源：http://fu.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://kz.gzmigu.cn

PHP:  // 手写递归交换
来源：http://hh.lnxyls.cn

JS:   // 手写回溯递归
来源：http://uo.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://es.wgjwhj.cn

Java: // 手写回溯递归
来源：http://rn.newstarts.cn

Go:   // 手写回溯递归
来源：http://jr.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://bf.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://jy.huixinmuqiang.cn

[N09] 栈与队列
来源：http://vh.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mu.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aw.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xi.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ok.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rp.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pr.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jm.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oe.jctech888.com.cn

[N10] 链表节点定义
来源：http://jr.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ok.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://co.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rl.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zq.colortex.cn

Java: class Node { int v; Node next; }
来源：http://be.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://im.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tm.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://md.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://hs.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sh.hnjuh.cn

PHP:  // 手写递归函数
来源：http://ap.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://co.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://id.bookmarksfly.cn

Java: // 手写递归
来源：http://ws.huanxung.cn

Go:   // 手写递归
来源：http://zu.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mi.nszjky.cn

C#:   // 手写递归
来源：http://sf.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jd.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qe.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vp.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ak.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eu.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uu.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nl.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zb.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jv.9csxet.cn

================================================================================
来源：http://ls.chemitech.net.cn

O. 并发与异步
来源：http://he.shtwfgs.cn

================================================================================
来源：http://dt.szxytkj.cn

[O01] 启动一个线程
来源：http://zx.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gl.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jh.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bd.muxihuayi.cn

TS:   // 同 JS
来源：http://ll.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://zg.shtwfgs.cn

Go:   go f()
来源：http://jj.521024.cn

Ruby: Thread.new { f }
来源：http://vz.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://sa.asd995.cn

[O02] 使用线程池
来源：http://td.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kz.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bb.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://hv.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://zr.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zx.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mw.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qc.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hx.nszjky.cn

[O03] 加锁保护共享数据
来源：http://yh.hnjuh.cn

Py:   with lock: shared += 1
来源：http://pn.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://gm.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ny.asd995.cn

TS:   // 同 JS
来源：http://ei.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://fd.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bd.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sq.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://zh.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://wu.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://ep.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fc.nicolike.cn

JS:   async function f() { await g(); }
来源：http://px.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gz.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://of.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://km.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tm.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://hk.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://kr.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ha.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ub.colortex.cn

JS:   await Promise.all(tasks)
来源：http://gw.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://kq.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fs.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pl.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://cz.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yo.wgjwhj.cn

[O06] 使用进程池
来源：http://il.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://to.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bg.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://vn.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://qs.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://li.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wn.wgjwhj.cn

Ruby: // fork 块
来源：http://ya.huixinmuqiang.cn

C#:   Parallel.For
来源：http://if.muxihuayi.cn

================================================================================
来源：http://dz.nicolike.cn

P. 常用工具函数
来源：http://xd.9csxet.cn

================================================================================
来源：http://ad.chemitech.net.cn

[P01] 生成 UUID
来源：http://ej.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://pa.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pj.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://lr.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://ix.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://xy.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://xa.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://yv.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://dt.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://ah.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ls.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ti.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hg.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wo.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kk.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zc.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rc.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ud.hnjuh.cn

[P03] 生成短随机字符串
来源：http://dy.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://za.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://su.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tq.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yz.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ii.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gr.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://al.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gm.hahajie.cn

[P04] 求长度
来源：http://lu.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fj.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nc.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lo.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ai.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://ys.szsharing.cn

Go:   len(arr);  len(m)
来源：http://rg.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://nn.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mw.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://sa.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ff.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yb.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://je.yuntaijiaju.cn


<!-- 参考信息 -->