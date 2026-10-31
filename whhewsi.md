代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://vs.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://zl.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://lk.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ss.nicolike.cn

Go:   encoding/gob
来源：http://qj.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://ji.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uq.wgjwhj.cn

================================================================================
来源：http://uw.newstarts.cn

L. 网络请求
来源：http://xw.huixinmuqiang.cn

================================================================================
来源：http://od.newstarts.cn

[L01] 发送 GET 请求
来源：http://se.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zs.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uh.wgjwhj.cn

JS:   await fetch(url)
来源：http://bs.nszjky.cn

TS:   await fetch(url)
来源：http://bb.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fy.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ej.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xr.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://so.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://kp.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fl.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yb.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sp.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yl.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rq.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vo.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://qo.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uo.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ih.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ve.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ux.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nd.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ao.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bh.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qv.gzmigu.cn

[L04] 设置超时
来源：http://zz.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://wd.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://go.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wm.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://js.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://me.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yw.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qs.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://wp.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mk.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://et.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ri.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://re.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://re.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kl.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dd.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ac.huixinmuqiang.cn

Py:   resp.json()
来源：http://pj.9csxet.cn

PHP:  json_decode($body, true);
来源：http://ye.gzmigu.cn

JS:   await resp.json()
来源：http://ks.shxzukj.cn

TS:   await resp.json()
来源：http://tq.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vt.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ro.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://rm.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bi.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://jv.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://be.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yc.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://ld.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://hy.yuexingan06.cn

Java: resp.statusCode()
来源：http://at.szxytkj.cn

Go:   resp.StatusCode
来源：http://wk.hnjuh.cn

Ruby: resp.code.to_i
来源：http://pt.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://aq.shxzskj.cn

[L08] 并发请求多个地址
来源：http://ty.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ok.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://wk.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://er.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fc.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nv.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pl.muxihuayi.cn

================================================================================
来源：http://fz.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://nx.huixiangedu.cn

================================================================================
来源：http://jj.huanxung.cn

[M01] 读取命令行参数
来源：http://mp.nszjky.cn

Py:   sys.argv[1:]
来源：http://nz.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://sw.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://xl.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://wl.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://nh.haigaiapp.cn

Go:   os.Args[1:]
来源：http://nb.panjiajie.cn

Ruby: ARGV
来源：http://nl.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://ku.hnjuh.cn

[M02] 读取环境变量
来源：http://hn.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://xh.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cr.lnxyls.cn

JS:   process.env.HOME
来源：http://yj.shtwfgs.cn

TS:   process.env.HOME
来源：http://uu.lnxyls.cn

Java: System.getenv("HOME")
来源：http://pk.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ls.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://zq.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://in.hnjuh.cn

[M03] 执行外部命令
来源：http://di.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ht.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ta.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rf.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eu.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gg.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vy.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mu.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://kl.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://kj.panjiajie.cn

Py:   os.getcwd()
来源：http://cz.shxzukj.cn

PHP:  getcwd();
来源：http://ou.huanxung.cn

JS:   process.cwd()
来源：http://ku.hnjuh.cn

TS:   process.cwd()
来源：http://gc.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://fw.muxihuayi.cn

Go:   os.Getwd()
来源：http://xd.shxzskj.cn

Ruby: Dir.pwd
来源：http://xi.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jp.hnjuh.cn

[M05] 设置退出码
来源：http://iq.yuexingan06.cn

Py:   sys.exit(1)
来源：http://mc.newstarts.cn

PHP:  exit(1);
来源：http://wy.nicolike.cn

JS:   process.exit(1)
来源：http://fp.9csxet.cn

TS:   process.exit(1)
来源：http://vf.bjjhwx.cn

Java: System.exit(1)
来源：http://ea.shxzskj.cn

Go:   os.Exit(1)
来源：http://rc.huixiangedu.cn

Ruby: exit 1
来源：http://oi.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xg.huixiangedu.cn

[M06] 向标准错误输出
来源：http://dg.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://pa.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ls.shtwfgs.cn

JS:   console.error("err")
来源：http://sh.shxzskj.cn

TS:   console.error("err")
来源：http://qr.szsharing.cn

Java: System.err.println("err")
来源：http://ju.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ej.asd995.cn

