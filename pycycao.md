代发 wailian999

L. 网络请求
来源：http://ps.521024.cn

================================================================================
来源：http://fs.panjiajie.cn

[L01] 发送 GET 请求
来源：http://ct.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ub.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zz.nszjky.cn

JS:   await fetch(url)
来源：http://an.9csxet.cn

TS:   await fetch(url)
来源：http://dl.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wn.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://xe.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ph.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ec.nicolike.cn

[L02] 发送 POST JSON
来源：http://ei.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ng.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dw.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xd.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bg.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bx.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rr.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kh.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cd.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://xs.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ow.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pl.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wr.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dt.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://as.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://je.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sn.wgjwhj.cn

[L04] 设置超时
来源：http://cw.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://xw.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cg.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bl.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ea.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fd.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://az.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fh.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://va.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://cz.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gg.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tj.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oc.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pe.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wx.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qi.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://em.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wl.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://bo.panjiajie.cn

Py:   resp.json()
来源：http://ms.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://wu.jctech888.com.cn

JS:   await resp.json()
来源：http://er.jianghongdianzi.cn

TS:   await resp.json()
来源：http://sf.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fz.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://og.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://kl.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pb.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://rd.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hv.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bm.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://pn.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://nd.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://az.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://up.gzmigu.cn

Ruby: resp.code.to_i
来源：http://lc.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://mz.colortex.cn

[L08] 并发请求多个地址
来源：http://gk.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qo.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://ge.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cc.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oc.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fn.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yi.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bo.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mx.chemitech.net.cn

================================================================================
来源：http://or.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://cx.yuntaijiaju.cn

================================================================================
来源：http://si.hnjuh.cn

[M01] 读取命令行参数
来源：http://yf.lnxyls.cn

Py:   sys.argv[1:]
来源：http://fy.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://wp.521024.cn

JS:   process.argv.slice(2)
来源：http://dw.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://eu.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://zp.asd995.cn

Go:   os.Args[1:]
来源：http://lo.panjiajie.cn

Ruby: ARGV
来源：http://yt.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://bt.colortex.cn

[M02] 读取环境变量
来源：http://dq.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://sd.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kb.asd995.cn

JS:   process.env.HOME
来源：http://jw.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://ba.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://ee.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ph.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://lv.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dm.asd995.cn

[M03] 执行外部命令
来源：http://lr.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tb.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nb.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sl.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fu.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bm.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ti.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://cr.9csxet.cn

[M04] 获取当前工作目录
来源：http://yw.9csxet.cn

Py:   os.getcwd()
来源：http://sn.wgjwhj.cn

PHP:  getcwd();
来源：http://ka.huixiangedu.cn

JS:   process.cwd()
来源：http://nh.hahajie.cn

TS:   process.cwd()
来源：http://aj.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://on.bookmarksfly.cn

Go:   os.Getwd()
来源：http://fd.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://kx.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tm.yuexingan06.cn

[M05] 设置退出码
来源：http://pf.chemitech.net.cn

Py:   sys.exit(1)
来源：http://re.colortex.cn

PHP:  exit(1);
来源：http://gb.nszjky.cn

JS:   process.exit(1)
来源：http://rr.shxzskj.cn

TS:   process.exit(1)
来源：http://pi.wgjwhj.cn

Java: System.exit(1)
来源：http://cs.shxzukj.cn

Go:   os.Exit(1)
来源：http://hg.chemitech.net.cn

Ruby: exit 1
来源：http://ir.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cc.nszjky.cn

[M06] 向标准错误输出
来源：http://pk.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://kh.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sb.panjiajie.cn

JS:   console.error("err")
来源：http://jp.chemitech.net.cn

TS:   console.error("err")
来源：http://uw.panjiajie.cn

Java: System.err.println("err")
来源：http://tq.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ft.colortex.cn

Ruby: warn "err"
来源：http://dw.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://wx.shxzskj.cn

[M07] 判断是否为主入口
来源：http://ty.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://fi.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dd.bjjhwx.cn

JS:   require.main === module
来源：http://qi.asd995.cn

TS:   require.main === module
来源：http://cu.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://uy.huanxung.cn

