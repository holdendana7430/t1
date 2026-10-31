代发 wailian999

Go:   encoding/gob
来源：http://pk.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://ac.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jg.shxzskj.cn

================================================================================
来源：http://yg.bookmarksfly.cn

L. 网络请求
来源：http://id.colortex.cn

================================================================================
来源：http://hj.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://ca.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fn.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oe.huixiangedu.cn

JS:   await fetch(url)
来源：http://zd.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://um.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ql.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://xi.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zy.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kp.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://uq.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mj.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hj.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nn.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ag.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cs.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jr.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kc.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://za.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://cz.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yk.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tf.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ai.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ri.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kb.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jg.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mr.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wc.yuntaijiaju.cn

[L04] 设置超时
来源：http://kt.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://gn.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ax.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sm.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mm.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xu.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fl.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://th.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bi.szsharing.cn

[L05] 上传文件（multipart）
来源：http://uh.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jm.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lq.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fh.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ae.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ze.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://db.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xc.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ak.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://gq.bookmarksfly.cn

Py:   resp.json()
来源：http://ed.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://us.bjjhwx.cn

JS:   await resp.json()
来源：http://et.9csxet.cn

TS:   await resp.json()
来源：http://rf.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dy.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ta.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://xi.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bz.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://nh.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yr.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nv.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://bc.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://jk.asd995.cn

Java: resp.statusCode()
来源：http://dc.lnxyls.cn

Go:   resp.StatusCode
来源：http://ww.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://rd.521024.cn

C#:   (int)resp.StatusCode
来源：http://rw.panjiajie.cn

[L08] 并发请求多个地址
来源：http://qt.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tl.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://iv.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yu.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tb.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://je.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rx.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fz.hnjuh.cn

================================================================================
来源：http://gn.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://xk.huixiangedu.cn

================================================================================
来源：http://pn.jctech888.com.cn

[M01] 读取命令行参数
来源：http://ce.hnjuh.cn

Py:   sys.argv[1:]
来源：http://fh.szsharing.cn

PHP:  $argv;  $argc;
来源：http://op.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://tn.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ly.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://rs.bjjhwx.cn

Go:   os.Args[1:]
来源：http://df.shxzukj.cn

Ruby: ARGV
来源：http://ka.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://bk.muxihuayi.cn

[M02] 读取环境变量
来源：http://bk.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://th.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ts.lnxyls.cn

JS:   process.env.HOME
来源：http://gi.9csxet.cn

TS:   process.env.HOME
来源：http://oh.asd995.cn

Java: System.getenv("HOME")
来源：http://ee.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ou.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://us.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jt.shxzskj.cn

[M03] 执行外部命令
来源：http://lb.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vp.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gi.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kb.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pn.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tv.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bm.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jq.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://or.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://yy.panjiajie.cn

Py:   os.getcwd()
来源：http://my.bjjhwx.cn

PHP:  getcwd();
来源：http://ip.shxzukj.cn

JS:   process.cwd()
来源：http://ff.nszjky.cn

TS:   process.cwd()
来源：http://xq.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://nz.muxihuayi.cn

Go:   os.Getwd()
来源：http://ct.chemitech.net.cn

Ruby: Dir.pwd
来源：http://xc.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hx.szsharing.cn

[M05] 设置退出码
来源：http://dp.szsharing.cn

Py:   sys.exit(1)
来源：http://oh.lnxyls.cn

PHP:  exit(1);
来源：http://ab.nszjky.cn

JS:   process.exit(1)
来源：http://rw.huanxung.cn

TS:   process.exit(1)
来源：http://ur.bjjhwx.cn

Java: System.exit(1)
来源：http://mn.9csxet.cn

Go:   os.Exit(1)
来源：http://ct.lnxyls.cn

Ruby: exit 1
来源：http://gc.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lx.huanxung.cn

[M06] 向标准错误输出
来源：http://jv.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://zh.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xm.chemitech.net.cn

JS:   console.error("err")
来源：http://ve.haigaiapp.cn

TS:   console.error("err")
来源：http://lk.huanxung.cn

Java: System.err.println("err")
来源：http://qd.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dx.nicolike.cn

