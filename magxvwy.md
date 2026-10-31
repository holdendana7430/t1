代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kj.huanxung.cn

[L04] 设置超时
来源：http://qt.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://id.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gs.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://od.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://un.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bn.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fk.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nx.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://su.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://sm.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ae.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tg.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qm.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sj.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qj.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://go.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dj.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yf.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://au.huixiangedu.cn

Py:   resp.json()
来源：http://tk.nszjky.cn

PHP:  json_decode($body, true);
来源：http://bl.yuexingan06.cn

JS:   await resp.json()
来源：http://mj.szsharing.cn

TS:   await resp.json()
来源：http://ee.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xs.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zd.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://qu.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cr.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://oq.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yn.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pk.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://kq.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://kw.yuexingan06.cn

Java: resp.statusCode()
来源：http://lc.nicolike.cn

Go:   resp.StatusCode
来源：http://ur.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://kk.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://pq.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://oh.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://an.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://hl.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pp.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xt.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bf.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wp.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://em.521024.cn

================================================================================
来源：http://di.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://nw.yuexingan06.cn

================================================================================
来源：http://ty.jctech888.com.cn

[M01] 读取命令行参数
来源：http://kl.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://hp.521024.cn

PHP:  $argv;  $argc;
来源：http://tj.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://jw.hahajie.cn

TS:   process.argv.slice(2)
来源：http://cm.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://oo.nicolike.cn

Go:   os.Args[1:]
来源：http://wh.gzmigu.cn

Ruby: ARGV
来源：http://vg.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ly.nicolike.cn

[M02] 读取环境变量
来源：http://zl.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ez.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iz.wgjwhj.cn

JS:   process.env.HOME
来源：http://zq.nszjky.cn

TS:   process.env.HOME
来源：http://jg.shxzskj.cn

Java: System.getenv("HOME")
来源：http://aw.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lp.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ft.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qd.colortex.cn

[M03] 执行外部命令
来源：http://ex.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tw.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ib.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gi.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://co.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hl.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mi.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rl.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://xh.gzmigu.cn

[M04] 获取当前工作目录
来源：http://xs.bookmarksfly.cn

Py:   os.getcwd()
来源：http://rj.newstarts.cn

PHP:  getcwd();
来源：http://mm.huixiangedu.cn

JS:   process.cwd()
来源：http://su.gzmigu.cn

TS:   process.cwd()
来源：http://fc.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://bk.lnxyls.cn

Go:   os.Getwd()
来源：http://pn.nicolike.cn

Ruby: Dir.pwd
来源：http://wm.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eg.hahajie.cn

[M05] 设置退出码
来源：http://nf.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://bm.colortex.cn

PHP:  exit(1);
来源：http://hv.panjiajie.cn

JS:   process.exit(1)
来源：http://gt.szsharing.cn

TS:   process.exit(1)
来源：http://ce.nszjky.cn

Java: System.exit(1)
来源：http://td.hnjuh.cn

Go:   os.Exit(1)
来源：http://we.bookmarksfly.cn

Ruby: exit 1
来源：http://fw.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qh.shtwfgs.cn

[M06] 向标准错误输出
来源：http://nw.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://yr.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bn.nszjky.cn

JS:   console.error("err")
来源：http://ea.colortex.cn

TS:   console.error("err")
来源：http://ej.newstarts.cn

Java: System.err.println("err")
来源：http://zr.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yw.nicolike.cn

Ruby: warn "err"
来源：http://ew.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ji.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://lu.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://wd.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yl.shtwfgs.cn

JS:   require.main === module
来源：http://nd.haigaiapp.cn

TS:   require.main === module
来源：http://ws.nicolike.cn

Java: public static void main(String[] args)
来源：http://cn.colortex.cn

Go:   func main()
来源：http://qa.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oa.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://ki.521024.cn

[M08] 获取系统与运行时信息
来源：http://mv.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://wu.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://pm.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://iq.huanxung.cn

TS:   process.platform;  process.version
来源：http://jq.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fg.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ow.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eb.huixiangedu.cn

================================================================================
来源：http://hh.newstarts.cn

N. 数据结构与算法
来源：http://kk.yuexingan06.cn

