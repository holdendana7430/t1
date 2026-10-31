代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sw.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://va.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://tg.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lg.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://hf.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ax.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://od.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://vz.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://rr.shxzskj.cn

Java: resp.statusCode()
来源：http://fe.lnxyls.cn

Go:   resp.StatusCode
来源：http://yc.lnxyls.cn

Ruby: resp.code.to_i
来源：http://vq.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://ix.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://ye.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vd.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ff.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pu.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://si.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ym.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gn.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yq.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iv.panjiajie.cn

================================================================================
来源：http://if.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://bw.shtwfgs.cn

================================================================================
来源：http://ov.colortex.cn

[M01] 读取命令行参数
来源：http://zx.newstarts.cn

Py:   sys.argv[1:]
来源：http://ev.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://ry.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ac.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://lb.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://ud.muxihuayi.cn

Go:   os.Args[1:]
来源：http://pf.bjjhwx.cn

Ruby: ARGV
来源：http://da.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://kx.9csxet.cn

[M02] 读取环境变量
来源：http://lh.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://rq.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ab.shxzukj.cn

JS:   process.env.HOME
来源：http://if.shxzskj.cn

TS:   process.env.HOME
来源：http://et.panjiajie.cn

Java: System.getenv("HOME")
来源：http://pu.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xa.newstarts.cn

Ruby: ENV["HOME"]
来源：http://jv.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pk.panjiajie.cn

[M03] 执行外部命令
来源：http://sg.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rz.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xf.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wz.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rv.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tu.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wd.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oy.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://ev.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://bg.bookmarksfly.cn

Py:   os.getcwd()
来源：http://ys.huixiangedu.cn

PHP:  getcwd();
来源：http://sc.lnxyls.cn

JS:   process.cwd()
来源：http://yb.lnxyls.cn

TS:   process.cwd()
来源：http://va.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pt.panjiajie.cn

Go:   os.Getwd()
来源：http://iu.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://hk.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lt.szxytkj.cn

[M05] 设置退出码
来源：http://rv.huanxung.cn

Py:   sys.exit(1)
来源：http://me.bookmarksfly.cn

PHP:  exit(1);
来源：http://ns.wgjwhj.cn

JS:   process.exit(1)
来源：http://hk.gzmigu.cn

TS:   process.exit(1)
来源：http://xb.nicolike.cn

Java: System.exit(1)
来源：http://ix.yuexingan06.cn

Go:   os.Exit(1)
来源：http://du.yuntaijiaju.cn

Ruby: exit 1
来源：http://rj.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tv.colortex.cn

[M06] 向标准错误输出
来源：http://gv.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ca.nszjky.cn

JS:   console.error("err")
来源：http://xc.huixiangedu.cn

TS:   console.error("err")
来源：http://qc.gzmigu.cn

Java: System.err.println("err")
来源：http://hr.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ms.bjjhwx.cn

Ruby: warn "err"
来源：http://nc.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://vh.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://hv.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://qb.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ai.yuexingan06.cn

JS:   require.main === module
来源：http://kx.newstarts.cn

TS:   require.main === module
来源：http://lt.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://xa.newstarts.cn

Go:   func main()
来源：http://hv.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rq.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://ac.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://vy.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://tn.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://rh.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://wy.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://vx.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://he.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bt.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ei.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pa.hnjuh.cn

================================================================================
来源：http://bn.jctech888.com.cn

N. 数据结构与算法
来源：http://xr.jctech888.com.cn

================================================================================
来源：http://bt.colortex.cn

[N01] 二分查找（有序数组）
来源：http://zq.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uw.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pk.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vv.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ix.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gu.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://vc.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hy.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://in.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://bm.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bg.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ke.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://de.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zz.colortex.cn

Go:   slices.Sort(arr)
来源：http://zh.huixiangedu.cn

Ruby: arr.sort
来源：http://ya.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ch.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://gx.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gf.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://bg.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cq.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mn.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aw.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xk.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qt.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ug.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://da.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qf.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lc.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ff.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tb.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ve.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ex.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cb.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hp.gzmigu.cn

