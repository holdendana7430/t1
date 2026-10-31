代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fp.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gs.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uj.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ss.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yr.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://he.9csxet.cn

[L05] 上传文件（multipart）
来源：http://wp.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vk.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mu.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kf.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vj.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://by.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fg.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ba.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://jp.szsharing.cn

Py:   resp.json()
来源：http://be.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://pn.huanxung.cn

JS:   await resp.json()
来源：http://qd.huixiangedu.cn

TS:   await resp.json()
来源：http://gi.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xc.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ly.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://tz.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ak.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://fo.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ty.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vo.colortex.cn

JS:   resp.ok;  resp.status
来源：http://iy.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://cc.shxzskj.cn

Java: resp.statusCode()
来源：http://uc.shxzukj.cn

Go:   resp.StatusCode
来源：http://te.nszjky.cn

Ruby: resp.code.to_i
来源：http://yl.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://tz.9csxet.cn

[L08] 并发请求多个地址
来源：http://gw.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pk.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ej.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ph.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bm.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tw.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ss.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pw.szxytkj.cn

================================================================================
来源：http://ds.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://hd.hnjuh.cn

================================================================================
来源：http://gh.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://uo.nszjky.cn

Py:   sys.argv[1:]
来源：http://wq.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://zy.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://nb.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://zp.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ke.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ym.szsharing.cn

Ruby: ARGV
来源：http://ii.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://uy.shxzukj.cn

[M02] 读取环境变量
来源：http://ot.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://uz.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oi.9csxet.cn

JS:   process.env.HOME
来源：http://ix.lnxyls.cn

TS:   process.env.HOME
来源：http://ou.9csxet.cn

Java: System.getenv("HOME")
来源：http://ms.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mo.9csxet.cn

Ruby: ENV["HOME"]
来源：http://zg.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://en.yuexingan06.cn

[M03] 执行外部命令
来源：http://ax.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kk.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yf.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wd.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yk.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nj.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://si.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vk.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://kg.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://zw.szsharing.cn

Py:   os.getcwd()
来源：http://tr.huanxung.cn

PHP:  getcwd();
来源：http://zg.9csxet.cn

JS:   process.cwd()
来源：http://ss.colortex.cn

TS:   process.cwd()
来源：http://no.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://nu.chemitech.net.cn

Go:   os.Getwd()
来源：http://sa.gzmigu.cn

Ruby: Dir.pwd
来源：http://xo.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yp.shtwfgs.cn

[M05] 设置退出码
来源：http://mo.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ms.bjjhwx.cn

PHP:  exit(1);
来源：http://nr.gzmigu.cn

JS:   process.exit(1)
来源：http://jx.shxzskj.cn

TS:   process.exit(1)
来源：http://fe.521024.cn

Java: System.exit(1)
来源：http://zo.asd995.cn

Go:   os.Exit(1)
来源：http://mw.lnxyls.cn

Ruby: exit 1
来源：http://ef.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ce.lnxyls.cn

[M06] 向标准错误输出
来源：http://jc.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://gp.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ix.haigaiapp.cn

JS:   console.error("err")
来源：http://hu.hahajie.cn

TS:   console.error("err")
来源：http://xt.haigaiapp.cn

Java: System.err.println("err")
来源：http://oc.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yo.szsharing.cn

Ruby: warn "err"
来源：http://ct.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ef.gzmigu.cn

[M07] 判断是否为主入口
来源：http://do.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://lt.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ry.hahajie.cn

JS:   require.main === module
来源：http://pm.yuntaijiaju.cn

TS:   require.main === module
来源：http://gw.asd995.cn

Java: public static void main(String[] args)
来源：http://uk.9csxet.cn

Go:   func main()
来源：http://zm.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iv.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://mn.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://ac.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://uo.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://fo.gzmigu.cn

JS:   process.platform;  process.version
来源：http://er.huanxung.cn

TS:   process.platform;  process.version
来源：http://wj.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pe.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oz.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hp.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uw.nszjky.cn

================================================================================
来源：http://aq.shtwfgs.cn

N. 数据结构与算法
来源：http://yf.newstarts.cn

================================================================================
来源：http://ty.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://da.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vu.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://as.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lx.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vi.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dr.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://su.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ei.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dx.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://du.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://be.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ux.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wn.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tx.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://pn.haigaiapp.cn

