代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xs.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qg.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xk.shxzukj.cn

[K05] 深拷贝对象
来源：http://xi.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://jf.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://yi.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://bi.shxzskj.cn

TS:   structuredClone(obj)
来源：http://ko.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oi.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qs.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tg.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ad.huanxung.cn

[K06] 解析 URL 查询串
来源：http://cd.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hb.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fy.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://is.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://os.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gl.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jz.nicolike.cn

[K07] 进制转换
来源：http://os.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ff.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cg.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://td.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://id.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yu.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ia.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ux.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bu.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wp.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://eg.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vh.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://fq.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://vf.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hx.bjjhwx.cn

Go:   encoding/gob
来源：http://gd.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://ju.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://va.colortex.cn

================================================================================
来源：http://bf.9csxet.cn

L. 网络请求
来源：http://vk.yuntaijiaju.cn

================================================================================
来源：http://mg.shxzskj.cn

[L01] 发送 GET 请求
来源：http://sr.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://du.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yb.muxihuayi.cn

JS:   await fetch(url)
来源：http://ir.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://og.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oi.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://rg.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ga.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bd.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://qu.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bj.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ua.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://as.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hy.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pn.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pv.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zb.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zb.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://kz.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kj.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://km.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nb.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bw.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tv.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jx.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cm.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wc.haigaiapp.cn

[L04] 设置超时
来源：http://cq.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://bh.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://he.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gm.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kl.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kj.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kl.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://av.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hk.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://zc.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rf.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lb.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jc.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wz.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cc.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tp.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://in.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tr.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://sk.asd995.cn

Py:   resp.json()
来源：http://js.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://dl.9csxet.cn

JS:   await resp.json()
来源：http://gm.newstarts.cn

TS:   await resp.json()
来源：http://xp.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xt.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ee.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://xp.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hk.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://db.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://om.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://ba.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://ql.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://nt.lnxyls.cn

Go:   resp.StatusCode
来源：http://nq.szxytkj.cn

Ruby: resp.code.to_i
来源：http://ze.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://zu.521024.cn

[L08] 并发请求多个地址
来源：http://mw.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nl.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://zl.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://od.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vz.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vv.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ef.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://as.shtwfgs.cn

================================================================================
来源：http://so.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://do.huanxung.cn

================================================================================
来源：http://uf.bjjhwx.cn

[M01] 读取命令行参数
来源：http://uz.nicolike.cn

Py:   sys.argv[1:]
来源：http://wj.nszjky.cn

PHP:  $argv;  $argc;
来源：http://cy.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://kh.9csxet.cn

TS:   process.argv.slice(2)
来源：http://eb.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ja.shtwfgs.cn

Go:   os.Args[1:]
来源：http://zx.521024.cn

Ruby: ARGV
来源：http://ur.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://aw.9csxet.cn

[M02] 读取环境变量
来源：http://gj.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://xk.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oq.gzmigu.cn

JS:   process.env.HOME
来源：http://un.wgjwhj.cn

TS:   process.env.HOME
来源：http://gv.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://qv.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://en.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://pf.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ah.asd995.cn

[M03] 执行外部命令
来源：http://rp.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://de.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qt.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cx.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ks.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lr.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pr.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jj.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://st.hahajie.cn

[M04] 获取当前工作目录
来源：http://ve.bjjhwx.cn

Py:   os.getcwd()
来源：http://xj.szxytkj.cn

PHP:  getcwd();
来源：http://jp.gzmigu.cn

JS:   process.cwd()
来源：http://kl.wgjwhj.cn

TS:   process.cwd()
来源：http://ko.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://pr.nszjky.cn

Go:   os.Getwd()
来源：http://yc.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://pi.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pf.bookmarksfly.cn

[M05] 设置退出码
来源：http://eg.chemitech.net.cn

Py:   sys.exit(1)
来源：http://wq.szsharing.cn

PHP:  exit(1);
来源：http://nl.hnjuh.cn

