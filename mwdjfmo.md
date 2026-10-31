代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nj.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vl.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ha.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kh.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xs.bookmarksfly.cn

[L04] 设置超时
来源：http://zh.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://yd.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lp.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aw.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ey.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rd.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tr.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ge.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://yb.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ks.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mr.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://da.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ku.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oi.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hu.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://km.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://az.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://vw.huanxung.cn

Py:   resp.json()
来源：http://ei.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://cz.huixinmuqiang.cn

JS:   await resp.json()
来源：http://cx.huanxung.cn

TS:   await resp.json()
来源：http://ef.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cz.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://it.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://gn.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yv.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ch.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zh.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nq.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://wt.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://vn.shxzukj.cn

Java: resp.statusCode()
来源：http://hu.shtwfgs.cn

Go:   resp.StatusCode
来源：http://uh.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://wy.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://jd.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://nw.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cc.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://ma.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zl.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tm.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hw.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ib.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ax.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eh.huanxung.cn

================================================================================
来源：http://yn.521024.cn

M. 命令行 / 进程 / 环境
来源：http://zg.521024.cn

================================================================================
来源：http://ey.shtwfgs.cn

[M01] 读取命令行参数
来源：http://bc.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://rr.521024.cn

PHP:  $argv;  $argc;
来源：http://jk.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://xz.9csxet.cn

TS:   process.argv.slice(2)
来源：http://wq.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://ed.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://pj.bjjhwx.cn

Ruby: ARGV
来源：http://cd.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://vd.shxzskj.cn

[M02] 读取环境变量
来源：http://qb.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://hb.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qe.hnjuh.cn

JS:   process.env.HOME
来源：http://fp.huanxung.cn

TS:   process.env.HOME
来源：http://bw.9csxet.cn

Java: System.getenv("HOME")
来源：http://wj.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hs.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://hn.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mc.hnjuh.cn

[M03] 执行外部命令
来源：http://ke.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ap.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yf.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://us.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bm.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://la.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ky.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eg.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ci.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://go.nicolike.cn

Py:   os.getcwd()
来源：http://kb.panjiajie.cn

PHP:  getcwd();
来源：http://ol.newstarts.cn

JS:   process.cwd()
来源：http://xf.colortex.cn

TS:   process.cwd()
来源：http://zf.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://gl.muxihuayi.cn

Go:   os.Getwd()
来源：http://zw.shxzukj.cn

Ruby: Dir.pwd
来源：http://tt.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vc.colortex.cn

[M05] 设置退出码
来源：http://ax.hahajie.cn

Py:   sys.exit(1)
来源：http://oz.hnjuh.cn

PHP:  exit(1);
来源：http://rw.jctech888.com.cn

JS:   process.exit(1)
来源：http://yl.wgjwhj.cn

TS:   process.exit(1)
来源：http://cp.bjjhwx.cn

Java: System.exit(1)
来源：http://uw.hnjuh.cn

Go:   os.Exit(1)
来源：http://xl.9csxet.cn

Ruby: exit 1
来源：http://pd.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lt.chemitech.net.cn

[M06] 向标准错误输出
来源：http://gq.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://js.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ho.muxihuayi.cn

JS:   console.error("err")
来源：http://oy.nszjky.cn

TS:   console.error("err")
来源：http://ye.hahajie.cn

Java: System.err.println("err")
来源：http://jj.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://et.shxzukj.cn

Ruby: warn "err"
来源：http://mw.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://uf.huanxung.cn

[M07] 判断是否为主入口
来源：http://vl.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://ko.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://or.shtwfgs.cn

JS:   require.main === module
来源：http://an.bjjhwx.cn

TS:   require.main === module
来源：http://tp.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://xw.yuexingan06.cn

Go:   func main()
来源：http://gj.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ao.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://oq.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://yx.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://dw.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ss.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://gy.gzmigu.cn

TS:   process.platform;  process.version
来源：http://xn.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zv.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pt.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gw.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hg.jctech888.com.cn

================================================================================
来源：http://wf.hnjuh.cn

N. 数据结构与算法
来源：http://sg.panjiajie.cn

================================================================================
来源：http://wp.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://qu.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jy.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hg.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ki.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qk.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yf.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://pn.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://px.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jx.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://at.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zv.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rf.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aj.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eg.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://se.gzmigu.cn

