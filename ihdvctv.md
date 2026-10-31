代发 wailian999

C#:   (int)resp.StatusCode
来源：http://ak.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://wv.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gt.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://gm.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nx.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lp.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nn.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ft.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pc.bjjhwx.cn

================================================================================
来源：http://yc.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://cu.huixinmuqiang.cn

================================================================================
来源：http://oq.huanxung.cn

[M01] 读取命令行参数
来源：http://rl.lnxyls.cn

Py:   sys.argv[1:]
来源：http://lt.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://un.nszjky.cn

JS:   process.argv.slice(2)
来源：http://zr.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://il.521024.cn

Java: args 数组（main 方法参数）
来源：http://tf.chemitech.net.cn

Go:   os.Args[1:]
来源：http://fi.hnjuh.cn

Ruby: ARGV
来源：http://cm.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://wi.shxzskj.cn

[M02] 读取环境变量
来源：http://vs.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://to.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tq.haigaiapp.cn

JS:   process.env.HOME
来源：http://zf.jctech888.com.cn

TS:   process.env.HOME
来源：http://if.szxytkj.cn

Java: System.getenv("HOME")
来源：http://bq.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jt.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://lt.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wi.chemitech.net.cn

[M03] 执行外部命令
来源：http://uu.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pe.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cj.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://db.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nn.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vf.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bm.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yp.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://ct.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://or.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://cx.newstarts.cn

PHP:  getcwd();
来源：http://dp.lnxyls.cn

JS:   process.cwd()
来源：http://hd.shxzukj.cn

TS:   process.cwd()
来源：http://kn.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://vc.shxzukj.cn

Go:   os.Getwd()
来源：http://lh.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://bu.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://md.yuntaijiaju.cn

[M05] 设置退出码
来源：http://hc.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://ex.nszjky.cn

PHP:  exit(1);
来源：http://bx.shxzukj.cn

JS:   process.exit(1)
来源：http://gj.bjjhwx.cn

TS:   process.exit(1)
来源：http://wt.jctech888.com.cn

Java: System.exit(1)
来源：http://ee.muxihuayi.cn

Go:   os.Exit(1)
来源：http://sb.panjiajie.cn

Ruby: exit 1
来源：http://ao.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bs.yuexingan06.cn

[M06] 向标准错误输出
来源：http://vl.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://hu.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bp.hahajie.cn

JS:   console.error("err")
来源：http://df.wgjwhj.cn

TS:   console.error("err")
来源：http://yu.chemitech.net.cn

Java: System.err.println("err")
来源：http://xv.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qk.szxytkj.cn

Ruby: warn "err"
来源：http://mr.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://oa.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://om.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://yh.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nj.lnxyls.cn

JS:   require.main === module
来源：http://sv.shxzskj.cn

TS:   require.main === module
来源：http://zy.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://zb.colortex.cn

Go:   func main()
来源：http://pu.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xi.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://jj.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://hw.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://eo.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ru.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://iu.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://fl.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fa.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sc.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yh.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xe.huixiangedu.cn

================================================================================
来源：http://bb.haigaiapp.cn

N. 数据结构与算法
来源：http://vp.nicolike.cn

================================================================================
来源：http://dl.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://ps.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hk.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://br.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mo.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fl.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dk.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://wx.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ct.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kc.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://zn.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://th.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fo.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ux.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tr.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ny.szsharing.cn

Go:   slices.Sort(arr)
来源：http://oq.jianghongdianzi.cn

Ruby: arr.sort
来源：http://px.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wb.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://id.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wu.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://hl.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rd.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fq.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yf.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oc.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zn.colortex.cn

[N04] 斐波那契数列
来源：http://ie.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qv.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zt.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ed.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qy.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eu.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bm.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ft.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ov.szxytkj.cn

[N05] 最大公约数
来源：http://qc.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://kp.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ik.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oc.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nz.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ew.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qc.nszjky.cn

