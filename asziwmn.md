代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vc.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://al.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ie.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fi.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pn.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xi.521024.cn

[L05] 上传文件（multipart）
来源：http://zw.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hp.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sk.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://en.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uh.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sn.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pc.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fc.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iu.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://gx.huixiangedu.cn

Py:   resp.json()
来源：http://gb.521024.cn

PHP:  json_decode($body, true);
来源：http://kt.521024.cn

JS:   await resp.json()
来源：http://ey.szsharing.cn

TS:   await resp.json()
来源：http://mf.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mi.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bp.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://sc.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://po.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://qa.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://li.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tm.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://si.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://ud.lnxyls.cn

Java: resp.statusCode()
来源：http://zo.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://bv.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://un.521024.cn

C#:   (int)resp.StatusCode
来源：http://qh.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://kk.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eg.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://om.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mv.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sb.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://za.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ep.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://go.huixinmuqiang.cn

================================================================================
来源：http://wm.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://ee.huixinmuqiang.cn

================================================================================
来源：http://we.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://fn.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://gt.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://zh.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://vf.asd995.cn

TS:   process.argv.slice(2)
来源：http://zz.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://jg.gzmigu.cn

Go:   os.Args[1:]
来源：http://kw.muxihuayi.cn

Ruby: ARGV
来源：http://zu.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://wk.shxzskj.cn

[M02] 读取环境变量
来源：http://vk.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://nd.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gz.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://zk.shtwfgs.cn

TS:   process.env.HOME
来源：http://dz.lnxyls.cn

Java: System.getenv("HOME")
来源：http://qh.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nj.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://uj.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rm.shxzskj.cn

[M03] 执行外部命令
来源：http://fr.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yy.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ej.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ae.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nq.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bp.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pi.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wo.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://mj.lnxyls.cn

[M04] 获取当前工作目录
来源：http://pz.shxzskj.cn

Py:   os.getcwd()
来源：http://fy.gzmigu.cn

PHP:  getcwd();
来源：http://fd.szsharing.cn

JS:   process.cwd()
来源：http://lz.yuexingan06.cn

TS:   process.cwd()
来源：http://ue.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://xk.haigaiapp.cn

Go:   os.Getwd()
来源：http://in.shxzukj.cn

Ruby: Dir.pwd
来源：http://gd.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kn.lnxyls.cn

[M05] 设置退出码
来源：http://mp.shxzskj.cn

Py:   sys.exit(1)
来源：http://tw.nicolike.cn

PHP:  exit(1);
来源：http://vi.bookmarksfly.cn

JS:   process.exit(1)
来源：http://sf.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://tw.huanxung.cn

Java: System.exit(1)
来源：http://xw.hnjuh.cn

Go:   os.Exit(1)
来源：http://hp.shxzskj.cn

Ruby: exit 1
来源：http://lz.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gl.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://oe.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://gh.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gj.panjiajie.cn

JS:   console.error("err")
来源：http://ms.haigaiapp.cn

TS:   console.error("err")
来源：http://cn.jctech888.com.cn

Java: System.err.println("err")
来源：http://ra.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vq.nszjky.cn

Ruby: warn "err"
来源：http://nn.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://eq.panjiajie.cn

[M07] 判断是否为主入口
来源：http://ci.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://zr.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://us.lnxyls.cn

JS:   require.main === module
来源：http://ip.hahajie.cn

TS:   require.main === module
来源：http://cd.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://nm.yuexingan06.cn

Go:   func main()
来源：http://xk.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://as.521024.cn

C#:   static void Main(string[] args)
来源：http://vw.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://ch.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://py.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://no.nicolike.cn

JS:   process.platform;  process.version
来源：http://sr.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://bl.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jo.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xr.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fx.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jd.szxytkj.cn

================================================================================
来源：http://uh.panjiajie.cn

N. 数据结构与算法
来源：http://wa.jctech888.com.cn

================================================================================
来源：http://uf.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://lb.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nr.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yd.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rl.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vh.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wz.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://rl.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rt.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fm.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://na.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://kx.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://im.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zy.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://na.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xk.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://sy.haigaiapp.cn