Ruby: arr.sort
来源：http://sn.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yh.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://pw.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ep.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ig.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vz.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fw.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ka.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zo.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hd.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ok.szsharing.cn

[N04] 斐波那契数列
来源：http://hu.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://st.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mp.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jl.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gh.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zi.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gu.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jt.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ar.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ry.nszjky.cn

Py:   math.gcd(a, b)
来源：http://bw.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://in.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iw.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wx.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dv.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://tu.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ay.szsharing.cn

[N06] 判断回文字符串
来源：http://td.huanxung.cn

Py:   s == s[::-1]
来源：http://xw.nszjky.cn

PHP:  $s === strrev($s);
来源：http://hv.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://rh.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://ic.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ms.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://tl.nszjky.cn

Ruby: s == s.reverse
来源：http://sq.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zv.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://fc.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lt.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ca.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cu.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://ed.haigaiapp.cn

Java: // 手写 HashMap
来源：http://ks.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://hf.shxzukj.cn

Ruby: // 手写 Hash
来源：http://oz.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aj.nszjky.cn

[N08] 生成全排列
来源：http://xq.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://cg.gzmigu.cn

PHP:  // 手写递归交换
来源：http://wo.szsharing.cn

JS:   // 手写回溯递归
来源：http://gy.asd995.cn

TS:   // 手写回溯递归
来源：http://jg.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://nj.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ws.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ib.521024.cn

C#:   // 手写回溯递归
来源：http://pf.jianghongdianzi.cn

[N09] 栈与队列
来源：http://id.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zv.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ao.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ms.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rf.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jq.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gh.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://de.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ke.asd995.cn

[N10] 链表节点定义
来源：http://vb.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mm.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zk.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://va.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wi.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://zu.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gw.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ul.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rs.hahajie.cn

[N11] 二叉树中序遍历
来源：http://qa.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uh.521024.cn

PHP:  // 手写递归函数
来源：http://ex.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jw.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bw.jianghongdianzi.cn

Java: // 手写递归
来源：http://ez.asd995.cn

Go:   // 手写递归
来源：http://fj.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qs.lnxyls.cn

C#:   // 手写递归
来源：http://tn.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zx.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uw.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hn.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vs.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ul.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ih.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qh.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lr.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nk.shxzukj.cn

================================================================================
来源：http://by.nszjky.cn

O. 并发与异步
来源：http://hk.huanxung.cn

================================================================================
来源：http://hd.huixiangedu.cn

[O01] 启动一个线程
来源：http://gz.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wc.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rw.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://is.huixinmuqiang.cn

TS:   // 同 JS
来源：http://cl.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://ws.521024.cn

Go:   go f()
来源：http://sq.hahajie.cn

Ruby: Thread.new { f }
来源：http://qp.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://qp.colortex.cn

[O02] 使用线程池
来源：http://zj.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cr.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ru.asd995.cn

JS:   // worker_threads 线程池
来源：http://wi.colortex.cn

TS:   // worker_threads 线程池
来源：http://hf.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fc.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oy.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yi.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bl.colortex.cn

[O03] 加锁保护共享数据
来源：http://qn.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ii.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://mh.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pc.yuntaijiaju.cn

TS:   // 同 JS
来源：http://om.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://qy.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tr.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://td.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://xp.asd995.cn

[O04] 定义异步函数并等待
来源：http://hb.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://hs.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ci.newstarts.cn

JS:   async function f() { await g(); }
来源：http://mt.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://os.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tj.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oq.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pd.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://zk.521024.cn

[O05] 并发执行并等待全部完成
来源：http://ej.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://da.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cy.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://ti.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://xu.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xm.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zr.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://nj.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vy.panjiajie.cn

[O06] 使用进程池
来源：http://ao.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ie.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ll.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://gt.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://aq.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pe.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ak.chemitech.net.cn

Ruby: // fork 块
来源：http://ac.huixiangedu.cn

C#:   Parallel.For
来源：http://av.hahajie.cn

================================================================================
来源：http://gw.hnjuh.cn

P. 常用工具函数
来源：http://dy.shxzskj.cn

================================================================================
来源：http://lt.haigaiapp.cn

[P01] 生成 UUID
来源：http://ls.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://xn.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mv.szsharing.cn

JS:   crypto.randomUUID()
来源：http://fb.huanxung.cn


<!-- 参考信息 -->