代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cu.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wx.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tx.colortex.cn

[L06] 解析响应为 JSON
来源：http://mq.newstarts.cn

Py:   resp.json()
来源：http://tu.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://hg.shtwfgs.cn

JS:   await resp.json()
来源：http://wr.hnjuh.cn

TS:   await resp.json()
来源：http://vh.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bg.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wt.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://iv.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fz.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://ia.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://td.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bh.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://vj.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ei.muxihuayi.cn

Java: resp.statusCode()
来源：http://fp.shtwfgs.cn

Go:   resp.StatusCode
来源：http://dk.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://xh.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://uc.nicolike.cn

[L08] 并发请求多个地址
来源：http://rh.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://so.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://as.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ur.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://en.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qk.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jk.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://al.shtwfgs.cn

================================================================================
来源：http://jn.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://nz.shxzskj.cn

================================================================================
来源：http://uh.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ap.shxzukj.cn

Py:   sys.argv[1:]
来源：http://mk.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://kd.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://dv.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://dk.asd995.cn

Java: args 数组（main 方法参数）
来源：http://ou.colortex.cn

Go:   os.Args[1:]
来源：http://ic.panjiajie.cn

Ruby: ARGV
来源：http://jl.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://xn.shtwfgs.cn

[M02] 读取环境变量
来源：http://op.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://qz.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xs.lnxyls.cn

JS:   process.env.HOME
来源：http://on.szxytkj.cn

TS:   process.env.HOME
来源：http://yf.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ud.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ue.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://it.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hi.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://dv.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vu.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dx.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mi.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qk.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ts.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yb.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://ax.newstarts.cn

[M04] 获取当前工作目录
来源：http://jj.hnjuh.cn

Py:   os.getcwd()
来源：http://mt.9csxet.cn

PHP:  getcwd();
来源：http://qy.colortex.cn

JS:   process.cwd()
来源：http://dt.hnjuh.cn

TS:   process.cwd()
来源：http://hd.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://kl.gzmigu.cn

Go:   os.Getwd()
来源：http://pb.asd995.cn

Ruby: Dir.pwd
来源：http://rq.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zi.gzmigu.cn

[M05] 设置退出码
来源：http://rf.panjiajie.cn

Py:   sys.exit(1)
来源：http://ga.jianghongdianzi.cn

PHP:  exit(1);
来源：http://wb.chemitech.net.cn

JS:   process.exit(1)
来源：http://di.shxzukj.cn

TS:   process.exit(1)
来源：http://fb.asd995.cn

Java: System.exit(1)
来源：http://hq.wgjwhj.cn

Go:   os.Exit(1)
来源：http://bj.colortex.cn

Ruby: exit 1
来源：http://tf.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pb.nszjky.cn

[M06] 向标准错误输出
来源：http://bf.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://il.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mz.szsharing.cn

JS:   console.error("err")
来源：http://rt.hahajie.cn

TS:   console.error("err")
来源：http://xb.szxytkj.cn

Java: System.err.println("err")
来源：http://ax.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kx.chemitech.net.cn

Ruby: warn "err"
来源：http://qz.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://zt.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://nv.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ox.szsharing.cn

JS:   require.main === module
来源：http://gv.shtwfgs.cn

TS:   require.main === module
来源：http://tk.521024.cn

Java: public static void main(String[] args)
来源：http://qz.newstarts.cn

Go:   func main()
来源：http://kj.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hh.hahajie.cn

C#:   static void Main(string[] args)
来源：http://pl.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://vl.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://bk.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://xu.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://fx.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://al.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ed.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vl.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sx.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nf.nszjky.cn

================================================================================
来源：http://jy.szsharing.cn

N. 数据结构与算法
来源：http://bu.szxytkj.cn

================================================================================
来源：http://hx.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://te.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://od.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cg.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://is.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hi.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qo.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://pu.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bw.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lu.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ub.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qw.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kd.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://te.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uy.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dg.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://xb.huixiangedu.cn

Ruby: arr.sort
来源：http://ci.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rj.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://bt.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mi.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://hi.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pb.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wm.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jm.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yb.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ty.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wt.chemitech.net.cn

