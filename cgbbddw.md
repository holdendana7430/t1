代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lt.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hf.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://oj.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mh.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gn.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zb.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kp.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xz.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qe.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kj.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nk.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://mk.huanxung.cn

Py:   resp.json()
来源：http://lb.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://eb.bjjhwx.cn

JS:   await resp.json()
来源：http://fq.muxihuayi.cn

TS:   await resp.json()
来源：http://ot.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gb.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wt.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://mc.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ox.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://bb.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gb.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://th.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ih.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://fg.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://hw.newstarts.cn

Go:   resp.StatusCode
来源：http://ae.newstarts.cn

Ruby: resp.code.to_i
来源：http://zs.521024.cn

C#:   (int)resp.StatusCode
来源：http://hw.gzmigu.cn

[L08] 并发请求多个地址
来源：http://cs.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://we.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://gv.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ae.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sj.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://st.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ve.nszjky.cn

================================================================================
来源：http://tz.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://zx.521024.cn

================================================================================
来源：http://ml.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://fc.newstarts.cn

Py:   sys.argv[1:]
来源：http://ew.9csxet.cn

PHP:  $argv;  $argc;
来源：http://fv.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://or.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://cl.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://iv.9csxet.cn

Go:   os.Args[1:]
来源：http://rd.9csxet.cn

Ruby: ARGV
来源：http://jn.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://kt.newstarts.cn

[M02] 读取环境变量
来源：http://ng.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://iv.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gc.shxzskj.cn

JS:   process.env.HOME
来源：http://ib.huixiangedu.cn

TS:   process.env.HOME
来源：http://dt.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://fi.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pz.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://lx.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jy.nicolike.cn

[M03] 执行外部命令
来源：http://ei.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ss.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vu.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tz.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nh.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ax.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mh.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://du.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://qh.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://zq.haigaiapp.cn

Py:   os.getcwd()
来源：http://ee.szxytkj.cn

PHP:  getcwd();
来源：http://ku.newstarts.cn

JS:   process.cwd()
来源：http://ff.shxzukj.cn

TS:   process.cwd()
来源：http://mn.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ds.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://yx.shxzukj.cn

Ruby: Dir.pwd
来源：http://ul.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cu.9csxet.cn

[M05] 设置退出码
来源：http://zr.huixiangedu.cn

Py:   sys.exit(1)
来源：http://ev.yuntaijiaju.cn

PHP:  exit(1);
来源：http://zb.muxihuayi.cn

JS:   process.exit(1)
来源：http://dl.szsharing.cn

TS:   process.exit(1)
来源：http://ax.9csxet.cn

Java: System.exit(1)
来源：http://nb.muxihuayi.cn

Go:   os.Exit(1)
来源：http://oi.panjiajie.cn

Ruby: exit 1
来源：http://rn.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zt.nszjky.cn

[M06] 向标准错误输出
来源：http://dd.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://lx.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lg.huixinmuqiang.cn

JS:   console.error("err")
来源：http://ae.asd995.cn

TS:   console.error("err")
来源：http://td.nicolike.cn

Java: System.err.println("err")
来源：http://ep.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sh.yuexingan06.cn

Ruby: warn "err"
来源：http://fw.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://dh.nszjky.cn

[M07] 判断是否为主入口
来源：http://rp.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://hk.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yf.yuexingan06.cn

JS:   require.main === module
来源：http://ui.hnjuh.cn

TS:   require.main === module
来源：http://ib.nicolike.cn

Java: public static void main(String[] args)
来源：http://dd.newstarts.cn

Go:   func main()
来源：http://rx.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://et.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://fo.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://cf.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://xs.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://wd.huanxung.cn

JS:   process.platform;  process.version
来源：http://dp.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://da.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pz.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vi.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ch.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ow.nszjky.cn

================================================================================
来源：http://jr.shxzukj.cn

N. 数据结构与算法
来源：http://dk.chemitech.net.cn

================================================================================
来源：http://vp.asd995.cn

[N01] 二分查找（有序数组）
来源：http://go.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lf.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rs.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ug.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rg.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hv.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://wz.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wb.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pp.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://xx.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://vk.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zg.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nx.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zb.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kk.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://hi.shxzskj.cn

