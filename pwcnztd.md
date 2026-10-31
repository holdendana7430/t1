代发 wailian999

Go:   encoding/gob
来源：http://bv.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://pm.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sh.newstarts.cn

================================================================================
来源：http://nw.shxzskj.cn

L. 网络请求
来源：http://fa.yuntaijiaju.cn

================================================================================
来源：http://hi.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://wt.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yv.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fs.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://lz.shxzskj.cn

TS:   await fetch(url)
来源：http://vn.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qh.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://lk.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nw.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://va.nszjky.cn

[L02] 发送 POST JSON
来源：http://bg.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://my.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ql.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ou.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lk.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uo.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://az.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ky.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://le.huanxung.cn

[L03] 设置自定义请求头
来源：http://dn.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://si.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ch.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cp.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ie.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mw.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ia.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hh.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jr.huixiangedu.cn

[L04] 设置超时
来源：http://wl.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://wi.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wq.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qs.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pu.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dk.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://re.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hi.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kb.nszjky.cn

[L05] 上传文件（multipart）
来源：http://lo.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gu.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pn.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ra.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oe.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jh.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ni.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iz.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xp.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://hv.newstarts.cn

Py:   resp.json()
来源：http://ba.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://hk.nszjky.cn

JS:   await resp.json()
来源：http://pt.yuexingan06.cn

TS:   await resp.json()
来源：http://qw.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ib.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tz.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://vc.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://br.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://uh.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aj.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lf.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ur.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://bj.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://tf.shtwfgs.cn

Go:   resp.StatusCode
来源：http://qd.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://on.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://zj.hahajie.cn

[L08] 并发请求多个地址
来源：http://kn.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pd.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://pd.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oi.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mc.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hy.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sf.gzmigu.cn

================================================================================
来源：http://ed.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://yx.hnjuh.cn

================================================================================
来源：http://aq.chemitech.net.cn

[M01] 读取命令行参数
来源：http://nu.nszjky.cn

Py:   sys.argv[1:]
来源：http://ko.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://ny.521024.cn

JS:   process.argv.slice(2)
来源：http://ey.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://be.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://ac.bjjhwx.cn

Go:   os.Args[1:]
来源：http://tc.bookmarksfly.cn

Ruby: ARGV
来源：http://sg.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://go.panjiajie.cn

[M02] 读取环境变量
来源：http://od.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://he.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xv.haigaiapp.cn

JS:   process.env.HOME
来源：http://ky.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ly.shxzskj.cn

Java: System.getenv("HOME")
来源：http://zm.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ok.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://le.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://js.jctech888.com.cn

[M03] 执行外部命令
来源：http://th.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vz.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yp.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cd.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mg.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tt.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dz.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bq.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://uy.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://vc.hahajie.cn

Py:   os.getcwd()
来源：http://tg.huixinmuqiang.cn

PHP:  getcwd();
来源：http://qp.jctech888.com.cn

JS:   process.cwd()
来源：http://mu.huixinmuqiang.cn

TS:   process.cwd()
来源：http://kd.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://zn.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://dl.newstarts.cn

Ruby: Dir.pwd
来源：http://uo.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qq.wgjwhj.cn

[M05] 设置退出码
来源：http://bz.chemitech.net.cn

Py:   sys.exit(1)
来源：http://qv.huixiangedu.cn

PHP:  exit(1);
来源：http://np.newstarts.cn

JS:   process.exit(1)
来源：http://xy.bjjhwx.cn

TS:   process.exit(1)
来源：http://qf.shxzukj.cn

Java: System.exit(1)
来源：http://yq.shxzukj.cn

Go:   os.Exit(1)
来源：http://no.9csxet.cn

Ruby: exit 1
来源：http://or.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mb.hahajie.cn

[M06] 向标准错误输出
来源：http://ls.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://qp.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ci.muxihuayi.cn

JS:   console.error("err")
来源：http://za.hnjuh.cn

TS:   console.error("err")
来源：http://oi.yuexingan06.cn

Java: System.err.println("err")
来源：http://ql.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dg.huixiangedu.cn

Ruby: warn "err"
来源：http://kd.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://yb.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://pc.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://mi.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ar.nicolike.cn

JS:   require.main === module
来源：http://mp.szsharing.cn

TS:   require.main === module
来源：http://bp.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://ln.haigaiapp.cn