Ruby: warn "err"
来源：http://se.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://vm.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://sf.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://ub.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bx.bookmarksfly.cn

JS:   require.main === module
来源：http://hv.asd995.cn

TS:   require.main === module
来源：http://xk.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://eg.hnjuh.cn

Go:   func main()
来源：http://ry.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uw.huanxung.cn

C#:   static void Main(string[] args)
来源：http://vr.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://nj.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://le.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://ej.huanxung.cn

JS:   process.platform;  process.version
来源：http://nl.521024.cn

TS:   process.platform;  process.version
来源：http://qd.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ea.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ms.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://va.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dg.shtwfgs.cn

================================================================================
来源：http://cs.shtwfgs.cn

N. 数据结构与算法
来源：http://za.asd995.cn

================================================================================
来源：http://cl.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://zt.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tk.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lh.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wv.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zn.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cr.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://ki.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oa.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wx.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://bp.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ks.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uu.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fz.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ru.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yv.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ke.nicolike.cn

Ruby: arr.sort
来源：http://rn.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xd.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://eb.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ge.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://nx.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gj.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://np.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kt.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vh.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://un.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cz.yuexingan06.cn

[N04] 斐波那契数列
来源：http://vx.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uh.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aj.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://so.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://me.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ub.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gg.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xf.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uj.bjjhwx.cn

[N05] 最大公约数
来源：http://oc.hahajie.cn

Py:   math.gcd(a, b)
来源：http://mi.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oi.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://za.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gt.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ly.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://na.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://wf.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ie.nicolike.cn

[N06] 判断回文字符串
来源：http://qt.nszjky.cn

Py:   s == s[::-1]
来源：http://np.szsharing.cn

PHP:  $s === strrev($s);
来源：http://dq.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://nv.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://xh.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uz.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://vs.colortex.cn

Ruby: s == s.reverse
来源：http://ak.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://et.asd995.cn

[N07] 两数之和（返回下标）
来源：http://fx.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ze.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iz.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cx.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://my.wgjwhj.cn

Java: // 手写 HashMap
来源：http://jp.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://qz.nicolike.cn

Ruby: // 手写 Hash
来源：http://nc.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hj.haigaiapp.cn

[N08] 生成全排列
来源：http://rd.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://lm.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://oa.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ol.panjiajie.cn

TS:   // 手写回溯递归
来源：http://jw.panjiajie.cn

Java: // 手写回溯递归
来源：http://bl.panjiajie.cn

Go:   // 手写回溯递归
来源：http://au.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://fb.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://en.shxzukj.cn

[N09] 栈与队列
来源：http://hq.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sf.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cy.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gx.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zu.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zx.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://si.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fi.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ey.shxzukj.cn

[N10] 链表节点定义
来源：http://bz.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://um.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://et.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pn.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ww.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://iu.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gt.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hp.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vn.nszjky.cn

[N11] 二叉树中序遍历
来源：http://cb.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rj.521024.cn

PHP:  // 手写递归函数
来源：http://ah.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://st.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ay.colortex.cn

Java: // 手写递归
来源：http://wa.nszjky.cn

Go:   // 手写递归
来源：http://tr.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pn.panjiajie.cn

C#:   // 手写递归
来源：http://hy.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fm.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mu.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lk.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bi.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wn.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dv.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lt.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rf.bjjhwx.cn

================================================================================
来源：http://wp.muxihuayi.cn

O. 并发与异步
来源：http://ap.newstarts.cn

================================================================================
来源：http://xc.huanxung.cn

[O01] 启动一个线程
来源：http://fc.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pt.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vh.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xa.hahajie.cn

TS:   // 同 JS
来源：http://sa.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://dw.bjjhwx.cn

Go:   go f()
来源：http://up.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://qy.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://jr.nszjky.cn

[O02] 使用线程池
来源：http://fr.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rp.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ph.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://fr.nszjky.cn

TS:   // worker_threads 线程池
来源：http://ho.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qe.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ts.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://if.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fe.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://wg.asd995.cn

Py:   with lock: shared += 1
来源：http://jn.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://wk.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wd.panjiajie.cn

TS:   // 同 JS
来源：http://gd.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://de.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hc.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ru.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://cs.colortex.cn

[O04] 定义异步函数并等待
来源：http://ls.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://hy.szxytkj.cn


<!-- 参考信息 -->