Ruby: arr.sort
来源：http://eg.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://up.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://vj.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wr.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://dp.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gy.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bq.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qv.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nw.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ju.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bj.muxihuayi.cn

[N04] 斐波那契数列
来源：http://pc.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://da.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cy.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lu.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pf.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pd.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wv.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://in.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://db.nicolike.cn

[N05] 最大公约数
来源：http://px.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://gm.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rg.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ys.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cc.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cz.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xc.9csxet.cn

Ruby: a.gcd(b)
来源：http://de.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ds.colortex.cn

[N06] 判断回文字符串
来源：http://vw.szxytkj.cn

Py:   s == s[::-1]
来源：http://or.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://nd.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ja.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://yh.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ok.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://ng.szsharing.cn

Ruby: s == s.reverse
来源：http://id.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ji.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://yy.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wr.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ly.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ov.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://zq.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ri.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://bh.nicolike.cn

Ruby: // 手写 Hash
来源：http://et.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ff.shtwfgs.cn

[N08] 生成全排列
来源：http://ko.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://ie.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://aa.panjiajie.cn

JS:   // 手写回溯递归
来源：http://rn.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://fi.huixiangedu.cn

Java: // 手写回溯递归
来源：http://kh.gzmigu.cn

Go:   // 手写回溯递归
来源：http://qi.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://rv.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://vs.chemitech.net.cn

[N09] 栈与队列
来源：http://us.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xs.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ej.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://na.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pd.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yx.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dg.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kg.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rk.newstarts.cn

[N10] 链表节点定义
来源：http://fv.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sk.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kn.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ao.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tm.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://oj.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gg.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qe.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://im.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://gu.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ao.521024.cn

PHP:  // 手写递归函数
来源：http://av.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yd.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ty.bookmarksfly.cn

Java: // 手写递归
来源：http://me.szsharing.cn

Go:   // 手写递归
来源：http://vo.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ge.huixinmuqiang.cn

C#:   // 手写递归
来源：http://kv.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gz.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fq.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ef.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lu.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rr.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iv.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fl.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dh.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bh.asd995.cn

================================================================================
来源：http://ok.yuexingan06.cn

O. 并发与异步
来源：http://vm.muxihuayi.cn

================================================================================
来源：http://dz.yuexingan06.cn

[O01] 启动一个线程
来源：http://sl.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nd.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wo.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ky.nicolike.cn

TS:   // 同 JS
来源：http://wx.521024.cn

Java: new Thread(() -> f()).start()
来源：http://gk.9csxet.cn

Go:   go f()
来源：http://qk.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://hb.nszjky.cn

C#:   Task.Run(() => F());
来源：http://jm.nicolike.cn

[O02] 使用线程池
来源：http://yv.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fd.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xr.huanxung.cn

JS:   // worker_threads 线程池
来源：http://qn.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://fv.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bi.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jc.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wd.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qz.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://pd.hnjuh.cn

Py:   with lock: shared += 1
来源：http://ow.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://dm.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ia.asd995.cn

TS:   // 同 JS
来源：http://ua.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://hm.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tt.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://db.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://rt.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://dh.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://hn.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iz.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://gt.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xn.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iq.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qq.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zl.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ll.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://ba.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ek.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mm.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://hn.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://bj.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cd.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nc.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://jo.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eq.shxzukj.cn

[O06] 使用进程池
来源：http://uo.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nu.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qa.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://vb.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://wx.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://th.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eb.panjiajie.cn

Ruby: // fork 块
来源：http://wi.shtwfgs.cn

C#:   Parallel.For
来源：http://rn.shxzukj.cn

================================================================================
来源：http://ai.shxzukj.cn

P. 常用工具函数
来源：http://bj.hahajie.cn

================================================================================
来源：http://gr.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://mx.colortex.cn

Py:   str(uuid.uuid4())
来源：http://gz.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uh.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://if.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://ur.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://ap.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ww.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://ts.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://sq.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://nw.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vx.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oe.jianghongdianzi.cn


<!-- 参考信息 -->