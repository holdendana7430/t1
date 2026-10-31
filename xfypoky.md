代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tl.szsharing.cn

[L04] 设置超时
来源：http://ht.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ri.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cl.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lp.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hb.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zp.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tg.hahajie.cn

[L05] 上传文件（multipart）
来源：http://kf.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yd.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://he.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ll.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://az.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xx.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://al.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ae.asd995.cn

[L06] 解析响应为 JSON
来源：http://rv.huanxung.cn

Py:   resp.json()
来源：http://hs.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://hs.shxzukj.cn

JS:   await resp.json()
来源：http://jr.wgjwhj.cn

TS:   await resp.json()
来源：http://am.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xc.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dm.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://gc.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jy.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://cq.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ok.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kz.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ii.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://mg.jctech888.com.cn

Java: resp.statusCode()
来源：http://oh.haigaiapp.cn

Go:   resp.StatusCode
来源：http://yt.shxzskj.cn

Ruby: resp.code.to_i
来源：http://ss.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://fx.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://yd.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iu.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://dw.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zl.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aa.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nm.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://do.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gy.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zk.521024.cn

================================================================================
来源：http://oy.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://xj.hnjuh.cn

================================================================================
来源：http://yc.yuexingan06.cn

[M01] 读取命令行参数
来源：http://sw.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://po.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://zd.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://ii.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://uz.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://rf.huanxung.cn

Go:   os.Args[1:]
来源：http://wp.9csxet.cn

Ruby: ARGV
来源：http://ic.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://cq.hahajie.cn

[M02] 读取环境变量
来源：http://ym.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://kj.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mc.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://su.9csxet.cn

TS:   process.env.HOME
来源：http://ii.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://la.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hp.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ub.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pq.hahajie.cn

[M03] 执行外部命令
来源：http://ma.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pb.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nr.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fc.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fu.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pk.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dl.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hh.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://bv.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://gp.jctech888.com.cn

Py:   os.getcwd()
来源：http://xz.nszjky.cn

PHP:  getcwd();
来源：http://tb.chemitech.net.cn

JS:   process.cwd()
来源：http://ke.panjiajie.cn

TS:   process.cwd()
来源：http://nw.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://er.bjjhwx.cn

Go:   os.Getwd()
来源：http://wx.wgjwhj.cn

Ruby: Dir.pwd
来源：http://yh.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ra.muxihuayi.cn

[M05] 设置退出码
来源：http://qk.asd995.cn

Py:   sys.exit(1)
来源：http://ku.hahajie.cn

PHP:  exit(1);
来源：http://zy.huanxung.cn

JS:   process.exit(1)
来源：http://ba.muxihuayi.cn

TS:   process.exit(1)
来源：http://lv.huixiangedu.cn

Java: System.exit(1)
来源：http://az.bjjhwx.cn

Go:   os.Exit(1)
来源：http://mw.muxihuayi.cn

Ruby: exit 1
来源：http://zi.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yh.panjiajie.cn

[M06] 向标准错误输出
来源：http://xc.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://pi.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://va.haigaiapp.cn

JS:   console.error("err")
来源：http://ux.jctech888.com.cn

TS:   console.error("err")
来源：http://ad.hnjuh.cn

Java: System.err.println("err")
来源：http://ee.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ok.jctech888.com.cn

Ruby: warn "err"
来源：http://oq.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://jy.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://nm.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://jl.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ln.asd995.cn

JS:   require.main === module
来源：http://wv.nszjky.cn

TS:   require.main === module
来源：http://fd.nszjky.cn

Java: public static void main(String[] args)
来源：http://el.newstarts.cn

Go:   func main()
来源：http://bj.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lt.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://id.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://uw.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ep.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://ik.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://om.shxzukj.cn

TS:   process.platform;  process.version
来源：http://tc.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tw.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ws.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ae.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jr.lnxyls.cn

================================================================================
来源：http://tq.9csxet.cn

N. 数据结构与算法
来源：http://zo.huanxung.cn

================================================================================
来源：http://ep.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://hn.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nu.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lr.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zz.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lo.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nq.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ow.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://da.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bs.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://yr.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dn.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oi.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cm.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://qc.chemitech.net.cn

