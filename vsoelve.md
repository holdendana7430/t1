代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://za.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ma.lnxyls.cn

[J09] 时区处理
来源：http://ot.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zn.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ed.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ri.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pk.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ue.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ay.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jd.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fl.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://mf.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oq.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cd.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qn.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uq.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bl.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://da.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gj.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kz.newstarts.cn

================================================================================
来源：http://sj.asd995.cn

K. JSON 与序列化
来源：http://fj.muxihuayi.cn

================================================================================
来源：http://hf.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://am.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yw.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xv.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://sa.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://eg.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vj.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://nd.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yt.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://le.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ok.wgjwhj.cn

Py:   json.loads(s)
来源：http://dv.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qp.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://rj.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ff.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zr.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://eq.521024.cn

Ruby: JSON.parse(s)
来源：http://ib.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mn.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ev.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rl.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bb.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dd.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ym.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://px.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wq.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ez.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ce.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://eg.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nz.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fb.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ek.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uo.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ay.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xk.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ft.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ty.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://kc.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://zk.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ri.szxytkj.cn

TS:   structuredClone(obj)
来源：http://qr.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vv.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tb.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sm.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uo.szsharing.cn

[K06] 解析 URL 查询串
来源：http://pi.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ne.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pp.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nl.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bn.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hp.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kw.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://we.521024.cn

[K07] 进制转换
来源：http://bq.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://al.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ts.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://co.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ey.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aa.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://da.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ua.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qp.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://rm.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://kg.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jm.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://vo.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ai.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yn.newstarts.cn

Go:   encoding/gob
来源：http://kw.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://vp.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://iq.yuexingan06.cn

L. 网络请求
来源：http://bv.lnxyls.cn

================================================================================
来源：http://ox.panjiajie.cn

[L01] 发送 GET 请求
来源：http://wa.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jg.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://io.hahajie.cn

JS:   await fetch(url)
来源：http://fo.9csxet.cn

TS:   await fetch(url)
来源：http://tc.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rt.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ow.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ap.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lx.colortex.cn

[L02] 发送 POST JSON
来源：http://zd.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ms.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://db.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vp.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://me.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kd.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://or.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ac.521024.cn

[L03] 设置自定义请求头
来源：http://pi.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ak.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ab.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://by.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://og.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kx.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qx.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://np.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jx.hahajie.cn

[L04] 设置超时
来源：http://ch.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://mu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rn.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vw.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lu.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aq.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tw.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uf.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://or.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://nt.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ma.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rm.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rg.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sp.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pd.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uw.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nu.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://yx.newstarts.cn

Py:   resp.json()
来源：http://iq.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://bd.newstarts.cn

JS:   await resp.json()
来源：http://cx.shxzskj.cn

TS:   await resp.json()
来源：http://oj.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bb.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ji.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://uq.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gl.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://ko.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qn.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ve.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://me.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://yf.bookmarksfly.cn

Java: resp.statusCode()
来源：http://am.gzmigu.cn

Go:   resp.StatusCode
来源：http://cu.hnjuh.cn

Ruby: resp.code.to_i
来源：http://td.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://yi.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://ko.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hy.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://fg.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yu.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://of.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yo.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wh.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gz.gzmigu.cn

================================================================================
来源：http://ky.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://aj.muxihuayi.cn

================================================================================
来源：http://gt.nicolike.cn

[M01] 读取命令行参数
来源：http://rh.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ng.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://uo.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://sl.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://vw.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://mf.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ad.nszjky.cn

Ruby: ARGV
来源：http://yf.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://ta.bookmarksfly.cn

[M02] 读取环境变量
来源：http://tp.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://sv.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jy.nszjky.cn

JS:   process.env.HOME
来源：http://ca.colortex.cn

TS:   process.env.HOME
来源：http://of.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://nj.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dz.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ev.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dp.jctech888.com.cn

[M03] 执行外部命令
来源：http://bd.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ty.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dn.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cj.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gk.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rs.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ox.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fs.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://uv.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://px.shxzskj.cn

Py:   os.getcwd()
来源：http://og.bookmarksfly.cn

PHP:  getcwd();
来源：http://lm.chemitech.net.cn

JS:   process.cwd()
来源：http://ph.colortex.cn

TS:   process.cwd()
来源：http://ir.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://yv.colortex.cn

Go:   os.Getwd()
来源：http://rd.asd995.cn

Ruby: Dir.pwd
来源：http://mh.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oa.nszjky.cn

[M05] 设置退出码
来源：http://rk.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://vq.nicolike.cn

PHP:  exit(1);
来源：http://lc.huixiangedu.cn

JS:   process.exit(1)
来源：http://yb.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ho.szsharing.cn

Java: System.exit(1)
来源：http://ms.wgjwhj.cn

Go:   os.Exit(1)
来源：http://uz.bookmarksfly.cn

Ruby: exit 1
来源：http://wq.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gx.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://bw.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://xi.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yi.haigaiapp.cn

JS:   console.error("err")
来源：http://fz.shxzukj.cn

TS:   console.error("err")
来源：http://di.haigaiapp.cn

Java: System.err.println("err")
来源：http://ml.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lb.jctech888.com.cn

Ruby: warn "err"
来源：http://py.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://zq.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ub.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://xd.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ca.shxzskj.cn

JS:   require.main === module
来源：http://jv.jianghongdianzi.cn

TS:   require.main === module
来源：http://lx.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://cw.huixinmuqiang.cn

Go:   func main()
来源：http://ak.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uz.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://sj.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://uk.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://al.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://yd.shxzukj.cn

JS:   process.platform;  process.version
来源：http://cv.shxzukj.cn

TS:   process.platform;  process.version
来源：http://zi.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tn.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ag.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dl.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lx.asd995.cn

================================================================================
来源：http://iy.huixinmuqiang.cn

N. 数据结构与算法
来源：http://wg.nszjky.cn

================================================================================
来源：http://ww.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://jn.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lo.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bc.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zm.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ef.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xx.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://ny.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zr.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ht.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://np.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://bi.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bk.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xn.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qb.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dk.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ue.newstarts.cn

Ruby: arr.sort
来源：http://ix.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sf.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://cd.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xw.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://lj.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://py.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lq.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jb.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aw.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fn.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wi.shxzskj.cn

[N04] 斐波那契数列
来源：http://oo.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qd.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kw.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wh.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://os.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mo.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tg.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ll.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sm.szxytkj.cn

[N05] 最大公约数
来源：http://pp.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://xr.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ab.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aw.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pf.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nu.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ag.szsharing.cn

Ruby: a.gcd(b)
来源：http://yc.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zf.chemitech.net.cn

[N06] 判断回文字符串
来源：http://pg.colortex.cn

Py:   s == s[::-1]
来源：http://es.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://wd.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://bj.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://ii.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xk.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://xi.lnxyls.cn


<!-- 参考信息 -->