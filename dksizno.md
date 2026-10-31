代发 wailian999

Go:   encoding/gob
来源：http://ht.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://zm.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wp.gzmigu.cn

================================================================================
来源：http://ni.szsharing.cn

L. 网络请求
来源：http://yi.chemitech.net.cn

================================================================================
来源：http://rn.9csxet.cn

[L01] 发送 GET 请求
来源：http://ra.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uw.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://al.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://jd.huanxung.cn

TS:   await fetch(url)
来源：http://cz.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://db.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://hm.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ft.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oh.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://uv.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://le.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vx.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gv.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rz.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gc.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://no.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cz.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iz.shxzskj.cn

[L03] 设置自定义请求头
来源：http://rc.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ie.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jn.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kh.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rv.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lt.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lp.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uk.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sh.shxzskj.cn

[L04] 设置超时
来源：http://jp.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://xh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gz.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://co.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hr.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ta.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mv.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rz.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gp.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://en.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oq.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cn.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ue.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://li.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bv.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nj.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hf.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ts.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://fj.9csxet.cn

Py:   resp.json()
来源：http://qo.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ve.hnjuh.cn

JS:   await resp.json()
来源：http://ck.asd995.cn

TS:   await resp.json()
来源：http://co.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://al.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ol.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ec.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ym.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://ap.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xn.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dk.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://wo.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://gc.szxytkj.cn

Java: resp.statusCode()
来源：http://ax.hnjuh.cn

Go:   resp.StatusCode
来源：http://pi.shxzukj.cn

Ruby: resp.code.to_i
来源：http://jy.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://wy.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://dt.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vn.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://zw.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sf.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ch.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rf.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bk.huixinmuqiang.cn

================================================================================
来源：http://zv.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ga.jctech888.com.cn

================================================================================
来源：http://dc.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://cc.panjiajie.cn

Py:   sys.argv[1:]
来源：http://yq.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://rd.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://sv.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://cg.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://nd.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://bi.huanxung.cn

Ruby: ARGV
来源：http://bv.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ez.nszjky.cn

[M02] 读取环境变量
来源：http://vu.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://ym.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yi.gzmigu.cn

JS:   process.env.HOME
来源：http://gf.bookmarksfly.cn

TS:   process.env.HOME
来源：http://mx.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://ix.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gd.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://gb.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ys.521024.cn

[M03] 执行外部命令
来源：http://zp.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mt.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ki.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lj.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://an.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kn.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wu.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ht.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://fo.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://rh.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://iw.yuntaijiaju.cn

PHP:  getcwd();
来源：http://cy.chemitech.net.cn

JS:   process.cwd()
来源：http://ju.szsharing.cn

TS:   process.cwd()
来源：http://xu.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ij.521024.cn

Go:   os.Getwd()
来源：http://vg.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://gd.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uz.chemitech.net.cn

[M05] 设置退出码
来源：http://ba.nicolike.cn

Py:   sys.exit(1)
来源：http://ws.jctech888.com.cn

PHP:  exit(1);
来源：http://ef.nszjky.cn

JS:   process.exit(1)
来源：http://sm.shtwfgs.cn

TS:   process.exit(1)
来源：http://zk.szsharing.cn

Java: System.exit(1)
来源：http://vz.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://zq.huixiangedu.cn

Ruby: exit 1
来源：http://pq.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ys.hahajie.cn

[M06] 向标准错误输出
来源：http://yg.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://pd.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tk.jctech888.com.cn

JS:   console.error("err")
来源：http://lb.newstarts.cn

TS:   console.error("err")
来源：http://ng.wgjwhj.cn

Java: System.err.println("err")
来源：http://nt.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tz.shxzukj.cn

Ruby: warn "err"
来源：http://to.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://cy.shxzukj.cn

[M07] 判断是否为主入口
来源：http://uj.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ak.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ny.gzmigu.cn

JS:   require.main === module
来源：http://ws.521024.cn