Ruby: arr.sort
来源：http://qw.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tk.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://at.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ku.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://ue.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aa.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hb.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jb.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lb.newstarts.cn

[N04] 斐波那契数列
来源：http://xc.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tg.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pm.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ni.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kt.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lw.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ty.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ul.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ev.bjjhwx.cn

[N05] 最大公约数
来源：http://et.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://lu.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bq.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oj.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dw.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tn.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://hk.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ae.huanxung.cn

[N06] 判断回文字符串
来源：http://ne.gzmigu.cn

Py:   s == s[::-1]
来源：http://pr.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ui.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://gc.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://us.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ii.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://cf.521024.cn

Ruby: s == s.reverse
来源：http://yf.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yz.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://xl.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pl.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lg.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://of.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://zh.9csxet.cn

Java: // 手写 HashMap
来源：http://ri.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://pq.hahajie.cn

Ruby: // 手写 Hash
来源：http://dj.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mu.chemitech.net.cn

[N08] 生成全排列
来源：http://bi.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://nx.panjiajie.cn

PHP:  // 手写递归交换
来源：http://pb.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://vk.9csxet.cn

TS:   // 手写回溯递归
来源：http://ww.newstarts.cn

Java: // 手写回溯递归
来源：http://fn.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://wm.521024.cn

Ruby: arr.permutation.to_a
来源：http://iw.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://lz.yuntaijiaju.cn

[N09] 栈与队列
来源：http://of.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wa.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cj.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uu.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ba.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ix.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kk.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vc.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fb.shxzskj.cn

[N10] 链表节点定义
来源：http://ak.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fa.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ke.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uj.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sq.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://if.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mv.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fh.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qg.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://li.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bd.asd995.cn

PHP:  // 手写递归函数
来源：http://ad.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tq.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nd.panjiajie.cn

Java: // 手写递归
来源：http://iy.haigaiapp.cn

Go:   // 手写递归
来源：http://ik.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://az.yuntaijiaju.cn

C#:   // 手写递归
来源：http://dj.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jx.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bn.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zu.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bj.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kw.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ll.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.szsharing.cn

================================================================================
来源：http://ro.huanxung.cn

O. 并发与异步
来源：http://ue.bookmarksfly.cn

================================================================================
来源：http://jy.9csxet.cn

[O01] 启动一个线程
来源：http://jh.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hk.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gw.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vi.jianghongdianzi.cn

TS:   // 同 JS
来源：http://gk.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://wq.9csxet.cn

Go:   go f()
来源：http://zf.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://gg.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ol.shtwfgs.cn

[O02] 使用线程池
来源：http://xn.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pz.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iv.newstarts.cn

JS:   // worker_threads 线程池
来源：http://mo.hahajie.cn

TS:   // worker_threads 线程池
来源：http://il.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wx.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ee.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bz.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qd.hahajie.cn

[O03] 加锁保护共享数据
来源：http://ay.huanxung.cn

Py:   with lock: shared += 1
来源：http://ld.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://em.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ft.shxzskj.cn

TS:   // 同 JS
来源：http://tg.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://bp.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hk.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tg.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://zw.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://kr.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://yw.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://th.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://gs.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ox.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oz.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fi.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ey.asd995.cn

C#:   async Task F() { await G(); }
来源：http://nb.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://jx.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://bw.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zc.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://xo.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://fd.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nw.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zi.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://de.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hf.huanxung.cn

[O06] 使用进程池
来源：http://uq.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dz.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://og.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://ik.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://wn.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ms.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hk.yuexingan06.cn

Ruby: // fork 块
来源：http://zq.lnxyls.cn

C#:   Parallel.For
来源：http://fo.yuexingan06.cn

================================================================================
来源：http://eg.huanxung.cn

P. 常用工具函数
来源：http://ij.yuexingan06.cn

================================================================================
来源：http://wi.huixiangedu.cn

[P01] 生成 UUID
来源：http://zg.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://sn.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dt.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://uy.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://lv.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://we.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://ah.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://dp.shtwfgs.cn


<!-- 参考信息 -->