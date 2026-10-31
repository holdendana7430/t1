代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dm.hahajie.cn

JS:   await fetch(url)
来源：http://my.shxzukj.cn

TS:   await fetch(url)
来源：http://kq.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zy.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://fl.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uz.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rm.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ew.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eb.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cr.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ug.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lz.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qk.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nc.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ju.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vy.hnjuh.cn

[L03] 设置自定义请求头
来源：http://sy.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://im.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pn.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rq.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cp.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ei.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pd.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ol.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://or.wgjwhj.cn

[L04] 设置超时
来源：http://pt.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://oh.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rr.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gk.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vz.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yl.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cy.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bk.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tk.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://xg.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bq.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gr.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wh.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ru.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://es.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gc.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rt.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://pb.nicolike.cn

Py:   resp.json()
来源：http://jw.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://sq.szxytkj.cn

JS:   await resp.json()
来源：http://fs.bookmarksfly.cn

TS:   await resp.json()
来源：http://op.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pp.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bt.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://io.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fx.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ha.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jo.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://jw.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://cf.shtwfgs.cn

Java: resp.statusCode()
来源：http://mp.nszjky.cn

Go:   resp.StatusCode
来源：http://ze.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://ss.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://yw.shxzskj.cn

[L08] 并发请求多个地址
来源：http://rq.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ln.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://an.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hh.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vr.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rh.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bl.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dw.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eb.jianghongdianzi.cn

================================================================================
来源：http://mx.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://hc.hnjuh.cn

================================================================================
来源：http://zi.bjjhwx.cn

[M01] 读取命令行参数
来源：http://my.shxzukj.cn

Py:   sys.argv[1:]
来源：http://lh.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://pg.szsharing.cn

JS:   process.argv.slice(2)
来源：http://zg.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://pz.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://hj.jctech888.com.cn

Go:   os.Args[1:]
来源：http://tj.shxzskj.cn

Ruby: ARGV
来源：http://vh.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://xn.hahajie.cn

[M02] 读取环境变量
来源：http://kz.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://tg.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fm.hnjuh.cn

JS:   process.env.HOME
来源：http://en.muxihuayi.cn

TS:   process.env.HOME
来源：http://yy.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://yd.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ey.nicolike.cn

Ruby: ENV["HOME"]
来源：http://mw.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tk.jctech888.com.cn

[M03] 执行外部命令
来源：http://tt.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lt.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ey.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lg.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://no.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jr.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fa.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hq.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://vg.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://qx.colortex.cn

Py:   os.getcwd()
来源：http://ql.lnxyls.cn

PHP:  getcwd();
来源：http://ju.huixiangedu.cn

JS:   process.cwd()
来源：http://pa.yuntaijiaju.cn

TS:   process.cwd()
来源：http://gk.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://ff.chemitech.net.cn

Go:   os.Getwd()
来源：http://lz.szsharing.cn

Ruby: Dir.pwd
来源：http://wl.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uf.huixiangedu.cn

[M05] 设置退出码
来源：http://dd.gzmigu.cn

Py:   sys.exit(1)
来源：http://ln.jctech888.com.cn

PHP:  exit(1);
来源：http://oz.hnjuh.cn

JS:   process.exit(1)
来源：http://zc.huanxung.cn

TS:   process.exit(1)
来源：http://oe.yuexingan06.cn

Java: System.exit(1)
来源：http://as.panjiajie.cn

Go:   os.Exit(1)
来源：http://vk.huanxung.cn

Ruby: exit 1
来源：http://rz.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yx.jctech888.com.cn

[M06] 向标准错误输出
来源：http://mi.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://tb.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fj.huixiangedu.cn

JS:   console.error("err")
来源：http://na.huixiangedu.cn

TS:   console.error("err")
来源：http://ti.yuexingan06.cn

Java: System.err.println("err")
来源：http://rh.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pd.yuntaijiaju.cn

Ruby: warn "err"
来源：http://rq.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://qe.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://us.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://tc.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wp.jianghongdianzi.cn

JS:   require.main === module
来源：http://vx.szxytkj.cn

TS:   require.main === module
来源：http://ps.lnxyls.cn