TS:   require.main === module
来源：http://uy.9csxet.cn

Java: public static void main(String[] args)
来源：http://fo.asd995.cn

Go:   func main()
来源：http://li.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vb.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://rd.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://cw.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://bz.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://up.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ol.szxytkj.cn

TS:   process.platform;  process.version
来源：http://iv.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uj.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mj.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xv.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ck.huixiangedu.cn

================================================================================
来源：http://hn.hnjuh.cn

N. 数据结构与算法
来源：http://mg.colortex.cn

================================================================================
来源：http://dq.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://pl.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bp.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ym.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qz.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://uj.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cx.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qn.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://uc.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://fx.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pf.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rv.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rl.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://td.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://jk.huixiangedu.cn

Ruby: arr.sort
来源：http://kg.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hd.asd995.cn

[N03] 快速排序（分治示例）
来源：http://wn.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://td.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://hg.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pn.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://on.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aa.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://es.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://et.gzmigu.cn

[N04] 斐波那契数列
来源：http://zm.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yw.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://at.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://py.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rk.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fa.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fd.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hd.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://av.huixinmuqiang.cn

[N05] 最大公约数
来源：http://or.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://br.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://br.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fl.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vs.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ko.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cv.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://hx.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ds.nszjky.cn

[N06] 判断回文字符串
来源：http://xm.wgjwhj.cn

Py:   s == s[::-1]
来源：http://kl.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://nx.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://vx.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://we.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ni.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://gp.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://wc.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xd.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://dv.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ip.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ks.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://vz.521024.cn

Java: // 手写 HashMap
来源：http://ye.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://kn.9csxet.cn

Ruby: // 手写 Hash
来源：http://lg.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ql.huixiangedu.cn

[N08] 生成全排列
来源：http://nu.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://ze.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://kj.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://vy.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://xh.shxzskj.cn

Java: // 手写回溯递归
来源：http://ek.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ee.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ja.colortex.cn

C#:   // 手写回溯递归
来源：http://sa.haigaiapp.cn

[N09] 栈与队列
来源：http://pc.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ab.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://th.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://um.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kx.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kt.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ut.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ky.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vm.szxytkj.cn

[N10] 链表节点定义
来源：http://ow.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hy.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uv.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wt.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tz.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://mb.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ue.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ed.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zl.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://vu.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dt.hahajie.cn

PHP:  // 手写递归函数
来源：http://ho.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mr.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ow.nicolike.cn

Java: // 手写递归
来源：http://dd.jianghongdianzi.cn

Go:   // 手写递归
来源：http://yn.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ut.panjiajie.cn

C#:   // 手写递归
来源：http://xk.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lp.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sy.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yg.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ub.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vm.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jr.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uu.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://to.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hd.asd995.cn

================================================================================
来源：http://ar.521024.cn

O. 并发与异步
来源：http://ri.szxytkj.cn

================================================================================
来源：http://gi.yuexingan06.cn

[O01] 启动一个线程
来源：http://hi.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rh.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dp.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sh.huanxung.cn

TS:   // 同 JS
来源：http://zz.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://tj.shxzukj.cn

Go:   go f()
来源：http://bm.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://zj.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://hg.jctech888.com.cn

[O02] 使用线程池
来源：http://sw.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nc.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lz.521024.cn

JS:   // worker_threads 线程池
来源：http://kv.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://dt.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://os.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nh.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fn.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kg.nicolike.cn

[O03] 加锁保护共享数据
来源：http://xg.9csxet.cn

Py:   with lock: shared += 1
来源：http://bb.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://za.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oa.chemitech.net.cn

TS:   // 同 JS
来源：http://pf.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://hq.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yq.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sh.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://vv.asd995.cn

[O04] 定义异步函数并等待
来源：http://or.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://xg.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://il.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://lc.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vd.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zd.chemitech.net.cn


<!-- 参考信息 -->