[N05] 最大公约数
来源：http://ks.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://os.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ku.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jt.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dk.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vn.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vg.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://qb.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ke.huixiangedu.cn

[N06] 判断回文字符串
来源：http://ju.huixiangedu.cn

Py:   s == s[::-1]
来源：http://xm.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://ak.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://qf.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://mu.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mg.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://pb.wgjwhj.cn

Ruby: s == s.reverse
来源：http://oo.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dj.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://qn.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rf.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tw.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xx.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://eu.newstarts.cn

Java: // 手写 HashMap
来源：http://wm.colortex.cn

Go:   // 手写 map[int]int
来源：http://qq.nszjky.cn

Ruby: // 手写 Hash
来源：http://dg.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hx.9csxet.cn

[N08] 生成全排列
来源：http://vf.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://qa.9csxet.cn

PHP:  // 手写递归交换
来源：http://dv.shxzskj.cn

JS:   // 手写回溯递归
来源：http://aa.9csxet.cn

TS:   // 手写回溯递归
来源：http://aa.asd995.cn

Java: // 手写回溯递归
来源：http://zc.asd995.cn

Go:   // 手写回溯递归
来源：http://eh.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://ft.szsharing.cn

C#:   // 手写回溯递归
来源：http://ku.shxzskj.cn

[N09] 栈与队列
来源：http://cn.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dt.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://om.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iq.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sv.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ld.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qh.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pl.huanxung.cn

[N10] 链表节点定义
来源：http://ot.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pa.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gl.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mi.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oc.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://qb.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://se.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ne.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yk.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ys.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tf.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://ij.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dz.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.bjjhwx.cn

Java: // 手写递归
来源：http://nl.szsharing.cn

Go:   // 手写递归
来源：http://da.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gh.szxytkj.cn

C#:   // 手写递归
来源：http://lu.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jo.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lk.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pr.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iv.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oy.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xo.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xt.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oa.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.chemitech.net.cn

================================================================================
来源：http://jo.shtwfgs.cn

O. 并发与异步
来源：http://or.huanxung.cn

================================================================================
来源：http://nm.shxzukj.cn

[O01] 启动一个线程
来源：http://nu.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ol.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://do.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ok.9csxet.cn

TS:   // 同 JS
来源：http://ot.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://dt.szxytkj.cn

Go:   go f()
来源：http://gk.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://lk.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://pp.shxzskj.cn

[O02] 使用线程池
来源：http://rj.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zf.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ip.huanxung.cn

JS:   // worker_threads 线程池
来源：http://tp.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://mj.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ko.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mt.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qb.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ec.newstarts.cn

[O03] 加锁保护共享数据
来源：http://nh.shxzukj.cn

Py:   with lock: shared += 1
来源：http://dn.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://wy.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ta.szxytkj.cn

TS:   // 同 JS
来源：http://iv.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://mf.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fg.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gh.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://re.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://pm.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://du.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zb.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://jx.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://av.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hw.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dq.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hx.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://ty.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://rg.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://fn.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cc.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://ub.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://rq.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jo.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eu.hahajie.cn

Ruby: threads.map(&:join)
来源：http://zx.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bo.szsharing.cn

[O06] 使用进程池
来源：http://yy.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uk.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xw.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://yw.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://my.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vj.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sa.shxzukj.cn

Ruby: // fork 块
来源：http://xn.panjiajie.cn

C#:   Parallel.For
来源：http://wc.panjiajie.cn

================================================================================
来源：http://cc.nicolike.cn

P. 常用工具函数
来源：http://ty.wgjwhj.cn

================================================================================
来源：http://vq.hnjuh.cn

[P01] 生成 UUID
来源：http://kg.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://ed.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sj.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://rb.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://zs.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://yd.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://fj.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://rv.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://sp.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://ln.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dy.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hq.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xi.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yh.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xv.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lb.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://av.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xy.gzmigu.cn

[P03] 生成短随机字符串
来源：http://yo.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aw.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rw.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tr.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ks.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ha.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jl.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yg.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uu.hnjuh.cn

[P04] 求长度
来源：http://yf.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pm.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ay.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kx.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ok.nicolike.cn


<!-- 参考信息 -->