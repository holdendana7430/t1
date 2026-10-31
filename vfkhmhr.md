代发 wailian999

Py:   resp.json()
来源：http://ud.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://li.shtwfgs.cn

JS:   await resp.json()
来源：http://us.jianghongdianzi.cn

TS:   await resp.json()
来源：http://yl.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zy.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ba.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://st.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lz.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ik.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jz.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ip.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://sv.asd995.cn

TS:   resp.ok;  resp.status
来源：http://vy.bookmarksfly.cn

Java: resp.statusCode()
来源：http://pv.panjiajie.cn

Go:   resp.StatusCode
来源：http://is.colortex.cn

Ruby: resp.code.to_i
来源：http://xc.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://yi.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://sw.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vg.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://sq.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dg.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nu.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://et.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tt.szxytkj.cn

================================================================================
来源：http://di.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ti.bookmarksfly.cn

================================================================================
来源：http://wb.newstarts.cn

[M01] 读取命令行参数
来源：http://xp.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://lc.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://iv.9csxet.cn

JS:   process.argv.slice(2)
来源：http://vy.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://yg.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://pl.yuexingan06.cn

Go:   os.Args[1:]
来源：http://cm.bookmarksfly.cn

Ruby: ARGV
来源：http://te.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://hc.panjiajie.cn

[M02] 读取环境变量
来源：http://em.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://hd.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kc.huanxung.cn

JS:   process.env.HOME
来源：http://ac.newstarts.cn

TS:   process.env.HOME
来源：http://zd.shxzskj.cn

Java: System.getenv("HOME")
来源：http://wx.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sk.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://fs.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nh.szsharing.cn

[M03] 执行外部命令
来源：http://gi.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fi.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cy.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qu.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mv.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wq.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wx.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ve.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://yf.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://oy.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://tb.muxihuayi.cn

PHP:  getcwd();
来源：http://fw.panjiajie.cn

JS:   process.cwd()
来源：http://dr.gzmigu.cn

TS:   process.cwd()
来源：http://oe.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://eh.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ur.haigaiapp.cn

Ruby: Dir.pwd
来源：http://hk.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sa.gzmigu.cn

[M05] 设置退出码
来源：http://ra.9csxet.cn

Py:   sys.exit(1)
来源：http://hc.shxzukj.cn

PHP:  exit(1);
来源：http://qt.muxihuayi.cn

JS:   process.exit(1)
来源：http://um.nszjky.cn

TS:   process.exit(1)
来源：http://gc.chemitech.net.cn

Java: System.exit(1)
来源：http://rp.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ok.chemitech.net.cn

Ruby: exit 1
来源：http://yp.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lr.huanxung.cn

[M06] 向标准错误输出
来源：http://yx.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://sb.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bo.asd995.cn

JS:   console.error("err")
来源：http://uz.huanxung.cn

TS:   console.error("err")
来源：http://vc.muxihuayi.cn

Java: System.err.println("err")
来源：http://fb.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sc.newstarts.cn

Ruby: warn "err"
来源：http://vf.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://gy.colortex.cn

[M07] 判断是否为主入口
来源：http://gy.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://yz.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wj.shxzukj.cn

JS:   require.main === module
来源：http://zm.9csxet.cn

TS:   require.main === module
来源：http://yw.shxzukj.cn

Java: public static void main(String[] args)
来源：http://uw.gzmigu.cn

Go:   func main()
来源：http://sj.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sb.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://tw.asd995.cn

[M08] 获取系统与运行时信息
来源：http://dd.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://pf.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://co.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://at.panjiajie.cn

TS:   process.platform;  process.version
来源：http://wi.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wn.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://od.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://si.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ah.shxzskj.cn

================================================================================
来源：http://vl.hnjuh.cn

N. 数据结构与算法
来源：http://tr.huixiangedu.cn

================================================================================
来源：http://al.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://na.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qa.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://td.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://to.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pd.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wz.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://vl.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://it.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sk.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://cx.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://za.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fj.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ab.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://es.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vw.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://jr.haigaiapp.cn

Ruby: arr.sort
来源：http://yd.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://py.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://sb.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lp.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://rw.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ry.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mo.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jw.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nl.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lw.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yp.lnxyls.cn

