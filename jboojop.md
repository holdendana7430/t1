代发 wailian999

L. 网络请求
来源：http://uh.lnxyls.cn

================================================================================
来源：http://tl.shxzukj.cn

[L01] 发送 GET 请求
来源：http://cl.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eb.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mf.shxzskj.cn

JS:   await fetch(url)
来源：http://ik.szxytkj.cn

TS:   await fetch(url)
来源：http://il.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uy.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://pb.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kx.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ua.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://wn.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kj.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hs.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kb.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xw.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ty.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zj.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fv.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://we.hahajie.cn

[L03] 设置自定义请求头
来源：http://am.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ad.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zz.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ll.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ao.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kf.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://si.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jh.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sp.wgjwhj.cn

[L04] 设置超时
来源：http://ew.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://sm.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://od.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zx.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hb.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wi.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vg.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://do.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://ja.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ie.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://if.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eo.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://il.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ka.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zv.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zg.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oi.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://zx.muxihuayi.cn

Py:   resp.json()
来源：http://yf.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://he.hnjuh.cn

JS:   await resp.json()
来源：http://tq.shtwfgs.cn

TS:   await resp.json()
来源：http://ua.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vr.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zx.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ri.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kd.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://pj.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sk.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://as.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://sp.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://kh.9csxet.cn

Java: resp.statusCode()
来源：http://yn.nicolike.cn

Go:   resp.StatusCode
来源：http://ld.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://ff.colortex.cn

C#:   (int)resp.StatusCode
来源：http://nw.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://xu.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dc.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://vg.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://al.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ru.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yg.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zu.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xh.nicolike.cn

================================================================================
来源：http://wp.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://oe.shxzukj.cn

================================================================================
来源：http://ob.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://vd.asd995.cn

Py:   sys.argv[1:]
来源：http://xz.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://wb.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://zp.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://uu.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://er.hnjuh.cn

Go:   os.Args[1:]
来源：http://uf.bjjhwx.cn

Ruby: ARGV
来源：http://bi.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://go.asd995.cn

[M02] 读取环境变量
来源：http://ac.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://iw.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ri.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://wh.9csxet.cn

TS:   process.env.HOME
来源：http://jx.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://pz.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yp.asd995.cn

Ruby: ENV["HOME"]
来源：http://ch.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fp.hnjuh.cn

[M03] 执行外部命令
来源：http://bz.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hj.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vt.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dc.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iu.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ny.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vu.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://en.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://ab.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ka.9csxet.cn

Py:   os.getcwd()
来源：http://ki.9csxet.cn

PHP:  getcwd();
来源：http://yb.huanxung.cn

JS:   process.cwd()
来源：http://vl.panjiajie.cn

TS:   process.cwd()
来源：http://gr.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://mf.shxzskj.cn

Go:   os.Getwd()
来源：http://go.colortex.cn

Ruby: Dir.pwd
来源：http://ob.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dt.gzmigu.cn

[M05] 设置退出码
来源：http://dv.nszjky.cn

Py:   sys.exit(1)
来源：http://gw.wgjwhj.cn

PHP:  exit(1);
来源：http://ie.wgjwhj.cn

JS:   process.exit(1)
来源：http://zh.yuexingan06.cn

TS:   process.exit(1)
来源：http://ry.shxzskj.cn

Java: System.exit(1)
来源：http://jy.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ec.gzmigu.cn

Ruby: exit 1
来源：http://ja.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tx.chemitech.net.cn

[M06] 向标准错误输出
来源：http://xr.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://uz.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tj.nicolike.cn

JS:   console.error("err")
来源：http://hy.huanxung.cn

TS:   console.error("err")
来源：http://oc.huixiangedu.cn

Java: System.err.println("err")
来源：http://hq.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nh.yuexingan06.cn

Ruby: warn "err"
来源：http://wu.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://me.panjiajie.cn

[M07] 判断是否为主入口
来源：http://ti.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://js.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ne.9csxet.cn

JS:   require.main === module
来源：http://ux.521024.cn

