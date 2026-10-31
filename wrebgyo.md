代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://bz.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rn.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qo.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nq.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://te.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bw.521024.cn

[K04] 读取 JSON 文件
来源：http://xl.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mr.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fv.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://br.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ws.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xs.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pb.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gk.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lf.gzmigu.cn

[K05] 深拷贝对象
来源：http://qj.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://qv.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://lr.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://qt.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ir.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tv.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bl.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iu.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dt.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://cm.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://so.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ug.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bf.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xj.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hg.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mq.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cl.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pg.colortex.cn

[K07] 进制转换
来源：http://ly.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mq.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pb.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oy.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://po.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ce.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yh.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ti.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://km.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://yj.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://tv.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dz.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://sb.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://tr.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ll.bookmarksfly.cn

Go:   encoding/gob
来源：http://ol.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://cp.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vs.nicolike.cn

================================================================================
来源：http://nn.521024.cn

L. 网络请求
来源：http://az.szsharing.cn

================================================================================
来源：http://xb.szsharing.cn

[L01] 发送 GET 请求
来源：http://wg.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ly.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gu.hnjuh.cn

JS:   await fetch(url)
来源：http://bv.muxihuayi.cn

TS:   await fetch(url)
来源：http://vv.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rb.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://ng.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ym.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jg.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://yi.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sa.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qu.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vy.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lz.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rm.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cs.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vs.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://dx.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://em.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ls.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gv.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pt.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gd.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fi.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cw.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tb.jianghongdianzi.cn

[L04] 设置超时
来源：http://nq.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://pb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pr.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hl.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kh.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iy.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bv.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lr.huanxung.cn

[L05] 上传文件（multipart）
来源：http://mm.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iv.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://du.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://io.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yf.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uw.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://up.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hw.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ln.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ga.hnjuh.cn

Py:   resp.json()
来源：http://hs.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://om.asd995.cn

JS:   await resp.json()
来源：http://xo.yuntaijiaju.cn

TS:   await resp.json()
来源：http://hn.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xd.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ke.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://th.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wb.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://at.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ba.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://dr.colortex.cn

TS:   resp.ok;  resp.status
来源：http://oo.hahajie.cn

Java: resp.statusCode()
来源：http://pr.szsharing.cn

Go:   resp.StatusCode
来源：http://zd.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://of.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://tc.newstarts.cn

[L08] 并发请求多个地址
来源：http://xw.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xi.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://rx.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vb.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://op.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mm.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zi.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rp.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xw.gzmigu.cn

================================================================================
来源：http://bl.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://my.muxihuayi.cn

================================================================================
来源：http://or.521024.cn

[M01] 读取命令行参数
来源：http://xq.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://fx.nszjky.cn

PHP:  $argv;  $argc;
来源：http://wd.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://sw.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://oi.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://ge.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://nm.hnjuh.cn

Ruby: ARGV
来源：http://oh.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://nj.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ak.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://zr.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vs.hnjuh.cn

JS:   process.env.HOME
来源：http://tq.521024.cn

TS:   process.env.HOME
来源：http://hx.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://fz.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tk.hahajie.cn

Ruby: ENV["HOME"]
来源：http://hs.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jt.gzmigu.cn

[M03] 执行外部命令
来源：http://px.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zh.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ms.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hl.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dg.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mf.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://qg.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://qs.521024.cn

Py:   os.getcwd()
来源：http://gj.hnjuh.cn

PHP:  getcwd();
来源：http://mt.nicolike.cn

JS:   process.cwd()
来源：http://lo.jctech888.com.cn

TS:   process.cwd()
来源：http://os.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://fi.jctech888.com.cn

Go:   os.Getwd()
来源：http://vm.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://hx.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lz.lnxyls.cn

[M05] 设置退出码
来源：http://ay.wgjwhj.cn

Py:   sys.exit(1)
来源：http://gv.521024.cn

PHP:  exit(1);
来源：http://ja.asd995.cn

JS:   process.exit(1)
来源：http://yi.panjiajie.cn

TS:   process.exit(1)
来源：http://gd.bookmarksfly.cn

Java: System.exit(1)
来源：http://hg.asd995.cn

Go:   os.Exit(1)
来源：http://xp.colortex.cn

Ruby: exit 1
来源：http://cy.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.hnjuh.cn

[M06] 向标准错误输出
来源：http://um.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://rl.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kc.jctech888.com.cn

JS:   console.error("err")
来源：http://em.nszjky.cn

TS:   console.error("err")
来源：http://ds.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ft.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kg.asd995.cn

Ruby: warn "err"
来源：http://yn.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://dd.521024.cn

[M07] 判断是否为主入口
来源：http://ae.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://lv.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ps.asd995.cn

JS:   require.main === module
来源：http://do.shxzukj.cn

TS:   require.main === module
来源：http://pw.521024.cn

Java: public static void main(String[] args)
来源：http://ss.bjjhwx.cn

Go:   func main()
来源：http://kz.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eq.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://ke.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://qf.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://td.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://im.shxzskj.cn

JS:   process.platform;  process.version
来源：http://sj.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://mt.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gu.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ga.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bq.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://di.lnxyls.cn

================================================================================
来源：http://ll.haigaiapp.cn

N. 数据结构与算法
来源：http://id.newstarts.cn

================================================================================
来源：http://nz.521024.cn

[N01] 二分查找（有序数组）
来源：http://hz.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://me.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fd.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://am.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bd.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://js.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ye.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yv.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://kb.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://zm.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bs.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gk.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://se.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nz.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://bx.muxihuayi.cn

Ruby: arr.sort
来源：http://dy.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zy.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://ku.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fg.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://au.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uk.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cl.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tb.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://db.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cj.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kj.muxihuayi.cn

[N04] 斐波那契数列
来源：http://fc.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ud.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kr.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cw.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qn.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sr.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lb.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kl.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jj.nszjky.cn

[N05] 最大公约数
来源：http://ik.hahajie.cn

Py:   math.gcd(a, b)
来源：http://qu.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mi.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ra.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zw.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ly.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://le.hnjuh.cn

Ruby: a.gcd(b)
来源：http://cn.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wy.huanxung.cn

[N06] 判断回文字符串
来源：http://wm.nszjky.cn

Py:   s == s[::-1]
来源：http://ty.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://io.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ry.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://zq.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uk.521024.cn

Go:   // 双指针从两端比较
来源：http://qk.nszjky.cn

Ruby: s == s.reverse
来源：http://ux.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://py.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://pq.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bb.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ib.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qr.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://ob.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://nn.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://bt.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://vv.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bd.newstarts.cn

[N08] 生成全排列
来源：http://rz.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://fu.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://ui.huanxung.cn

JS:   // 手写回溯递归
来源：http://zj.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://ph.panjiajie.cn

Java: // 手写回溯递归
来源：http://pk.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://ne.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://bc.lnxyls.cn

C#:   // 手写回溯递归
来源：http://el.huixiangedu.cn

[N09] 栈与队列
来源：http://nr.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bb.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://px.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sj.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vh.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fi.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pi.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tb.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tj.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://rv.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vv.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pi.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ll.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tg.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://mv.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cw.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wl.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wt.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://ab.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pu.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://pz.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bm.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wq.nicolike.cn

Java: // 手写递归
来源：http://qh.nszjky.cn


<!-- 参考信息 -->