================================================================================
来源：http://yq.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://sn.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mt.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://by.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vv.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ef.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jy.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ab.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aw.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kx.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://im.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://qo.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pt.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://os.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bu.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rf.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://mz.huixiangedu.cn

Ruby: arr.sort
来源：http://td.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ev.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://vh.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fk.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://hw.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yg.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hb.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sg.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wd.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qy.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sh.nszjky.cn

[N04] 斐波那契数列
来源：http://bw.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vh.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://js.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ux.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bc.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vv.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fp.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ve.szsharing.cn

[N05] 最大公约数
来源：http://xy.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://nn.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mq.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://un.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ui.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yb.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tp.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://zo.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qn.hahajie.cn

[N06] 判断回文字符串
来源：http://dh.asd995.cn

Py:   s == s[::-1]
来源：http://ai.521024.cn

PHP:  $s === strrev($s);
来源：http://rm.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://hi.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://fb.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yl.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://jp.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://zn.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ch.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ie.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ff.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://po.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wu.521024.cn

TS:   // 手写 Map<string, number>
来源：http://cr.huanxung.cn

Java: // 手写 HashMap
来源：http://co.huanxung.cn

Go:   // 手写 map[int]int
来源：http://rg.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://hm.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lc.521024.cn

[N08] 生成全排列
来源：http://by.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://gq.shxzskj.cn

PHP:  // 手写递归交换
来源：http://xv.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://kz.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://in.newstarts.cn

Java: // 手写回溯递归
来源：http://uy.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://eh.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://as.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://hs.huanxung.cn

[N09] 栈与队列
来源：http://ax.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aa.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sl.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://du.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bu.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kd.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wk.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aj.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iy.muxihuayi.cn

[N10] 链表节点定义
来源：http://on.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iy.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oy.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dj.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://tj.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gs.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kz.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ng.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://qt.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vf.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ow.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rj.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xo.yuntaijiaju.cn

Java: // 手写递归
来源：http://pd.panjiajie.cn

Go:   // 手写递归
来源：http://to.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bz.shxzukj.cn

C#:   // 手写递归
来源：http://xz.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dx.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://th.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pc.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ec.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lo.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ex.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sb.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vk.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gw.huixiangedu.cn

================================================================================
来源：http://qe.bjjhwx.cn

O. 并发与异步
来源：http://ac.newstarts.cn

================================================================================
来源：http://ky.shxzukj.cn

[O01] 启动一个线程
来源：http://ve.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lk.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dp.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xn.huixinmuqiang.cn

TS:   // 同 JS
来源：http://wt.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://cm.nicolike.cn

Go:   go f()
来源：http://se.colortex.cn

Ruby: Thread.new { f }
来源：http://pw.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://un.haigaiapp.cn

[O02] 使用线程池
来源：http://gu.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kp.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xo.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ir.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://xe.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wa.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oe.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wa.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://at.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://xz.colortex.cn

Py:   with lock: shared += 1
来源：http://yx.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://vq.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bu.shxzukj.cn

TS:   // 同 JS
来源：http://to.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://gq.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aq.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://np.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://mx.9csxet.cn

[O04] 定义异步函数并等待
来源：http://na.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://qi.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qm.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://sy.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hr.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jv.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ia.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wt.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://zh.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://kj.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://gj.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jo.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ds.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://pk.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fs.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yf.huanxung.cn

Ruby: threads.map(&:join)
来源：http://rz.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oo.muxihuayi.cn

[O06] 使用进程池
来源：http://nw.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://be.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jy.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://bx.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ai.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ds.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dh.huixinmuqiang.cn

Ruby: // fork 块
来源：http://mt.szxytkj.cn

C#:   Parallel.For
来源：http://li.bjjhwx.cn

================================================================================
来源：http://lo.szsharing.cn

P. 常用工具函数
来源：http://py.shxzskj.cn

================================================================================
来源：http://ys.jctech888.com.cn

[P01] 生成 UUID
来源：http://hk.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://rd.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dt.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://sk.521024.cn

TS:   crypto.randomUUID()
来源：http://st.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://iy.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://wh.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://wj.panjiajie.cn


<!-- 参考信息 -->