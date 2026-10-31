代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://wy.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://bi.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://jt.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qu.lnxyls.cn

Go:   encoding/gob
来源：http://lf.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://gu.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pw.hahajie.cn

================================================================================
来源：http://dr.szxytkj.cn

L. 网络请求
来源：http://fv.shtwfgs.cn

================================================================================
来源：http://wm.shxzskj.cn

[L01] 发送 GET 请求
来源：http://za.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hs.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ui.nszjky.cn

JS:   await fetch(url)
来源：http://rw.lnxyls.cn

TS:   await fetch(url)
来源：http://cy.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lf.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://sc.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gj.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yu.colortex.cn

[L02] 发送 POST JSON
来源：http://ap.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uf.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hl.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ve.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fx.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gg.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://be.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fv.colortex.cn

[L03] 设置自定义请求头
来源：http://sm.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qk.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qk.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wm.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nb.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zg.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wj.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qq.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://it.yuntaijiaju.cn

[L04] 设置超时
来源：http://do.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://db.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zj.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xn.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tg.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xp.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ql.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yn.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nh.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://lw.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://np.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zd.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zd.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vw.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jt.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xs.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qj.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rc.szsharing.cn

[L06] 解析响应为 JSON
来源：http://kt.shxzskj.cn

Py:   resp.json()
来源：http://ma.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://vr.huanxung.cn

JS:   await resp.json()
来源：http://xn.gzmigu.cn

TS:   await resp.json()
来源：http://qj.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://og.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ra.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://pp.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oh.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://lh.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bu.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iu.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://zs.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://dg.szxytkj.cn

Java: resp.statusCode()
来源：http://zd.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://qa.szsharing.cn

Ruby: resp.code.to_i
来源：http://zu.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://vt.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://zd.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ut.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://hp.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fq.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ft.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://na.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mp.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pi.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lv.jianghongdianzi.cn

================================================================================
来源：http://uj.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ri.huanxung.cn

================================================================================
来源：http://yg.muxihuayi.cn

[M01] 读取命令行参数
来源：http://aj.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://fq.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ak.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://nf.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://nc.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://vq.nszjky.cn

Go:   os.Args[1:]
来源：http://jc.bjjhwx.cn

Ruby: ARGV
来源：http://yc.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://sm.bjjhwx.cn

[M02] 读取环境变量
来源：http://rb.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://si.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xq.yuexingan06.cn

JS:   process.env.HOME
来源：http://ln.chemitech.net.cn

TS:   process.env.HOME
来源：http://oq.szsharing.cn

Java: System.getenv("HOME")
来源：http://sl.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://of.colortex.cn

Ruby: ENV["HOME"]
来源：http://ke.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vd.bjjhwx.cn

[M03] 执行外部命令
来源：http://xg.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sp.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sj.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://db.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yu.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qq.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sv.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pz.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://zs.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://uj.panjiajie.cn

Py:   os.getcwd()
来源：http://ev.jctech888.com.cn

PHP:  getcwd();
来源：http://ax.bjjhwx.cn

JS:   process.cwd()
来源：http://xr.hnjuh.cn

TS:   process.cwd()
来源：http://ze.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://jw.shtwfgs.cn

Go:   os.Getwd()
来源：http://zq.huixiangedu.cn

Ruby: Dir.pwd
来源：http://mh.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bs.newstarts.cn

[M05] 设置退出码
来源：http://xp.wgjwhj.cn

Py:   sys.exit(1)
来源：http://xk.huixinmuqiang.cn

PHP:  exit(1);
来源：http://on.nicolike.cn

JS:   process.exit(1)
来源：http://qk.nicolike.cn

TS:   process.exit(1)
来源：http://sq.haigaiapp.cn

Java: System.exit(1)
来源：http://vx.shxzukj.cn

Go:   os.Exit(1)
来源：http://rl.chemitech.net.cn

Ruby: exit 1
来源：http://da.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ah.panjiajie.cn

[M06] 向标准错误输出
来源：http://hi.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://ib.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pi.bjjhwx.cn

JS:   console.error("err")
来源：http://tq.shxzukj.cn

TS:   console.error("err")
来源：http://cv.hahajie.cn

Java: System.err.println("err")
来源：http://vw.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://si.gzmigu.cn