[N04] 斐波那契数列
来源：http://mu.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yv.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bk.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sq.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qe.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sl.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pz.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fa.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yf.huixiangedu.cn

[N05] 最大公约数
来源：http://ys.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://fp.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ib.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jb.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ww.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fe.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ie.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://iw.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://or.hnjuh.cn

[N06] 判断回文字符串
来源：http://hn.nszjky.cn

Py:   s == s[::-1]
来源：http://pi.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://mr.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://hb.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://dx.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iv.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://ax.panjiajie.cn

Ruby: s == s.reverse
来源：http://bq.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ul.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://ey.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tw.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ue.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qi.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://fc.nicolike.cn

Java: // 手写 HashMap
来源：http://lx.szsharing.cn

Go:   // 手写 map[int]int
来源：http://fq.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://ym.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yv.nszjky.cn

[N08] 生成全排列
来源：http://qk.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://st.colortex.cn

PHP:  // 手写递归交换
来源：http://km.huanxung.cn

JS:   // 手写回溯递归
来源：http://lh.lnxyls.cn

TS:   // 手写回溯递归
来源：http://fh.colortex.cn

Java: // 手写回溯递归
来源：http://aj.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://mu.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ib.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ml.521024.cn

[N09] 栈与队列
来源：http://kn.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mv.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qd.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wp.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rs.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sr.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vp.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://em.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rt.521024.cn

[N10] 链表节点定义
来源：http://fp.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sd.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mu.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ee.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ia.colortex.cn

Java: class Node { int v; Node next; }
来源：http://re.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tq.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vi.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ep.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://hf.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vy.colortex.cn

PHP:  // 手写递归函数
来源：http://iw.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://po.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://er.shxzukj.cn

Java: // 手写递归
来源：http://gh.bookmarksfly.cn

Go:   // 手写递归
来源：http://pf.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://of.9csxet.cn

C#:   // 手写递归
来源：http://jb.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wn.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ub.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dh.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xy.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ti.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ei.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://it.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dm.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://di.asd995.cn

================================================================================
来源：http://xn.huixiangedu.cn

O. 并发与异步
来源：http://wl.wgjwhj.cn

================================================================================
来源：http://rm.asd995.cn

[O01] 启动一个线程
来源：http://te.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://za.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kk.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wf.colortex.cn

TS:   // 同 JS
来源：http://ee.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://lh.panjiajie.cn

Go:   go f()
来源：http://fz.shxzskj.cn

Ruby: Thread.new { f }
来源：http://dd.szsharing.cn

C#:   Task.Run(() => F());
来源：http://td.panjiajie.cn

[O02] 使用线程池
来源：http://xx.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bu.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ew.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://we.nszjky.cn

TS:   // worker_threads 线程池
来源：http://fd.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mp.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://at.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hi.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://to.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://qg.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://ln.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ay.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ro.bjjhwx.cn

TS:   // 同 JS
来源：http://oz.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://rd.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qf.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tm.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://cd.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ms.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://og.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gc.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://ak.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://np.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kt.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vb.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mr.colortex.cn

C#:   async Task F() { await G(); }
来源：http://ia.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://vs.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://qu.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sn.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://tl.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://gf.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dd.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yd.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://zc.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jq.jianghongdianzi.cn

[O06] 使用进程池
来源：http://ns.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://co.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tk.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://at.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://lv.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sm.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bs.colortex.cn

Ruby: // fork 块
来源：http://sm.9csxet.cn

C#:   Parallel.For
来源：http://vr.szsharing.cn

================================================================================
来源：http://oe.szsharing.cn

P. 常用工具函数
来源：http://wj.szxytkj.cn

================================================================================
来源：http://pf.szsharing.cn

[P01] 生成 UUID
来源：http://vs.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://hp.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sk.9csxet.cn

JS:   crypto.randomUUID()
来源：http://iu.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://ed.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://oy.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://nh.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://vc.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ul.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://jk.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ri.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rs.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://us.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ia.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qz.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fd.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ts.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kk.521024.cn

[P03] 生成短随机字符串
来源：http://ep.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xy.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rf.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://as.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://as.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xx.shxzskj.cn


<!-- 参考信息 -->