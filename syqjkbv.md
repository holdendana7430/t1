代发 wailian999

L. 网络请求
来源：http://yf.hahajie.cn

================================================================================
来源：http://mq.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://uy.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oi.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://md.9csxet.cn

JS:   await fetch(url)
来源：http://jb.hahajie.cn

TS:   await fetch(url)
来源：http://lz.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ye.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://th.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fz.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://at.hahajie.cn

[L02] 发送 POST JSON
来源：http://qa.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wy.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zo.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yu.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tf.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jr.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zs.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kv.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nv.hahajie.cn

[L03] 设置自定义请求头
来源：http://zu.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ql.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aj.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://js.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hk.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qo.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oo.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jd.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gm.huanxung.cn

[L04] 设置超时
来源：http://qk.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://kv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kk.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jv.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gn.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kj.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xo.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yr.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lp.huanxung.cn

[L05] 上传文件（multipart）
来源：http://qb.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oo.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ep.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wx.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lw.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wx.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jc.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jf.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bl.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://gb.521024.cn

Py:   resp.json()
来源：http://aw.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://iz.szxytkj.cn

JS:   await resp.json()
来源：http://xc.asd995.cn

TS:   await resp.json()
来源：http://bx.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://un.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rx.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://yv.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wn.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://gu.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hw.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xj.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ei.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://mv.haigaiapp.cn

Java: resp.statusCode()
来源：http://ug.jctech888.com.cn

Go:   resp.StatusCode
来源：http://pd.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://oz.521024.cn

C#:   (int)resp.StatusCode
来源：http://qg.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://xz.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://va.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://hi.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ms.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ix.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tl.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hc.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ln.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vk.lnxyls.cn

================================================================================
来源：http://dp.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://xw.jctech888.com.cn

================================================================================
来源：http://vh.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://ey.newstarts.cn

Py:   sys.argv[1:]
来源：http://kq.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://tq.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://sq.521024.cn

TS:   process.argv.slice(2)
来源：http://wk.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://vw.shxzukj.cn

Go:   os.Args[1:]
来源：http://vc.yuntaijiaju.cn

Ruby: ARGV
来源：http://wk.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://fb.jctech888.com.cn

[M02] 读取环境变量
来源：http://yc.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://jv.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cb.hnjuh.cn

JS:   process.env.HOME
来源：http://fj.huanxung.cn

TS:   process.env.HOME
来源：http://nt.panjiajie.cn

Java: System.getenv("HOME")
来源：http://yt.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ex.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://df.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ao.yuexingan06.cn

[M03] 执行外部命令
来源：http://jf.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lc.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zm.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jg.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uk.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xe.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wb.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gg.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://yf.colortex.cn

[M04] 获取当前工作目录
来源：http://tb.gzmigu.cn

Py:   os.getcwd()
来源：http://wt.nicolike.cn

PHP:  getcwd();
来源：http://eh.shxzskj.cn

JS:   process.cwd()
来源：http://cc.bjjhwx.cn

TS:   process.cwd()
来源：http://ir.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://dv.shtwfgs.cn

Go:   os.Getwd()
来源：http://rb.haigaiapp.cn

Ruby: Dir.pwd
来源：http://to.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mh.lnxyls.cn

[M05] 设置退出码
来源：http://qm.9csxet.cn

Py:   sys.exit(1)
来源：http://mp.9csxet.cn

PHP:  exit(1);
来源：http://xl.521024.cn

JS:   process.exit(1)
来源：http://go.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ka.yuntaijiaju.cn

Java: System.exit(1)
来源：http://ep.wgjwhj.cn

Go:   os.Exit(1)
来源：http://oc.panjiajie.cn

Ruby: exit 1
来源：http://yp.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zn.chemitech.net.cn

[M06] 向标准错误输出
来源：http://tp.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://bo.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hp.lnxyls.cn

JS:   console.error("err")
来源：http://kc.shxzukj.cn

TS:   console.error("err")
来源：http://ft.szxytkj.cn

Java: System.err.println("err")
来源：http://ni.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://im.hnjuh.cn