JS:   process.exit(1)
来源：http://ta.nicolike.cn

TS:   process.exit(1)
来源：http://xm.nszjky.cn

Java: System.exit(1)
来源：http://vy.szsharing.cn

Go:   os.Exit(1)
来源：http://br.bookmarksfly.cn

Ruby: exit 1
来源：http://en.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://av.wgjwhj.cn

[M06] 向标准错误输出
来源：http://wf.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://hs.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lo.szsharing.cn

JS:   console.error("err")
来源：http://py.bjjhwx.cn

TS:   console.error("err")
来源：http://om.chemitech.net.cn

Java: System.err.println("err")
来源：http://zj.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jn.lnxyls.cn

Ruby: warn "err"
来源：http://fl.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://wx.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://zs.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://jl.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mo.jctech888.com.cn

JS:   require.main === module
来源：http://iy.521024.cn

TS:   require.main === module
来源：http://uf.shxzukj.cn

Java: public static void main(String[] args)
来源：http://dz.jianghongdianzi.cn

Go:   func main()
来源：http://zt.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kp.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://co.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://sb.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://gm.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://zs.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://br.hnjuh.cn

TS:   process.platform;  process.version
来源：http://yu.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aa.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eg.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://as.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ej.huixiangedu.cn

================================================================================
来源：http://ge.bookmarksfly.cn

N. 数据结构与算法
来源：http://ob.panjiajie.cn

================================================================================
来源：http://yv.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://pd.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qz.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zh.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fj.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jq.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tn.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://tm.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cc.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zm.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://wz.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ot.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ml.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vc.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nx.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ht.szsharing.cn

Go:   slices.Sort(arr)
来源：http://vx.huixinmuqiang.cn

Ruby: arr.sort
来源：http://bm.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://is.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://cj.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wr.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://up.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fx.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://km.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gq.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ps.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dl.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ag.muxihuayi.cn

[N04] 斐波那契数列
来源：http://yg.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ac.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://or.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://co.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vp.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tz.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mf.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://li.newstarts.cn

[N05] 最大公约数
来源：http://vs.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://sc.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ul.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oy.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yo.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gt.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wp.lnxyls.cn

Ruby: a.gcd(b)
来源：http://kl.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ir.shxzukj.cn

[N06] 判断回文字符串
来源：http://um.hahajie.cn

Py:   s == s[::-1]
来源：http://ec.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://uu.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://jy.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://ha.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ju.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://xo.gzmigu.cn

Ruby: s == s.reverse
来源：http://fu.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zb.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ps.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hc.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rs.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://io.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ld.shxzukj.cn

Java: // 手写 HashMap
来源：http://np.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://bh.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://uk.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ab.bjjhwx.cn

[N08] 生成全排列
来源：http://dr.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://wm.shxzukj.cn

PHP:  // 手写递归交换
来源：http://zv.colortex.cn

JS:   // 手写回溯递归
来源：http://fh.521024.cn

TS:   // 手写回溯递归
来源：http://wt.lnxyls.cn

Java: // 手写回溯递归
来源：http://gb.521024.cn

Go:   // 手写回溯递归
来源：http://fv.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://yl.panjiajie.cn

C#:   // 手写回溯递归
来源：http://do.hahajie.cn

[N09] 栈与队列
来源：http://et.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qz.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://az.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pj.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bk.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nv.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://js.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ms.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xt.haigaiapp.cn

[N10] 链表节点定义
来源：http://fr.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yj.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sm.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vq.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jr.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://pm.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ih.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xr.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tb.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://mw.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://as.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://du.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yb.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://su.nszjky.cn

Java: // 手写递归
来源：http://gk.panjiajie.cn

Go:   // 手写递归
来源：http://mp.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zl.bookmarksfly.cn

C#:   // 手写递归
来源：http://xm.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vu.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ld.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cm.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ff.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ol.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bb.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eo.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ti.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ig.haigaiapp.cn


<!-- 参考信息 -->