Ruby: warn "err"
来源：http://ts.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://wz.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://ir.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://kq.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bl.colortex.cn

JS:   require.main === module
来源：http://je.lnxyls.cn

TS:   require.main === module
来源：http://sz.huanxung.cn

Java: public static void main(String[] args)
来源：http://mp.shxzukj.cn

Go:   func main()
来源：http://nx.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dy.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://ln.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://jo.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://bu.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://eu.lnxyls.cn

JS:   process.platform;  process.version
来源：http://eb.nicolike.cn

TS:   process.platform;  process.version
来源：http://gr.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hf.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bi.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yq.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rw.asd995.cn

================================================================================
来源：http://mt.yuexingan06.cn

N. 数据结构与算法
来源：http://vh.shxzskj.cn

================================================================================
来源：http://xv.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://tm.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kj.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://my.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oc.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wi.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ku.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://nr.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uo.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ng.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://ms.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://sd.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://df.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pc.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yd.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://to.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://gp.panjiajie.cn

Ruby: arr.sort
来源：http://wh.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tq.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://lu.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ro.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ap.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dy.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yk.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ng.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wv.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ii.muxihuayi.cn

[N04] 斐波那契数列
来源：http://fh.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fd.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hh.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ge.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hg.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rq.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zo.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oe.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qc.wgjwhj.cn

[N05] 最大公约数
来源：http://is.huanxung.cn

Py:   math.gcd(a, b)
来源：http://cp.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jm.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wo.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ka.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ja.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fe.nszjky.cn

Ruby: a.gcd(b)
来源：http://vd.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lb.gzmigu.cn

[N06] 判断回文字符串
来源：http://tl.nicolike.cn

Py:   s == s[::-1]
来源：http://ir.asd995.cn

PHP:  $s === strrev($s);
来源：http://js.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://xp.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://dh.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mr.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://og.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ve.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://os.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://gi.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ac.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vy.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fl.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://zy.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://kr.hahajie.cn

Go:   // 手写 map[int]int
来源：http://pr.shxzukj.cn

Ruby: // 手写 Hash
来源：http://px.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hy.shxzukj.cn

[N08] 生成全排列
来源：http://gy.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://bn.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://xr.nicolike.cn

JS:   // 手写回溯递归
来源：http://ss.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://zk.panjiajie.cn

Java: // 手写回溯递归
来源：http://cv.colortex.cn

Go:   // 手写回溯递归
来源：http://cm.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://pk.nicolike.cn

C#:   // 手写回溯递归
来源：http://aq.yuntaijiaju.cn

[N09] 栈与队列
来源：http://ft.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oq.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sa.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hf.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kj.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xt.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gp.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wg.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://th.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ah.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pg.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yw.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nj.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ta.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hb.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sc.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qz.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://jl.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xw.szxytkj.cn

PHP:  // 手写递归函数
来源：http://ts.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ld.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ti.yuexingan06.cn

Java: // 手写递归
来源：http://zg.jctech888.com.cn

Go:   // 手写递归
来源：http://js.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://so.colortex.cn

C#:   // 手写递归
来源：http://ly.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ew.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ci.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pu.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nt.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oq.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mi.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dj.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ng.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ng.szxytkj.cn

================================================================================
来源：http://lz.yuntaijiaju.cn

O. 并发与异步
来源：http://cn.hnjuh.cn

================================================================================
来源：http://yp.bjjhwx.cn

[O01] 启动一个线程
来源：http://xn.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cs.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pw.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lr.hnjuh.cn

TS:   // 同 JS
来源：http://ku.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://gg.muxihuayi.cn

Go:   go f()
来源：http://hc.newstarts.cn

Ruby: Thread.new { f }
来源：http://hu.hahajie.cn

C#:   Task.Run(() => F());
来源：http://xi.huixiangedu.cn

[O02] 使用线程池
来源：http://rh.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iv.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fk.asd995.cn

JS:   // worker_threads 线程池
来源：http://xz.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://qy.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zq.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jk.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kr.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sm.asd995.cn

[O03] 加锁保护共享数据
来源：http://xp.colortex.cn

Py:   with lock: shared += 1
来源：http://ne.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ix.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cu.asd995.cn

TS:   // 同 JS
来源：http://yy.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://vn.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ae.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wn.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://dk.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://pq.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://nf.9csxet.cn


<!-- 参考信息 -->