Ruby: warn "err"
来源：http://lo.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://bd.shxzukj.cn

[M07] 判断是否为主入口
来源：http://th.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://mh.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://av.gzmigu.cn

JS:   require.main === module
来源：http://dx.shxzukj.cn

TS:   require.main === module
来源：http://qh.nicolike.cn

Java: public static void main(String[] args)
来源：http://ju.nicolike.cn

Go:   func main()
来源：http://wj.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://na.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://xb.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://dd.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://eg.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ex.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://sz.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://mz.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://if.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://it.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rq.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ft.9csxet.cn

================================================================================
来源：http://py.9csxet.cn

N. 数据结构与算法
来源：http://uu.nszjky.cn

================================================================================
来源：http://pp.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://rw.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uz.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cq.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gh.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ps.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jh.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://ar.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sx.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ib.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://wf.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://zc.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rg.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gy.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ai.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://by.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://az.nicolike.cn

Ruby: arr.sort
来源：http://ch.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xw.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://pu.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xa.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ef.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://un.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yc.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jv.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ov.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tn.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hf.hnjuh.cn

[N04] 斐波那契数列
来源：http://vz.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dx.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cg.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://km.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nx.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hl.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oi.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ym.haigaiapp.cn

[N05] 最大公约数
来源：http://ir.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://ng.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ki.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qc.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ri.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wj.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pf.lnxyls.cn

Ruby: a.gcd(b)
来源：http://zc.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ow.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://bp.wgjwhj.cn

Py:   s == s[::-1]
来源：http://hv.asd995.cn

PHP:  $s === strrev($s);
来源：http://dd.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://vo.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://yr.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pt.szsharing.cn

Go:   // 双指针从两端比较
来源：http://gy.nszjky.cn

Ruby: s == s.reverse
来源：http://bs.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uk.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://pb.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ui.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qu.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uw.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://af.panjiajie.cn

Java: // 手写 HashMap
来源：http://sy.asd995.cn

Go:   // 手写 map[int]int
来源：http://zf.colortex.cn

Ruby: // 手写 Hash
来源：http://hp.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qs.shxzukj.cn

[N08] 生成全排列
来源：http://vi.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://tu.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://zy.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://zc.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://on.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://ex.newstarts.cn

Go:   // 手写回溯递归
来源：http://lz.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://nl.asd995.cn

C#:   // 手写回溯递归
来源：http://jd.yuntaijiaju.cn

[N09] 栈与队列
来源：http://xv.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ol.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tp.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jy.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ve.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oo.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qz.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yv.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sg.gzmigu.cn

[N10] 链表节点定义
来源：http://tp.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dq.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kd.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xt.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://id.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://sv.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xk.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vh.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://he.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://ii.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ea.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://hz.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://au.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ow.jctech888.com.cn

Java: // 手写递归
来源：http://ch.wgjwhj.cn

Go:   // 手写递归
来源：http://gc.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jz.lnxyls.cn

C#:   // 手写递归
来源：http://fe.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qp.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://id.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cq.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fo.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sk.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ub.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fw.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mg.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pw.jianghongdianzi.cn

================================================================================
来源：http://hm.521024.cn

O. 并发与异步
来源：http://op.shtwfgs.cn

================================================================================
来源：http://tw.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://qj.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gn.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ve.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mb.yuexingan06.cn

TS:   // 同 JS
来源：http://rw.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ih.bjjhwx.cn

Go:   go f()
来源：http://pc.hahajie.cn

Ruby: Thread.new { f }
来源：http://ww.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://ni.yuexingan06.cn

[O02] 使用线程池
来源：http://mg.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rv.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ex.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://au.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://fy.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ll.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mx.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pk.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fu.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://ub.9csxet.cn

Py:   with lock: shared += 1
来源：http://uf.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://pq.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ru.lnxyls.cn

TS:   // 同 JS
来源：http://uk.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://oo.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wf.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ey.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://cx.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://te.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://iu.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jg.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://nf.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://in.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mp.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ji.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ag.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://vq.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://bq.muxihuayi.cn


<!-- 参考信息 -->