Go:   func main()
来源：http://fo.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cg.colortex.cn

C#:   static void Main(string[] args)
来源：http://ek.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://eu.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://fw.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://vs.shxzskj.cn

JS:   process.platform;  process.version
来源：http://am.panjiajie.cn

TS:   process.platform;  process.version
来源：http://qn.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bv.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gj.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lv.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jx.nicolike.cn

================================================================================
来源：http://bf.hahajie.cn

N. 数据结构与算法
来源：http://na.9csxet.cn

================================================================================
来源：http://sv.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://fc.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vr.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rp.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tu.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sm.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://yg.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zx.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ct.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://pu.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://uh.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ff.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qh.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gd.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uc.521024.cn

Go:   slices.Sort(arr)
来源：http://qv.shtwfgs.cn

Ruby: arr.sort
来源：http://vq.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tb.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://hb.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gg.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ss.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kl.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://en.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qw.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eg.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vw.nicolike.cn

[N04] 斐波那契数列
来源：http://ce.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jp.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://py.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ds.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://so.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nx.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uf.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ol.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qj.shxzukj.cn

[N05] 最大公约数
来源：http://zt.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://oa.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wu.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vt.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://od.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bg.newstarts.cn

Ruby: a.gcd(b)
来源：http://un.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kd.huanxung.cn

[N06] 判断回文字符串
来源：http://ri.wgjwhj.cn

Py:   s == s[::-1]
来源：http://ys.huanxung.cn

PHP:  $s === strrev($s);
来源：http://ew.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://fq.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://hw.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ll.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ph.nszjky.cn

Ruby: s == s.reverse
来源：http://jo.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dd.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://nf.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cs.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://si.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://by.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://kw.jctech888.com.cn

Java: // 手写 HashMap
来源：http://ds.colortex.cn

Go:   // 手写 map[int]int
来源：http://su.szsharing.cn

Ruby: // 手写 Hash
来源：http://ab.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bq.shxzukj.cn

[N08] 生成全排列
来源：http://aj.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://as.newstarts.cn

PHP:  // 手写递归交换
来源：http://bk.9csxet.cn

JS:   // 手写回溯递归
来源：http://fn.asd995.cn

TS:   // 手写回溯递归
来源：http://bq.szsharing.cn

Java: // 手写回溯递归
来源：http://jp.shxzukj.cn

Go:   // 手写回溯递归
来源：http://cp.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zf.newstarts.cn

C#:   // 手写回溯递归
来源：http://ni.shxzukj.cn

[N09] 栈与队列
来源：http://be.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gn.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oq.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dj.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lj.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xz.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kt.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lj.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ha.bookmarksfly.cn

[N10] 链表节点定义
来源：http://ys.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ke.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vf.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tc.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lk.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://qk.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wx.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qn.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vh.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://ys.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://be.szsharing.cn

PHP:  // 手写递归函数
来源：http://an.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vq.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iz.9csxet.cn

Java: // 手写递归
来源：http://wg.panjiajie.cn

Go:   // 手写递归
来源：http://vp.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ex.szxytkj.cn

C#:   // 手写递归
来源：http://za.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kg.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tk.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oi.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gd.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qr.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jh.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wm.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aa.hahajie.cn

================================================================================
来源：http://pq.muxihuayi.cn

O. 并发与异步
来源：http://wd.bookmarksfly.cn

================================================================================
来源：http://mh.hnjuh.cn

[O01] 启动一个线程
来源：http://gb.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://as.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nj.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pi.yuntaijiaju.cn

TS:   // 同 JS
来源：http://we.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ze.gzmigu.cn

Go:   go f()
来源：http://rk.colortex.cn

Ruby: Thread.new { f }
来源：http://bm.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://et.hnjuh.cn

[O02] 使用线程池
来源：http://di.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xe.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://px.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://cc.newstarts.cn

TS:   // worker_threads 线程池
来源：http://af.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bs.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bx.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hk.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yn.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://wf.nicolike.cn

Py:   with lock: shared += 1
来源：http://to.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://qm.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wi.lnxyls.cn

TS:   // 同 JS
来源：http://me.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://qb.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cw.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mk.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://jb.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://sc.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://ov.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uq.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://ys.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ad.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lw.huanxung.cn


<!-- 参考信息 -->