Ruby: a.gcd(b)
来源：http://hm.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jv.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://nr.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://cu.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://dv.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://mn.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://is.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lw.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://pu.colortex.cn

Ruby: s == s.reverse
来源：http://wr.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qn.colortex.cn

[N07] 两数之和（返回下标）
来源：http://sy.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sr.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gj.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cc.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://kp.jctech888.com.cn

Java: // 手写 HashMap
来源：http://gx.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://mu.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://oy.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hl.yuntaijiaju.cn

[N08] 生成全排列
来源：http://hl.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://yy.szxytkj.cn

PHP:  // 手写递归交换
来源：http://cg.shxzukj.cn

JS:   // 手写回溯递归
来源：http://gn.huanxung.cn

TS:   // 手写回溯递归
来源：http://mt.shtwfgs.cn

Java: // 手写回溯递归
来源：http://sf.szsharing.cn

Go:   // 手写回溯递归
来源：http://bs.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://rt.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://mu.hahajie.cn

[N09] 栈与队列
来源：http://sk.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hh.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ms.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ls.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://us.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lu.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yf.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gb.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tg.jctech888.com.cn

[N10] 链表节点定义
来源：http://pi.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jg.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ay.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gi.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gn.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://wf.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cz.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qj.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jc.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://wx.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://as.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://fz.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://od.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cx.huixinmuqiang.cn

Java: // 手写递归
来源：http://mk.shxzukj.cn

Go:   // 手写递归
来源：http://qo.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jp.szsharing.cn

C#:   // 手写递归
来源：http://xh.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hk.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ws.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ky.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ov.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fo.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dy.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://li.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xq.shtwfgs.cn

================================================================================
来源：http://tc.shtwfgs.cn

O. 并发与异步
来源：http://dk.colortex.cn

================================================================================
来源：http://pm.muxihuayi.cn

[O01] 启动一个线程
来源：http://za.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://og.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fn.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sp.nszjky.cn

TS:   // 同 JS
来源：http://cb.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://bb.szxytkj.cn

Go:   go f()
来源：http://vt.lnxyls.cn

Ruby: Thread.new { f }
来源：http://xb.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://fp.521024.cn

[O02] 使用线程池
来源：http://ja.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nx.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wq.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://ey.521024.cn

TS:   // worker_threads 线程池
来源：http://qm.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nm.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oy.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fp.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kr.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ix.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://dr.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://ms.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fg.bjjhwx.cn

TS:   // 同 JS
来源：http://rc.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://xk.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lq.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ef.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://gs.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://bg.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://iw.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ig.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://io.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wh.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dk.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://au.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://go.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://fp.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://ou.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://xt.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ow.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://rw.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://fq.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mq.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tg.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://zl.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ao.muxihuayi.cn

[O06] 使用进程池
来源：http://ex.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bt.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://am.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://xt.asd995.cn

TS:   // child_process / cluster 模块
来源：http://yg.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wd.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://al.hnjuh.cn

Ruby: // fork 块
来源：http://ra.hnjuh.cn

C#:   Parallel.For
来源：http://my.huanxung.cn

================================================================================
来源：http://wt.nszjky.cn

P. 常用工具函数
来源：http://vm.bookmarksfly.cn

================================================================================
来源：http://tc.gzmigu.cn

[P01] 生成 UUID
来源：http://nl.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://qg.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yc.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://vt.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://ku.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://xb.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://aj.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://hq.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://zh.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://gv.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ux.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vc.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cj.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cq.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qu.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eq.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://at.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tw.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://ja.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jq.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gh.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vm.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nh.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eh.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wm.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uh.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bb.nicolike.cn

[P04] 求长度
来源：http://pz.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ql.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rx.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dt.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ew.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ub.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://rm.nszjky.cn

Ruby: x.length;  x.size
来源：http://hm.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ew.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ta.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nz.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bk.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kx.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ww.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ef.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mx.yuexingan06.cn

Ruby: a == b
来源：http://yu.yuntaijiaju.cn


<!-- 参考信息 -->