Ruby: arr.sort
来源：http://vi.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dh.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://ei.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yd.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ra.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tb.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://my.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fh.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://az.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ot.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rc.chemitech.net.cn

[N04] 斐波那契数列
来源：http://xy.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zv.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://al.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nb.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pl.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yo.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hy.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pc.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zo.szxytkj.cn

[N05] 最大公约数
来源：http://rv.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://ty.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hu.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hk.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rc.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ob.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ud.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://ut.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cy.huanxung.cn

[N06] 判断回文字符串
来源：http://ub.colortex.cn

Py:   s == s[::-1]
来源：http://zv.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://ug.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://dv.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://tz.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nx.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ct.colortex.cn

Ruby: s == s.reverse
来源：http://bh.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nk.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://oa.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zo.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xn.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hh.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ev.chemitech.net.cn

Java: // 手写 HashMap
来源：http://fu.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://is.hnjuh.cn

Ruby: // 手写 Hash
来源：http://am.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fj.bookmarksfly.cn

[N08] 生成全排列
来源：http://bw.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://um.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://bd.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://vn.shxzskj.cn

TS:   // 手写回溯递归
来源：http://tn.shxzukj.cn

Java: // 手写回溯递归
来源：http://dr.szxytkj.cn

Go:   // 手写回溯递归
来源：http://ja.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zp.lnxyls.cn

C#:   // 手写回溯递归
来源：http://ud.wgjwhj.cn

[N09] 栈与队列
来源：http://kg.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jn.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ni.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://am.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rh.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lo.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://is.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hy.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mk.9csxet.cn

[N10] 链表节点定义
来源：http://im.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pe.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://in.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fx.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ao.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://sb.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://na.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xp.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hx.nszjky.cn

[N11] 二叉树中序遍历
来源：http://wm.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dg.nszjky.cn

PHP:  // 手写递归函数
来源：http://ro.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wa.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ey.nicolike.cn

Java: // 手写递归
来源：http://ye.wgjwhj.cn

Go:   // 手写递归
来源：http://ju.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jv.newstarts.cn

C#:   // 手写递归
来源：http://um.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uq.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zx.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vy.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://za.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zl.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sl.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lb.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xk.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rm.jctech888.com.cn

================================================================================
来源：http://bs.shxzskj.cn

O. 并发与异步
来源：http://pr.muxihuayi.cn

================================================================================
来源：http://dn.shxzukj.cn

[O01] 启动一个线程
来源：http://xl.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tp.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fz.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fe.asd995.cn

TS:   // 同 JS
来源：http://sx.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://du.jianghongdianzi.cn

Go:   go f()
来源：http://qc.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://oo.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://zm.yuntaijiaju.cn

[O02] 使用线程池
来源：http://mu.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wm.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zs.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ha.nicolike.cn

TS:   // worker_threads 线程池
来源：http://mc.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://py.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fe.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xy.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://er.newstarts.cn

[O03] 加锁保护共享数据
来源：http://ml.panjiajie.cn

Py:   with lock: shared += 1
来源：http://qp.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://af.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pr.bjjhwx.cn

TS:   // 同 JS
来源：http://nf.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://qq.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://td.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yd.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ao.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://gn.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://zj.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wc.nicolike.cn

JS:   async function f() { await g(); }
来源：http://is.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hv.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ir.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ii.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nc.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://zv.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://mp.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://ty.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ql.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://vl.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://ut.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dc.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://km.nszjky.cn

Ruby: threads.map(&:join)
来源：http://jy.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wd.hnjuh.cn

[O06] 使用进程池
来源：http://qn.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zd.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lq.asd995.cn

JS:   // child_process / cluster 模块
来源：http://so.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://zw.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vn.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ot.bjjhwx.cn

Ruby: // fork 块
来源：http://tv.colortex.cn

C#:   Parallel.For
来源：http://fk.newstarts.cn

================================================================================
来源：http://np.asd995.cn

P. 常用工具函数
来源：http://jj.shxzukj.cn

================================================================================
来源：http://ar.bjjhwx.cn

[P01] 生成 UUID
来源：http://nd.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://wl.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fg.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://ps.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ca.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://zf.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://uq.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://hw.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://kk.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://rv.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ww.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qq.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pu.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tg.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zk.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mr.panjiajie.cn


<!-- 参考信息 -->