Ruby: warn "err"
来源：http://ni.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://mr.nicolike.cn

[M07] 判断是否为主入口
来源：http://ud.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://ko.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://es.bjjhwx.cn

JS:   require.main === module
来源：http://hm.asd995.cn

TS:   require.main === module
来源：http://ps.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ee.yuexingan06.cn

Go:   func main()
来源：http://be.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rq.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://mm.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://cl.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://pv.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://cc.9csxet.cn

JS:   process.platform;  process.version
来源：http://zw.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ko.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hi.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ro.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bd.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pa.hahajie.cn

================================================================================
来源：http://ge.colortex.cn

N. 数据结构与算法
来源：http://ir.colortex.cn

================================================================================
来源：http://lb.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://hf.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ah.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dk.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oh.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bv.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yo.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://bl.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ry.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ws.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://vs.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://tp.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://in.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ue.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vp.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ge.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://qg.asd995.cn

Ruby: arr.sort
来源：http://ow.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iq.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://sh.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zs.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://xv.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sa.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bs.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jd.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gk.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gx.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://go.nicolike.cn

[N04] 斐波那契数列
来源：http://wt.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qa.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ui.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cm.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uy.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qx.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://op.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gi.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://db.hahajie.cn

[N05] 最大公约数
来源：http://qh.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://wn.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tq.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://or.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rn.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bu.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ft.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://zo.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uv.bjjhwx.cn

[N06] 判断回文字符串
来源：http://mz.newstarts.cn

Py:   s == s[::-1]
来源：http://vu.9csxet.cn

PHP:  $s === strrev($s);
来源：http://jw.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://xm.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://wq.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ul.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://sw.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ju.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gi.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://mp.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nw.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ip.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zy.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ns.shxzukj.cn

Java: // 手写 HashMap
来源：http://vu.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://dv.newstarts.cn

Ruby: // 手写 Hash
来源：http://ks.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yb.hnjuh.cn

[N08] 生成全排列
来源：http://uw.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://mp.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://qn.hahajie.cn

JS:   // 手写回溯递归
来源：http://og.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://vb.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://zk.hahajie.cn

Go:   // 手写回溯递归
来源：http://lq.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://se.lnxyls.cn

C#:   // 手写回溯递归
来源：http://sw.yuexingan06.cn

[N09] 栈与队列
来源：http://ws.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://db.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bm.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://um.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dd.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xj.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ie.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fb.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ki.haigaiapp.cn

[N10] 链表节点定义
来源：http://tr.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rx.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uz.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wk.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://la.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://ob.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://la.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pk.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ak.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://ds.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zv.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://mv.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xk.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ob.asd995.cn

Java: // 手写递归
来源：http://gs.colortex.cn

Go:   // 手写递归
来源：http://kq.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rs.haigaiapp.cn

C#:   // 手写递归
来源：http://xx.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gr.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ts.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nu.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qo.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xz.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oa.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nu.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://po.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ch.huixinmuqiang.cn

================================================================================
来源：http://uc.haigaiapp.cn

O. 并发与异步
来源：http://ue.colortex.cn

================================================================================
来源：http://yw.colortex.cn

[O01] 启动一个线程
来源：http://su.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sk.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aq.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://es.panjiajie.cn

TS:   // 同 JS
来源：http://km.521024.cn

Java: new Thread(() -> f()).start()
来源：http://bs.muxihuayi.cn

Go:   go f()
来源：http://mn.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://qm.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://nz.lnxyls.cn

[O02] 使用线程池
来源：http://qc.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gc.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fq.hahajie.cn

JS:   // worker_threads 线程池
来源：http://dc.colortex.cn

TS:   // worker_threads 线程池
来源：http://di.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iq.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ek.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gu.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kh.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://wx.521024.cn

Py:   with lock: shared += 1
来源：http://uo.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://iw.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wi.nicolike.cn

TS:   // 同 JS
来源：http://st.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://px.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ex.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zx.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://nw.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://lu.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://vr.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pb.hahajie.cn

JS:   async function f() { await g(); }
来源：http://wh.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://be.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sy.wgjwhj.cn


<!-- 参考信息 -->