[N04] 斐波那契数列
来源：http://ng.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://th.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rv.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ve.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tx.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vr.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fx.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ol.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ag.haigaiapp.cn

[N05] 最大公约数
来源：http://ma.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://wa.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rv.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vw.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qq.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xv.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://st.szsharing.cn

Ruby: a.gcd(b)
来源：http://go.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vs.wgjwhj.cn

[N06] 判断回文字符串
来源：http://ej.shxzskj.cn

Py:   s == s[::-1]
来源：http://op.newstarts.cn

PHP:  $s === strrev($s);
来源：http://hc.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://nl.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://hx.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rw.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://ru.gzmigu.cn

Ruby: s == s.reverse
来源：http://yk.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sg.asd995.cn

[N07] 两数之和（返回下标）
来源：http://od.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bk.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://em.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ca.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://qz.szxytkj.cn

Java: // 手写 HashMap
来源：http://gq.newstarts.cn

Go:   // 手写 map[int]int
来源：http://zn.shxzukj.cn

Ruby: // 手写 Hash
来源：http://te.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ii.chemitech.net.cn

[N08] 生成全排列
来源：http://jp.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://mw.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://zf.nszjky.cn

JS:   // 手写回溯递归
来源：http://eo.9csxet.cn

TS:   // 手写回溯递归
来源：http://mv.chemitech.net.cn

Java: // 手写回溯递归
来源：http://wp.9csxet.cn

Go:   // 手写回溯递归
来源：http://jp.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://xs.hahajie.cn

C#:   // 手写回溯递归
来源：http://re.lnxyls.cn

[N09] 栈与队列
来源：http://am.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://au.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zi.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nq.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vb.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ka.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ku.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cz.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nc.shxzukj.cn

[N10] 链表节点定义
来源：http://kz.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://po.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ch.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xa.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mb.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://oq.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wy.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hb.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yy.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://lo.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cj.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ab.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ov.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lz.haigaiapp.cn

Java: // 手写递归
来源：http://yn.huanxung.cn

Go:   // 手写递归
来源：http://sy.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://co.hahajie.cn

C#:   // 手写递归
来源：http://ge.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nj.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ja.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vu.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fn.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lv.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://am.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xw.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ke.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zm.gzmigu.cn

================================================================================
来源：http://ra.hnjuh.cn

O. 并发与异步
来源：http://sm.jctech888.com.cn

================================================================================
来源：http://mt.nszjky.cn

[O01] 启动一个线程
来源：http://zb.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bg.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dc.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wt.nszjky.cn

TS:   // 同 JS
来源：http://rv.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://uu.521024.cn

Go:   go f()
来源：http://gi.hahajie.cn

Ruby: Thread.new { f }
来源：http://hm.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://fx.shtwfgs.cn

[O02] 使用线程池
来源：http://da.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sw.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rp.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://ad.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://hd.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iw.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wg.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eu.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fc.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://on.huanxung.cn

Py:   with lock: shared += 1
来源：http://qr.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://uf.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ww.szxytkj.cn

TS:   // 同 JS
来源：http://ks.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://hb.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jw.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fk.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://vu.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://oo.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://qy.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mn.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://ai.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kz.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kd.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lj.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fm.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://tv.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://sa.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://de.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cv.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://lh.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://lx.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zl.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cf.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://lr.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rl.shxzukj.cn

[O06] 使用进程池
来源：http://pp.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://at.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ja.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://mw.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://fl.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bl.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zk.hnjuh.cn

Ruby: // fork 块
来源：http://ky.huixinmuqiang.cn

C#:   Parallel.For
来源：http://nj.szxytkj.cn

================================================================================
来源：http://jo.hahajie.cn

P. 常用工具函数
来源：http://tw.shtwfgs.cn

================================================================================
来源：http://pq.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://wb.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://eo.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cd.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://zi.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://kj.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://lc.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://bf.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://rb.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://pp.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://qo.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vp.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://th.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sn.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ch.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ky.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zu.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vv.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sv.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://wo.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pr.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yl.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dx.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mv.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tk.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ir.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kt.haigaiapp.cn

[P04] 求长度
来源：http://gr.bookmarksfly.cn


<!-- 参考信息 -->