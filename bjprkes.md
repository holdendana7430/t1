代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qc.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://ca.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gk.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://km.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ve.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tk.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hj.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ko.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iz.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rt.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://lf.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uo.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://su.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ki.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fy.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bf.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pc.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://at.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qj.panjiajie.cn

[K05] 深拷贝对象
来源：http://gf.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://ui.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://cz.9csxet.cn

JS:   structuredClone(obj)
来源：http://uc.colortex.cn

TS:   structuredClone(obj)
来源：http://ij.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ml.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rv.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://na.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pf.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://ms.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sh.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ky.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fo.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cb.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://om.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ul.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fy.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uz.yuexingan06.cn

[K07] 进制转换
来源：http://wg.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://os.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dm.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vb.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yw.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vg.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://og.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gt.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sv.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://fi.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://fu.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mt.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://pa.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://kd.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://do.9csxet.cn

Go:   encoding/gob
来源：http://sw.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://lk.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kk.chemitech.net.cn

================================================================================
来源：http://eo.huixiangedu.cn

L. 网络请求
来源：http://wg.hahajie.cn

================================================================================
来源：http://mf.521024.cn

[L01] 发送 GET 请求
来源：http://kf.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ql.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jf.muxihuayi.cn

JS:   await fetch(url)
来源：http://io.szxytkj.cn

TS:   await fetch(url)
来源：http://rd.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fb.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://tj.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rs.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ak.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://yi.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mm.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ok.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tj.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xh.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gq.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wq.shxzukj.cn

[L03] 设置自定义请求头
来源：http://vz.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mk.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hr.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://up.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ei.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fb.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uk.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nu.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ee.nicolike.cn

[L04] 设置超时
来源：http://dk.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://sh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dg.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zu.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bd.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lp.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gl.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lf.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://do.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ci.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uj.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vz.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://de.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rr.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lt.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cl.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uf.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://ri.lnxyls.cn

Py:   resp.json()
来源：http://pl.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://um.hahajie.cn

JS:   await resp.json()
来源：http://gw.hahajie.cn

TS:   await resp.json()
来源：http://zv.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rb.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mk.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://mv.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mh.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://xi.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ly.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nv.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ml.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://mc.muxihuayi.cn

Java: resp.statusCode()
来源：http://yj.9csxet.cn

Go:   resp.StatusCode
来源：http://ke.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://ig.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ce.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://wj.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fd.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://fv.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://az.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cm.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://de.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zw.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bt.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://io.521024.cn

================================================================================
来源：http://ee.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://yw.haigaiapp.cn

================================================================================
来源：http://iu.521024.cn

[M01] 读取命令行参数
来源：http://jt.szxytkj.cn

Py:   sys.argv[1:]
来源：http://dy.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://al.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://is.hahajie.cn

TS:   process.argv.slice(2)
来源：http://je.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://vy.muxihuayi.cn

Go:   os.Args[1:]
来源：http://jp.hnjuh.cn

Ruby: ARGV
来源：http://ig.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://gi.colortex.cn

[M02] 读取环境变量
来源：http://td.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://zr.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hf.jctech888.com.cn

JS:   process.env.HOME
来源：http://wy.jctech888.com.cn

TS:   process.env.HOME
来源：http://ch.huanxung.cn

Java: System.getenv("HOME")
来源：http://qz.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nd.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://mj.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uz.yuexingan06.cn

[M03] 执行外部命令
来源：http://ft.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qa.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xw.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dm.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ij.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dl.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vz.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uw.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://pv.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://we.nicolike.cn

Py:   os.getcwd()
来源：http://pa.lnxyls.cn

PHP:  getcwd();
来源：http://pu.wgjwhj.cn

JS:   process.cwd()
来源：http://jp.9csxet.cn

TS:   process.cwd()
来源：http://tz.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://wi.bookmarksfly.cn

Go:   os.Getwd()
来源：http://ul.9csxet.cn

Ruby: Dir.pwd
来源：http://co.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oo.newstarts.cn

[M05] 设置退出码
来源：http://cu.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://lm.newstarts.cn

PHP:  exit(1);
来源：http://jo.lnxyls.cn

JS:   process.exit(1)
来源：http://xv.jctech888.com.cn

TS:   process.exit(1)
来源：http://xg.bookmarksfly.cn

Java: System.exit(1)
来源：http://ob.colortex.cn

Go:   os.Exit(1)
来源：http://sl.muxihuayi.cn

Ruby: exit 1
来源：http://ix.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dx.chemitech.net.cn

[M06] 向标准错误输出
来源：http://mp.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://uv.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xm.yuntaijiaju.cn

JS:   console.error("err")
来源：http://eg.nszjky.cn

TS:   console.error("err")
来源：http://dn.nicolike.cn

Java: System.err.println("err")
来源：http://kk.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ym.yuexingan06.cn

Ruby: warn "err"
来源：http://fp.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://wt.colortex.cn

[M07] 判断是否为主入口
来源：http://rx.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://yf.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sy.chemitech.net.cn

JS:   require.main === module
来源：http://qw.newstarts.cn

TS:   require.main === module
来源：http://gw.gzmigu.cn

Java: public static void main(String[] args)
来源：http://kq.bjjhwx.cn

Go:   func main()
来源：http://dw.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://do.huanxung.cn

C#:   static void Main(string[] args)
来源：http://us.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://tx.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://eu.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://mt.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://wn.lnxyls.cn

TS:   process.platform;  process.version
来源：http://jg.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ge.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vf.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eh.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dh.hahajie.cn

================================================================================
来源：http://go.colortex.cn

N. 数据结构与算法
来源：http://ie.jctech888.com.cn

================================================================================
来源：http://zv.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://nk.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vv.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gd.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hw.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gk.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nm.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://oq.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gi.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iw.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://el.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rg.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xf.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gl.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mq.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ly.hahajie.cn

Go:   slices.Sort(arr)
来源：http://fk.chemitech.net.cn

Ruby: arr.sort
来源：http://qa.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mr.521024.cn

[N03] 快速排序（分治示例）
来源：http://eq.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xh.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://pf.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ve.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uo.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://es.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bf.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zw.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mb.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://op.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fz.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sv.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nr.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://du.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tv.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ow.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wl.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xh.haigaiapp.cn

[N05] 最大公约数
来源：http://gy.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ad.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://an.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xv.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://np.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ej.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eb.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://sj.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://da.colortex.cn

[N06] 判断回文字符串
来源：http://hd.muxihuayi.cn

Py:   s == s[::-1]
来源：http://wk.nicolike.cn

PHP:  $s === strrev($s);
来源：http://dw.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://gu.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://pa.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xp.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://pv.huanxung.cn

Ruby: s == s.reverse
来源：http://vw.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oj.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://dm.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zo.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ac.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uj.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://qi.colortex.cn

Java: // 手写 HashMap
来源：http://ec.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://yx.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://fs.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pa.shxzskj.cn

[N08] 生成全排列
来源：http://qy.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://li.szxytkj.cn

PHP:  // 手写递归交换
来源：http://ph.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://bb.hnjuh.cn

TS:   // 手写回溯递归
来源：http://av.521024.cn

Java: // 手写回溯递归
来源：http://ts.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://oh.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://lr.szsharing.cn

C#:   // 手写回溯递归
来源：http://rk.hahajie.cn

[N09] 栈与队列
来源：http://ym.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kq.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qe.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ey.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mz.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dw.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ud.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lc.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wg.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://ak.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://io.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mh.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lm.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fj.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://bk.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mj.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hb.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iz.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://pw.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bl.huanxung.cn


<!-- 参考信息 -->