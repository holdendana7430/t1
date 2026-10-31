代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://od.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uo.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ie.colortex.cn

[K05] 深拷贝对象
来源：http://pp.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://pc.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://gc.panjiajie.cn

JS:   structuredClone(obj)
来源：http://sv.huanxung.cn

TS:   structuredClone(obj)
来源：http://cb.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hu.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ky.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lw.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gx.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://he.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qi.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jc.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ik.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qr.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gk.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tb.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://je.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eu.hahajie.cn

[K07] 进制转换
来源：http://lj.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qr.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gu.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zs.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xh.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cm.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bk.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://px.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wg.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://mf.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://se.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nc.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://sr.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://ch.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xq.yuntaijiaju.cn

Go:   encoding/gob
来源：http://fp.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://yb.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bk.yuntaijiaju.cn

================================================================================
来源：http://fg.521024.cn

L. 网络请求
来源：http://bn.gzmigu.cn

================================================================================
来源：http://xs.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://vz.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zi.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vn.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://md.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ul.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ul.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://vx.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nk.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xi.asd995.cn

[L02] 发送 POST JSON
来源：http://eq.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ye.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kd.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rx.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gb.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ug.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://js.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ko.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sz.521024.cn

[L03] 设置自定义请求头
来源：http://gu.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xo.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ty.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pc.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ij.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kh.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hd.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kl.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ai.nszjky.cn

[L04] 设置超时
来源：http://iv.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://wj.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ns.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ap.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cb.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ae.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ud.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zz.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dr.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://hl.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mk.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ep.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ls.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gl.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zv.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ls.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ex.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://op.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://qm.yuexingan06.cn

Py:   resp.json()
来源：http://pv.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ih.wgjwhj.cn

JS:   await resp.json()
来源：http://gt.haigaiapp.cn

TS:   await resp.json()
来源：http://yo.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ng.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://my.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://lv.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wo.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://yv.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jh.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yh.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ac.asd995.cn

TS:   resp.ok;  resp.status
来源：http://yi.huanxung.cn

Java: resp.statusCode()
来源：http://us.huanxung.cn

Go:   resp.StatusCode
来源：http://bz.huanxung.cn

Ruby: resp.code.to_i
来源：http://br.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ls.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://sm.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ao.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://jx.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fx.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://if.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://or.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pf.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tu.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nw.9csxet.cn

================================================================================
来源：http://fy.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://vp.bookmarksfly.cn

================================================================================
来源：http://ox.gzmigu.cn

[M01] 读取命令行参数
来源：http://ls.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ga.szsharing.cn

PHP:  $argv;  $argc;
来源：http://or.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://ta.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://uy.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://wd.bjjhwx.cn

Go:   os.Args[1:]
来源：http://xw.shxzskj.cn

Ruby: ARGV
来源：http://zw.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://uk.521024.cn

[M02] 读取环境变量
来源：http://xh.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://qn.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://de.newstarts.cn

JS:   process.env.HOME
来源：http://wt.gzmigu.cn

TS:   process.env.HOME
来源：http://nf.nszjky.cn

Java: System.getenv("HOME")
来源：http://cp.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yy.nszjky.cn

Ruby: ENV["HOME"]
来源：http://ga.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yi.gzmigu.cn

[M03] 执行外部命令
来源：http://fg.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sa.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pe.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yl.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hq.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xq.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tz.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yp.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://bg.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://fk.lnxyls.cn

Py:   os.getcwd()
来源：http://on.newstarts.cn

PHP:  getcwd();
来源：http://bh.bookmarksfly.cn

JS:   process.cwd()
来源：http://sp.huanxung.cn

TS:   process.cwd()
来源：http://sb.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://wb.nicolike.cn

Go:   os.Getwd()
来源：http://am.asd995.cn

Ruby: Dir.pwd
来源：http://oa.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sd.jctech888.com.cn

[M05] 设置退出码
来源：http://ap.hnjuh.cn