Java: public static void main(String[] args)
来源：http://ra.hahajie.cn

Go:   func main()
来源：http://wl.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mj.newstarts.cn

C#:   static void Main(string[] args)
来源：http://cl.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://np.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://vw.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://of.gzmigu.cn

JS:   process.platform;  process.version
来源：http://mi.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://kb.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://le.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cz.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zs.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hf.gzmigu.cn

================================================================================
来源：http://xi.hahajie.cn

N. 数据结构与算法
来源：http://sf.szxytkj.cn

================================================================================
来源：http://hs.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://cq.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lp.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gn.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eu.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ok.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kv.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://jg.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uj.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ua.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://kq.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://wi.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sp.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yl.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wf.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hf.asd995.cn

Go:   slices.Sort(arr)
来源：http://ko.hnjuh.cn

Ruby: arr.sort
来源：http://nr.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eo.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://hq.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nu.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://iz.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bn.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ai.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mp.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oy.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://th.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rl.shtwfgs.cn

[N04] 斐波那契数列
来源：http://uq.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gd.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lr.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cv.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yr.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qh.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yj.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ez.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mn.hnjuh.cn

[N05] 最大公约数
来源：http://el.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://wa.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lf.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jx.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mz.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ps.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qp.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://dx.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cj.colortex.cn

[N06] 判断回文字符串
来源：http://ff.gzmigu.cn

Py:   s == s[::-1]
来源：http://ir.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://bt.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://hx.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://nd.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://to.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://wm.huanxung.cn

Ruby: s == s.reverse
来源：http://su.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wz.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://pw.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://em.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jb.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dp.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://lj.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://di.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://ky.lnxyls.cn

Ruby: // 手写 Hash
来源：http://om.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dd.hnjuh.cn

[N08] 生成全排列
来源：http://ir.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://uj.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://yp.shxzskj.cn

JS:   // 手写回溯递归
来源：http://qj.9csxet.cn

TS:   // 手写回溯递归
来源：http://yj.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://si.panjiajie.cn

Go:   // 手写回溯递归
来源：http://bo.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://de.521024.cn

C#:   // 手写回溯递归
来源：http://qn.nszjky.cn

[N09] 栈与队列
来源：http://pc.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ss.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yh.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nw.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qe.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xz.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yw.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vn.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://la.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://wt.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oj.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jd.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yr.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ku.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://wk.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iu.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ix.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jy.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://jt.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gk.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://yc.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gr.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://of.panjiajie.cn

Java: // 手写递归
来源：http://fo.shxzukj.cn

Go:   // 手写递归
来源：http://dc.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ps.szxytkj.cn

C#:   // 手写递归
来源：http://ga.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bo.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vq.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rk.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tt.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ts.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://re.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fx.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://we.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jd.huixinmuqiang.cn

================================================================================
来源：http://sy.gzmigu.cn

O. 并发与异步
来源：http://cr.hnjuh.cn

================================================================================
来源：http://ow.bookmarksfly.cn

[O01] 启动一个线程
来源：http://gt.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://su.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ha.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qb.9csxet.cn

TS:   // 同 JS
来源：http://ru.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://ct.hahajie.cn

Go:   go f()
来源：http://ef.lnxyls.cn

Ruby: Thread.new { f }
来源：http://sk.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://mi.yuntaijiaju.cn

[O02] 使用线程池
来源：http://tl.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ys.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gd.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://jz.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://ba.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ug.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://et.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://md.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://so.nszjky.cn

[O03] 加锁保护共享数据
来源：http://yl.shxzukj.cn

Py:   with lock: shared += 1
来源：http://cj.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://px.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hn.shxzukj.cn

TS:   // 同 JS
来源：http://ay.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://nm.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jy.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ya.521024.cn

C#:   lock (gate) { shared++; }
来源：http://pi.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://ow.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://tp.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wy.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://kn.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eo.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dk.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gn.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qz.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://lq.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ur.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://kb.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mz.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://lx.asd995.cn

TS:   await Promise.all(tasks)
来源：http://sm.nicolike.cn


<!-- 参考信息 -->