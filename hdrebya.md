代发 wailian999

TS:   resp.ok;  resp.status
来源：http://qw.wgjwhj.cn

Java: resp.statusCode()
来源：http://yg.muxihuayi.cn

Go:   resp.StatusCode
来源：http://nx.nicolike.cn

Ruby: resp.code.to_i
来源：http://dw.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://lm.huanxung.cn

[L08] 并发请求多个地址
来源：http://mt.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fl.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://by.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://da.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sn.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yk.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sy.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ug.haigaiapp.cn

================================================================================
来源：http://pv.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://ur.shxzskj.cn

================================================================================
来源：http://wv.huanxung.cn

[M01] 读取命令行参数
来源：http://jo.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://lv.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://rm.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://eg.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://rw.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://gz.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ef.muxihuayi.cn

Ruby: ARGV
来源：http://ng.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://ml.huixiangedu.cn

[M02] 读取环境变量
来源：http://kb.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://md.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vh.panjiajie.cn

JS:   process.env.HOME
来源：http://tp.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://mq.nszjky.cn

Java: System.getenv("HOME")
来源：http://lr.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yk.huanxung.cn

Ruby: ENV["HOME"]
来源：http://mt.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ml.bookmarksfly.cn

[M03] 执行外部命令
来源：http://yq.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ve.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ly.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://og.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cl.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://et.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qn.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lw.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://vh.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://wv.shxzskj.cn

Py:   os.getcwd()
来源：http://ta.panjiajie.cn

PHP:  getcwd();
来源：http://cb.521024.cn

JS:   process.cwd()
来源：http://ll.jianghongdianzi.cn

TS:   process.cwd()
来源：http://ta.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://bg.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://bi.huanxung.cn

Ruby: Dir.pwd
来源：http://rg.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uu.9csxet.cn

[M05] 设置退出码
来源：http://kd.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://sq.hnjuh.cn

PHP:  exit(1);
来源：http://rl.gzmigu.cn

JS:   process.exit(1)
来源：http://wk.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ay.shtwfgs.cn

Java: System.exit(1)
来源：http://xw.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ur.shtwfgs.cn

Ruby: exit 1
来源：http://re.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vp.asd995.cn

[M06] 向标准错误输出
来源：http://ys.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://li.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ak.bookmarksfly.cn

JS:   console.error("err")
来源：http://dx.asd995.cn

TS:   console.error("err")
来源：http://hl.szsharing.cn

Java: System.err.println("err")
来源：http://sf.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uv.panjiajie.cn

Ruby: warn "err"
来源：http://ga.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://qv.shxzukj.cn

[M07] 判断是否为主入口
来源：http://ed.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://ex.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://et.bjjhwx.cn

JS:   require.main === module
来源：http://su.yuntaijiaju.cn

TS:   require.main === module
来源：http://jh.shxzskj.cn

Java: public static void main(String[] args)
来源：http://lw.huixiangedu.cn

Go:   func main()
来源：http://fu.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zw.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://mq.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://cl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://sd.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://sy.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://bo.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://rp.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qq.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ow.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eo.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://an.yuexingan06.cn

================================================================================
来源：http://mb.shtwfgs.cn

N. 数据结构与算法
来源：http://cr.bjjhwx.cn

================================================================================
来源：http://sb.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://hi.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iv.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tb.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eg.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ql.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://oo.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rg.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hl.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://sq.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://tx.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://va.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jz.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yr.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nu.szsharing.cn

Go:   slices.Sort(arr)
来源：http://wx.bjjhwx.cn

Ruby: arr.sort
来源：http://it.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://we.colortex.cn

[N03] 快速排序（分治示例）
来源：http://jf.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ds.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://yr.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pd.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nb.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ps.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ko.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lo.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://px.521024.cn

[N04] 斐波那契数列
来源：http://hk.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zu.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lf.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tt.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sw.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sk.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ap.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bh.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ip.szsharing.cn

[N05] 最大公约数
来源：http://cb.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ol.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qj.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nh.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ma.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ul.asd995.cn

Ruby: a.gcd(b)
来源：http://bi.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xd.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://xz.asd995.cn