Py:   sys.exit(1)
来源：http://jr.szsharing.cn

PHP:  exit(1);
来源：http://bf.szsharing.cn

JS:   process.exit(1)
来源：http://gw.chemitech.net.cn

TS:   process.exit(1)
来源：http://gu.huanxung.cn

Java: System.exit(1)
来源：http://ed.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://rs.asd995.cn

Ruby: exit 1
来源：http://sm.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hp.shtwfgs.cn

[M06] 向标准错误输出
来源：http://nn.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://zl.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pv.nicolike.cn

JS:   console.error("err")
来源：http://kx.hahajie.cn

TS:   console.error("err")
来源：http://hs.jctech888.com.cn

Java: System.err.println("err")
来源：http://jv.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bk.521024.cn

Ruby: warn "err"
来源：http://en.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://os.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://yv.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://yo.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ma.bookmarksfly.cn

JS:   require.main === module
来源：http://bo.wgjwhj.cn

TS:   require.main === module
来源：http://nt.colortex.cn

Java: public static void main(String[] args)
来源：http://hh.haigaiapp.cn

Go:   func main()
来源：http://rq.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gk.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ib.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://mh.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://ny.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://js.asd995.cn

JS:   process.platform;  process.version
来源：http://sp.shxzskj.cn

TS:   process.platform;  process.version
来源：http://kk.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zc.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cq.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uw.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://kw.chemitech.net.cn

N. 数据结构与算法
来源：http://pg.bjjhwx.cn

================================================================================
来源：http://ed.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://eg.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ay.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yx.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://to.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zi.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yr.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://cq.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rl.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qy.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://yv.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ib.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gz.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hv.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yz.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://or.jctech888.com.cn

Ruby: arr.sort
来源：http://qt.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://en.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://hc.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://na.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://fi.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oi.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qu.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pb.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vf.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fp.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gr.chemitech.net.cn

[N04] 斐波那契数列
来源：http://vy.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gs.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bj.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bh.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zz.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zt.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vv.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jf.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fa.asd995.cn

[N05] 最大公约数
来源：http://lx.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://kw.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ww.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ng.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ky.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bo.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://to.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xl.shtwfgs.cn

[N06] 判断回文字符串
来源：http://hn.hahajie.cn

Py:   s == s[::-1]
来源：http://kj.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://tk.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://wy.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://zs.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://px.521024.cn

Go:   // 双指针从两端比较
来源：http://cz.huixiangedu.cn

Ruby: s == s.reverse
来源：http://fy.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wx.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://lv.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kn.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hb.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ul.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://xs.szxytkj.cn

Java: // 手写 HashMap
来源：http://hn.huanxung.cn

Go:   // 手写 map[int]int
来源：http://zy.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ig.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qm.521024.cn

[N08] 生成全排列
来源：http://xi.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://kn.shxzukj.cn

PHP:  // 手写递归交换
来源：http://qh.szsharing.cn

JS:   // 手写回溯递归
来源：http://zh.gzmigu.cn

TS:   // 手写回溯递归
来源：http://ma.shtwfgs.cn

Java: // 手写回溯递归
来源：http://hk.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://gy.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://fd.521024.cn

C#:   // 手写回溯递归
来源：http://al.jctech888.com.cn

[N09] 栈与队列
来源：http://eh.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mj.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aq.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cx.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://id.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lf.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sq.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sf.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://su.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://sy.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zr.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hr.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ia.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zl.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://xy.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wz.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sq.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gk.hahajie.cn

[N11] 二叉树中序遍历
来源：http://sk.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pf.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://en.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pm.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yo.muxihuayi.cn

Java: // 手写递归
来源：http://fh.wgjwhj.cn

Go:   // 手写递归
来源：http://oz.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://md.muxihuayi.cn

C#:   // 手写递归
来源：http://lo.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ao.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://va.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zl.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://re.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tt.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lo.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zo.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yx.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pu.huixiangedu.cn


<!-- 参考信息 -->