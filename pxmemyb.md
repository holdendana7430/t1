代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://sk.hahajie.cn

[J08] 提取年月日与星期
来源：http://rr.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ja.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ih.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kp.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://os.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://es.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zd.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ef.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yt.szsharing.cn

[J09] 时区处理
来源：http://op.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qq.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uw.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://of.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bj.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ti.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lc.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://om.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lu.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://qa.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dr.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ix.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mz.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nh.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oi.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://km.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fs.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://um.szxytkj.cn

================================================================================
来源：http://yv.szxytkj.cn

K. JSON 与序列化
来源：http://oe.huanxung.cn

================================================================================
来源：http://ak.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://pa.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ws.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vn.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://xv.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://nj.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gs.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://qk.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qj.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vl.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ve.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ep.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://km.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://eu.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ok.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ft.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://ty.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ip.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tc.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://cr.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jf.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wz.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dt.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sb.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nd.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sg.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iq.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sr.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://ln.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oo.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uz.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yf.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hv.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ng.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wc.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://do.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bh.huixiangedu.cn

[K05] 深拷贝对象
来源：http://op.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://fs.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://wj.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://wq.shxzskj.cn

TS:   structuredClone(obj)
来源：http://zv.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rd.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bm.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fw.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oo.9csxet.cn

[K06] 解析 URL 查询串
来源：http://dh.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://er.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bw.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fy.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ar.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jx.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zo.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://du.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ie.colortex.cn

[K07] 进制转换
来源：http://py.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ok.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ar.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oe.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wf.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gp.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ab.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://io.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://at.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://re.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://jf.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://af.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nr.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://sf.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rv.shtwfgs.cn

Go:   encoding/gob
来源：http://dk.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://rf.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://be.lnxyls.cn

================================================================================
来源：http://tz.haigaiapp.cn

L. 网络请求
来源：http://jf.yuexingan06.cn

================================================================================
来源：http://rj.asd995.cn

[L01] 发送 GET 请求
来源：http://li.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://or.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ix.9csxet.cn

JS:   await fetch(url)
来源：http://ad.shxzukj.cn

TS:   await fetch(url)
来源：http://qq.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vy.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://ap.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ys.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cr.hahajie.cn

[L02] 发送 POST JSON
来源：http://xn.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uf.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ab.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qm.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dr.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hb.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ih.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qw.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ha.asd995.cn

[L03] 设置自定义请求头
来源：http://en.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wg.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pn.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ak.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nk.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sh.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://or.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pi.bookmarksfly.cn

[L04] 设置超时
来源：http://at.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://tj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ap.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ua.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jm.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ss.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ob.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qg.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yp.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ih.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ws.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ua.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ns.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qk.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ub.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pq.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mz.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ux.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://if.yuntaijiaju.cn

Py:   resp.json()
来源：http://qv.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://ws.asd995.cn

JS:   await resp.json()
来源：http://xt.huixiangedu.cn

TS:   await resp.json()
来源：http://ae.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dz.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bw.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://oj.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://za.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://wu.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ec.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wd.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://pv.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://vx.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://id.yuexingan06.cn

Go:   resp.StatusCode
来源：http://zy.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://wb.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://zc.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://kl.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ti.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://pj.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oj.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dk.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uk.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fz.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ip.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ui.bjjhwx.cn

================================================================================
来源：http://mv.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://xi.yuntaijiaju.cn

================================================================================
来源：http://bt.szsharing.cn

[M01] 读取命令行参数
来源：http://vp.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://xo.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://tm.asd995.cn

JS:   process.argv.slice(2)
来源：http://uj.newstarts.cn

TS:   process.argv.slice(2)
来源：http://yt.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://fq.panjiajie.cn

Go:   os.Args[1:]
来源：http://ty.lnxyls.cn

Ruby: ARGV
来源：http://hk.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://rl.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://pw.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://fz.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vs.521024.cn

JS:   process.env.HOME
来源：http://uk.gzmigu.cn

TS:   process.env.HOME
来源：http://lk.nicolike.cn

Java: System.getenv("HOME")
来源：http://ol.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qj.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://qm.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ih.nicolike.cn

[M03] 执行外部命令
来源：http://ni.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hp.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ql.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ct.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ca.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vw.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wj.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://og.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://gy.shxzukj.cn

[M04] 获取当前工作目录
来源：http://fg.szsharing.cn

Py:   os.getcwd()
来源：http://ug.bjjhwx.cn

PHP:  getcwd();
来源：http://rf.nszjky.cn

JS:   process.cwd()
来源：http://ew.hahajie.cn

TS:   process.cwd()
来源：http://as.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://rj.9csxet.cn

Go:   os.Getwd()
来源：http://gt.colortex.cn

Ruby: Dir.pwd
来源：http://sy.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bb.lnxyls.cn

[M05] 设置退出码
来源：http://di.nicolike.cn

Py:   sys.exit(1)
来源：http://oo.colortex.cn

PHP:  exit(1);
来源：http://dk.chemitech.net.cn

JS:   process.exit(1)
来源：http://go.nszjky.cn

TS:   process.exit(1)
来源：http://rn.muxihuayi.cn

Java: System.exit(1)
来源：http://ui.jctech888.com.cn

Go:   os.Exit(1)
来源：http://tt.shtwfgs.cn

Ruby: exit 1
来源：http://td.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vk.newstarts.cn

[M06] 向标准错误输出
来源：http://ka.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://zt.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kr.shxzskj.cn

JS:   console.error("err")
来源：http://kn.panjiajie.cn

TS:   console.error("err")
来源：http://ki.nszjky.cn

Java: System.err.println("err")
来源：http://lg.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xp.huixiangedu.cn

Ruby: warn "err"
来源：http://ak.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://bj.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://bz.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://ux.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ka.hnjuh.cn

JS:   require.main === module
来源：http://pz.hnjuh.cn

TS:   require.main === module
来源：http://of.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://zu.huixiangedu.cn

Go:   func main()
来源：http://uc.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vw.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://to.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://hy.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://xp.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://lq.asd995.cn

JS:   process.platform;  process.version
来源：http://lb.9csxet.cn

TS:   process.platform;  process.version
来源：http://ax.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cj.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wg.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mz.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wt.huixiangedu.cn

================================================================================
来源：http://qv.wgjwhj.cn

N. 数据结构与算法
来源：http://ka.9csxet.cn

================================================================================
来源：http://ca.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://dr.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://du.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jf.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ew.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fl.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hh.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://qe.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ll.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cx.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://mp.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://us.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hh.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pq.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ic.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ri.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://ut.hahajie.cn

Ruby: arr.sort
来源：http://eb.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ma.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://xn.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mi.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://lc.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cb.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ne.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cv.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yb.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cz.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gi.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://nr.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qh.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ym.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://de.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rt.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wp.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uq.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ih.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://no.shxzskj.cn

[N05] 最大公约数
来源：http://ny.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://vu.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ws.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://md.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://om.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ht.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ie.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://qn.huixiangedu.cn


<!-- 参考信息 -->