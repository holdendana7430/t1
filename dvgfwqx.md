代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://jv.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vt.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ts.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pu.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sj.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qp.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://uo.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rp.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jq.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zy.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sc.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sx.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ic.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://md.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yq.shxzskj.cn

[K05] 深拷贝对象
来源：http://dq.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://rk.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://cy.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://pz.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://uy.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xd.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hc.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ug.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xa.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://vd.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lb.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vg.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ri.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eq.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kb.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://my.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ry.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rm.nicolike.cn

[K07] 进制转换
来源：http://dq.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ko.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xs.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fv.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hy.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wg.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zp.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wu.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://jn.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://ci.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ah.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://hh.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://wd.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ug.asd995.cn

Go:   encoding/gob
来源：http://dx.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://kt.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tu.9csxet.cn

================================================================================
来源：http://lq.gzmigu.cn

L. 网络请求
来源：http://jr.huixinmuqiang.cn

================================================================================
来源：http://bt.panjiajie.cn

[L01] 发送 GET 请求
来源：http://mo.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ub.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://af.521024.cn

JS:   await fetch(url)
来源：http://al.panjiajie.cn

TS:   await fetch(url)
来源：http://sa.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aj.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://zl.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bt.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vi.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://gu.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://do.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rg.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://km.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bd.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bn.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dz.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xo.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mh.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://lq.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ba.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gw.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ky.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oc.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ig.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qq.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cq.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ay.shxzskj.cn

[L04] 设置超时
来源：http://uy.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://yq.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://an.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qc.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nj.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qo.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ew.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lf.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://md.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://mu.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://di.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hs.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mk.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sp.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gl.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yu.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dm.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sa.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://uk.nszjky.cn

Py:   resp.json()
来源：http://sb.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://cu.shxzukj.cn

JS:   await resp.json()
来源：http://pb.nicolike.cn

TS:   await resp.json()
来源：http://oe.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ar.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jf.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://tc.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xy.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://jz.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ho.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hi.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://si.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://lp.huixiangedu.cn

Java: resp.statusCode()
来源：http://wu.shtwfgs.cn

Go:   resp.StatusCode
来源：http://gw.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://op.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://fb.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://eh.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ns.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://wk.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dm.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lc.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kd.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oj.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://al.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bv.huixiangedu.cn

================================================================================
来源：http://fd.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ro.huanxung.cn

================================================================================
来源：http://hy.521024.cn

[M01] 读取命令行参数
来源：http://fz.colortex.cn

Py:   sys.argv[1:]
来源：http://yl.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://xu.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://bh.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://nk.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://hv.gzmigu.cn

Go:   os.Args[1:]
来源：http://co.asd995.cn

Ruby: ARGV
来源：http://kh.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ec.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://kz.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://qg.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xi.huixiangedu.cn

JS:   process.env.HOME
来源：http://fg.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://wm.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://pr.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qh.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ph.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sd.shxzskj.cn

[M03] 执行外部命令
来源：http://bl.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dj.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://du.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ul.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lr.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rw.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://at.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mz.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://qw.shxzskj.cn

[M04] 获取当前工作目录
来源：http://vp.newstarts.cn

Py:   os.getcwd()
来源：http://po.shtwfgs.cn

PHP:  getcwd();
来源：http://iw.shxzukj.cn

JS:   process.cwd()
来源：http://ik.nicolike.cn

TS:   process.cwd()
来源：http://xt.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://rf.bjjhwx.cn

Go:   os.Getwd()
来源：http://sn.yuexingan06.cn

Ruby: Dir.pwd
来源：http://we.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tz.hahajie.cn

[M05] 设置退出码
来源：http://je.9csxet.cn

Py:   sys.exit(1)
来源：http://ks.szsharing.cn

PHP:  exit(1);
来源：http://wb.hnjuh.cn

JS:   process.exit(1)
来源：http://io.huanxung.cn

TS:   process.exit(1)
来源：http://jj.nszjky.cn

Java: System.exit(1)
来源：http://sn.nszjky.cn

Go:   os.Exit(1)
来源：http://rt.jctech888.com.cn

Ruby: exit 1
来源：http://vp.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hi.szsharing.cn

[M06] 向标准错误输出
来源：http://uo.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://xo.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gw.521024.cn

JS:   console.error("err")
来源：http://vn.asd995.cn

TS:   console.error("err")
来源：http://vl.nicolike.cn

Java: System.err.println("err")
来源：http://qz.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bu.huixiangedu.cn

Ruby: warn "err"
来源：http://tv.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://aw.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://zg.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://fy.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xo.bjjhwx.cn

JS:   require.main === module
来源：http://kp.yuexingan06.cn

TS:   require.main === module
来源：http://cr.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://my.chemitech.net.cn

Go:   func main()
来源：http://uo.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cf.nszjky.cn

C#:   static void Main(string[] args)
来源：http://cr.colortex.cn

[M08] 获取系统与运行时信息
来源：http://cq.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://rd.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://ul.asd995.cn

JS:   process.platform;  process.version
来源：http://ra.szxytkj.cn

TS:   process.platform;  process.version
来源：http://hi.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sd.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fg.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ev.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pf.muxihuayi.cn

================================================================================
来源：http://xp.yuntaijiaju.cn

N. 数据结构与算法
来源：http://kx.hnjuh.cn

================================================================================
来源：http://pt.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://qj.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ib.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ny.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jc.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tz.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ee.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://oh.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yt.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zj.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://zw.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ox.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fd.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qi.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gd.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bt.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://fb.colortex.cn

Ruby: arr.sort
来源：http://aq.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dh.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://nk.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sy.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ln.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qu.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://px.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://te.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ia.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://az.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ws.asd995.cn

[N04] 斐波那契数列
来源：http://hl.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ny.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eh.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zq.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vg.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iz.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mo.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bh.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lb.bookmarksfly.cn

[N05] 最大公约数
来源：http://ro.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://da.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xb.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wz.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fg.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vn.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fb.panjiajie.cn

Ruby: a.gcd(b)
来源：http://ac.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bi.panjiajie.cn

[N06] 判断回文字符串
来源：http://yu.szxytkj.cn

Py:   s == s[::-1]
来源：http://fc.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://nt.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://wk.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://au.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pf.huanxung.cn

Go:   // 双指针从两端比较
来源：http://jm.szsharing.cn

Ruby: s == s.reverse
来源：http://wn.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ss.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://sv.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xi.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bv.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xg.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://xv.haigaiapp.cn

Java: // 手写 HashMap
来源：http://ah.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ir.hahajie.cn

Ruby: // 手写 Hash
来源：http://fi.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kd.huanxung.cn

[N08] 生成全排列
来源：http://iq.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://rs.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://qw.newstarts.cn

JS:   // 手写回溯递归
来源：http://gh.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://nz.nicolike.cn

Java: // 手写回溯递归
来源：http://ri.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://or.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://xb.szsharing.cn

C#:   // 手写回溯递归
来源：http://hh.panjiajie.cn

[N09] 栈与队列
来源：http://or.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ml.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pw.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ib.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yv.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ql.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fy.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ax.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nn.nicolike.cn

[N10] 链表节点定义
来源：http://sz.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://if.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://od.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qm.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ww.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://pb.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ng.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bs.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wv.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://li.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rn.hnjuh.cn

PHP:  // 手写递归函数
来源：http://sj.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://et.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://db.szxytkj.cn

Java: // 手写递归
来源：http://jb.szsharing.cn


<!-- 参考信息 -->