TS:   require.main === module
来源：http://sf.hahajie.cn

Java: public static void main(String[] args)
来源：http://ee.panjiajie.cn

Go:   func main()
来源：http://fv.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zo.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://iz.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://ul.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://qy.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://cj.szsharing.cn

JS:   process.platform;  process.version
来源：http://yd.shxzskj.cn

TS:   process.platform;  process.version
来源：http://lh.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ir.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ks.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vo.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bd.hahajie.cn

================================================================================
来源：http://ce.haigaiapp.cn

N. 数据结构与算法
来源：http://wt.wgjwhj.cn

================================================================================
来源：http://rd.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://mx.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qd.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ft.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nv.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zr.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vk.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://wb.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pz.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ck.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zf.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://pq.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://il.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hf.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ub.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zy.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://fg.nszjky.cn

Ruby: arr.sort
来源：http://hm.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cc.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://mf.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://km.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ll.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qe.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://og.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vi.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zl.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wp.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ta.nicolike.cn

[N04] 斐波那契数列
来源：http://pz.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oh.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cf.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://en.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yx.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pi.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://or.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bs.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uy.panjiajie.cn

[N05] 最大公约数
来源：http://wm.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://kc.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gh.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qa.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vb.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://au.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mw.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://oe.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ue.9csxet.cn

[N06] 判断回文字符串
来源：http://ep.chemitech.net.cn

Py:   s == s[::-1]
来源：http://xg.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://td.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ey.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://yk.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ic.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ky.yuexingan06.cn

Ruby: s == s.reverse
来源：http://cl.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fq.colortex.cn

[N07] 两数之和（返回下标）
来源：http://jy.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mq.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qf.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gf.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://bx.asd995.cn

Java: // 手写 HashMap
来源：http://zc.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ae.szxytkj.cn

Ruby: // 手写 Hash
来源：http://mi.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://er.bjjhwx.cn

[N08] 生成全排列
来源：http://xb.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://cw.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://cx.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://fa.gzmigu.cn

TS:   // 手写回溯递归
来源：http://hx.9csxet.cn

Java: // 手写回溯递归
来源：http://wk.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://gs.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://jm.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://hk.hahajie.cn

[N09] 栈与队列
来源：http://np.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wf.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ou.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lc.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ak.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hu.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vr.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qg.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gw.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://qg.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dl.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ib.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uf.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xr.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://fc.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dr.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://or.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uf.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://lc.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ee.newstarts.cn

PHP:  // 手写递归函数
来源：http://wg.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nq.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.yuexingan06.cn

Java: // 手写递归
来源：http://dc.nszjky.cn

Go:   // 手写递归
来源：http://te.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jy.gzmigu.cn

C#:   // 手写递归
来源：http://rz.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ba.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kr.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ja.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uy.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dm.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yy.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sz.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ie.huixiangedu.cn

================================================================================
来源：http://he.hahajie.cn

O. 并发与异步
来源：http://sy.yuexingan06.cn

================================================================================
来源：http://wg.gzmigu.cn

[O01] 启动一个线程
来源：http://zn.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ms.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pr.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xq.newstarts.cn

TS:   // 同 JS
来源：http://qt.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://gd.hnjuh.cn

Go:   go f()
来源：http://jh.hnjuh.cn

Ruby: Thread.new { f }
来源：http://in.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://ba.521024.cn

[O02] 使用线程池
来源：http://pr.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rx.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://is.nicolike.cn

JS:   // worker_threads 线程池
来源：http://we.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://ml.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ro.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xo.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ct.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wi.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://nq.nszjky.cn

Py:   with lock: shared += 1
来源：http://gq.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://dw.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cu.nszjky.cn

TS:   // 同 JS
来源：http://mv.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://vw.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://px.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lk.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://mj.asd995.cn

[O04] 定义异步函数并等待
来源：http://yo.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://lb.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pe.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://kn.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hk.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ns.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mv.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qd.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://qd.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://ez.szxytkj.cn


<!-- 参考信息 -->