Py:   s == s[::-1]
来源：http://dk.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://gr.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://gu.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://nb.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yo.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://ok.wgjwhj.cn

Ruby: s == s.reverse
来源：http://uz.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tf.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://py.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mb.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ql.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ox.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://yb.bjjhwx.cn

Java: // 手写 HashMap
来源：http://qf.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://eh.hahajie.cn

Ruby: // 手写 Hash
来源：http://di.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://to.yuexingan06.cn

[N08] 生成全排列
来源：http://ho.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://qe.lnxyls.cn

PHP:  // 手写递归交换
来源：http://sj.szxytkj.cn

JS:   // 手写回溯递归
来源：http://fn.colortex.cn

TS:   // 手写回溯递归
来源：http://ry.szsharing.cn

Java: // 手写回溯递归
来源：http://uu.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://ev.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ke.asd995.cn

C#:   // 手写回溯递归
来源：http://is.nszjky.cn

[N09] 栈与队列
来源：http://rz.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sg.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://us.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bt.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mb.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fz.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jw.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lc.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fp.colortex.cn

[N10] 链表节点定义
来源：http://sd.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uy.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ee.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qv.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fk.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://jk.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nz.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rf.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ph.colortex.cn

[N11] 二叉树中序遍历
来源：http://xb.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uw.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://md.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vg.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yp.hahajie.cn

Java: // 手写递归
来源：http://wi.szxytkj.cn

Go:   // 手写递归
来源：http://du.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pi.nszjky.cn

C#:   // 手写递归
来源：http://ap.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qi.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ra.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kc.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wm.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://op.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ko.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bj.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cy.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.newstarts.cn

================================================================================
来源：http://ix.jianghongdianzi.cn

O. 并发与异步
来源：http://ck.haigaiapp.cn

================================================================================
来源：http://ki.wgjwhj.cn

[O01] 启动一个线程
来源：http://es.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ki.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bp.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ul.hahajie.cn

TS:   // 同 JS
来源：http://je.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://qy.bjjhwx.cn

Go:   go f()
来源：http://vi.huanxung.cn

Ruby: Thread.new { f }
来源：http://vc.szsharing.cn

C#:   Task.Run(() => F());
来源：http://od.huanxung.cn

[O02] 使用线程池
来源：http://ay.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jf.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sl.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://xx.hahajie.cn

TS:   // worker_threads 线程池
来源：http://ei.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bp.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://df.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qs.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xz.521024.cn

[O03] 加锁保护共享数据
来源：http://ja.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://qn.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://pi.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nc.muxihuayi.cn

TS:   // 同 JS
来源：http://uq.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://zl.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sb.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rh.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://cn.szsharing.cn

[O04] 定义异步函数并等待
来源：http://ib.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://md.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zv.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://pc.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ho.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zx.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xp.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dq.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://va.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://le.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://sk.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ws.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://el.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://di.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ow.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ez.huanxung.cn

Ruby: threads.map(&:join)
来源：http://so.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ok.yuexingan06.cn

[O06] 使用进程池
来源：http://hm.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pe.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ik.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://fj.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://om.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mi.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://he.lnxyls.cn

Ruby: // fork 块
来源：http://vo.jianghongdianzi.cn

C#:   Parallel.For
来源：http://uv.asd995.cn

================================================================================
来源：http://hu.szxytkj.cn

P. 常用工具函数
来源：http://jq.nszjky.cn

================================================================================
来源：http://yd.newstarts.cn

[P01] 生成 UUID
来源：http://kj.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://zj.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qa.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://zk.huanxung.cn

TS:   crypto.randomUUID()
来源：http://tv.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://mn.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ho.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://oy.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://td.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://fi.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mc.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xt.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wg.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fp.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sw.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tf.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://he.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pa.hnjuh.cn

[P03] 生成短随机字符串
来源：http://dz.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sb.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ow.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fr.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gu.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dy.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zq.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gi.haigaiapp.cn

[P04] 求长度
来源：http://zt.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ro.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sc.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ar.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qg.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://gn.szsharing.cn

Go:   len(arr);  len(m)
来源：http://xm.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://nf.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tl.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://or.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ic.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wp.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sh.nicolike.cn


<!-- 参考信息 -->