Ruby: arr.sort
来源：http://yo.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fn.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://vo.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jm.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://sl.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ra.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sq.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ls.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dj.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yz.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uk.huixiangedu.cn

[N04] 斐波那契数列
来源：http://cq.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://em.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vp.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kv.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vy.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fx.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xe.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tr.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://on.9csxet.cn

[N05] 最大公约数
来源：http://mo.521024.cn

Py:   math.gcd(a, b)
来源：http://vh.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rd.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gr.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ue.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yt.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pj.hahajie.cn

Ruby: a.gcd(b)
来源：http://if.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sv.gzmigu.cn

[N06] 判断回文字符串
来源：http://iu.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://lx.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://gg.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://vv.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://xe.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nf.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://uw.lnxyls.cn

Ruby: s == s.reverse
来源：http://wo.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://st.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ro.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sa.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nl.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ct.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ta.shxzukj.cn

Java: // 手写 HashMap
来源：http://lk.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://ig.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://hk.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lu.muxihuayi.cn

[N08] 生成全排列
来源：http://hb.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ox.shxzukj.cn

PHP:  // 手写递归交换
来源：http://vb.panjiajie.cn

JS:   // 手写回溯递归
来源：http://ll.huanxung.cn

TS:   // 手写回溯递归
来源：http://if.haigaiapp.cn

Java: // 手写回溯递归
来源：http://du.nszjky.cn

Go:   // 手写回溯递归
来源：http://cd.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://ph.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://mo.wgjwhj.cn

[N09] 栈与队列
来源：http://hj.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lu.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lx.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pb.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wu.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ig.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://no.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hw.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ea.shxzukj.cn

[N10] 链表节点定义
来源：http://jt.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uo.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wk.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ei.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oi.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://yz.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oy.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xt.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ug.hahajie.cn

[N11] 二叉树中序遍历
来源：http://vg.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aa.nszjky.cn

PHP:  // 手写递归函数
来源：http://dv.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://im.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ky.shtwfgs.cn

Java: // 手写递归
来源：http://ew.huixiangedu.cn

Go:   // 手写递归
来源：http://td.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dp.gzmigu.cn

C#:   // 手写递归
来源：http://dp.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oy.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://en.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ci.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cb.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nb.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zs.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://io.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ng.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.lnxyls.cn

================================================================================
来源：http://ic.newstarts.cn

O. 并发与异步
来源：http://av.yuexingan06.cn

================================================================================
来源：http://wg.521024.cn

[O01] 启动一个线程
来源：http://fu.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tq.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xx.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tn.hnjuh.cn

TS:   // 同 JS
来源：http://gx.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://oh.jctech888.com.cn

Go:   go f()
来源：http://ya.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ae.asd995.cn

C#:   Task.Run(() => F());
来源：http://dz.gzmigu.cn

[O02] 使用线程池
来源：http://aa.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://in.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pz.colortex.cn

JS:   // worker_threads 线程池
来源：http://rp.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://vi.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tp.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qb.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cj.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://da.huanxung.cn

[O03] 加锁保护共享数据
来源：http://ci.521024.cn

Py:   with lock: shared += 1
来源：http://xk.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://qz.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pi.yuexingan06.cn

TS:   // 同 JS
来源：http://ct.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://xn.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mz.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cx.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://eo.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://ak.asd995.cn

Py:   async def f():⏎    await g()
来源：http://ld.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jn.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://ph.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fk.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hr.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fo.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hj.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://xc.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://bh.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://xo.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pm.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://fs.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://xg.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://us.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wc.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://es.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ev.hahajie.cn

[O06] 使用进程池
来源：http://fa.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bk.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oq.521024.cn

JS:   // child_process / cluster 模块
来源：http://ks.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://do.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iz.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zj.jctech888.com.cn

Ruby: // fork 块
来源：http://aw.bjjhwx.cn

C#:   Parallel.For
来源：http://gj.9csxet.cn

================================================================================
来源：http://sj.muxihuayi.cn

P. 常用工具函数
来源：http://ee.haigaiapp.cn

================================================================================
来源：http://lx.szxytkj.cn

[P01] 生成 UUID
来源：http://wk.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ml.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qr.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://oo.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://kh.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://rj.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://fp.asd995.cn

Ruby: SecureRandom.uuid
来源：http://sz.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://qi.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://sj.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dp.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fs.bookmarksfly.cn


<!-- 参考信息 -->