Go:   func main()
来源：http://xo.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ov.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://yi.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://fj.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://ay.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://di.9csxet.cn

JS:   process.platform;  process.version
来源：http://rh.shxzukj.cn

TS:   process.platform;  process.version
来源：http://hx.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ig.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dz.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://re.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yf.muxihuayi.cn

================================================================================
来源：http://dk.muxihuayi.cn

N. 数据结构与算法
来源：http://zj.yuntaijiaju.cn

================================================================================
来源：http://xz.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://uu.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ra.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hn.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cy.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tm.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://yp.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zi.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gl.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://hq.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://nw.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ry.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pb.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lq.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dr.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://za.lnxyls.cn

Ruby: arr.sort
来源：http://ki.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fp.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://mp.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ij.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://jh.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://up.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gc.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xb.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://er.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ja.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lj.szxytkj.cn

[N04] 斐波那契数列
来源：http://nl.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ea.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wn.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yg.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tc.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lj.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dq.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lz.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cl.jianghongdianzi.cn

[N05] 最大公约数
来源：http://vo.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://eu.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lj.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pm.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ir.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yv.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qc.shxzskj.cn

Ruby: a.gcd(b)
来源：http://ww.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ik.muxihuayi.cn

[N06] 判断回文字符串
来源：http://hu.chemitech.net.cn

Py:   s == s[::-1]
来源：http://xa.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://qj.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://lq.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://lr.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lv.huanxung.cn

Go:   // 双指针从两端比较
来源：http://wm.asd995.cn

Ruby: s == s.reverse
来源：http://wo.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bu.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://ph.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vb.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gl.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yv.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://ue.colortex.cn

Java: // 手写 HashMap
来源：http://xh.nicolike.cn

Go:   // 手写 map[int]int
来源：http://ng.hnjuh.cn

Ruby: // 手写 Hash
来源：http://nm.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ye.yuexingan06.cn

[N08] 生成全排列
来源：http://xi.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://di.panjiajie.cn

PHP:  // 手写递归交换
来源：http://jj.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://vm.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://rg.shxzukj.cn

Java: // 手写回溯递归
来源：http://ft.szsharing.cn

Go:   // 手写回溯递归
来源：http://hh.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://gu.lnxyls.cn

C#:   // 手写回溯递归
来源：http://sa.yuexingan06.cn

[N09] 栈与队列
来源：http://vj.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lw.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cq.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uo.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qs.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iq.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rg.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bc.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mc.szsharing.cn

[N10] 链表节点定义
来源：http://mx.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gd.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xh.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ja.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pm.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://rx.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pg.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gr.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fw.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://ji.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sw.huanxung.cn

PHP:  // 手写递归函数
来源：http://nk.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ca.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fv.yuntaijiaju.cn

Java: // 手写递归
来源：http://le.newstarts.cn

Go:   // 手写递归
来源：http://oa.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wi.521024.cn

C#:   // 手写递归
来源：http://qr.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ym.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bx.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hp.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ei.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cq.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gs.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yr.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fd.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eo.gzmigu.cn

================================================================================
来源：http://ql.jianghongdianzi.cn

O. 并发与异步
来源：http://bf.jctech888.com.cn

================================================================================
来源：http://pz.lnxyls.cn

[O01] 启动一个线程
来源：http://wf.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://av.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jn.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yi.jianghongdianzi.cn

TS:   // 同 JS
来源：http://em.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://yi.shtwfgs.cn

Go:   go f()
来源：http://nu.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://se.9csxet.cn

C#:   Task.Run(() => F());
来源：http://sa.yuntaijiaju.cn

[O02] 使用线程池
来源：http://ih.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://im.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eh.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://vu.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://hf.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rr.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jl.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kr.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kk.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://jz.521024.cn

Py:   with lock: shared += 1
来源：http://ko.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://nf.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ll.wgjwhj.cn

TS:   // 同 JS
来源：http://ko.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://nd.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kp.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://er.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://tb.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://nm.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://zn.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wf.9csxet.cn

JS:   async function f() { await g(); }
来源：http://fj.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pb.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ct.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fr.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zn.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://st.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://tz.szxytkj.cn


<!-- 参考信息 -->