代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tq.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pu.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yw.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://na.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iu.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vz.asd995.cn

[J09] 时区处理
来源：http://rc.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ff.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ge.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yy.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ik.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ao.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cx.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ak.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jh.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://za.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uy.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://of.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ry.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uw.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oj.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qx.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zj.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ky.huixinmuqiang.cn

================================================================================
来源：http://ts.shxzskj.cn

K. JSON 与序列化
来源：http://sp.jctech888.com.cn

================================================================================
来源：http://ef.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://mb.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lf.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yb.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://un.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://us.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fj.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://zz.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ha.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tw.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://co.haigaiapp.cn

Py:   json.loads(s)
来源：http://mq.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gp.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ak.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://sl.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rx.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://cx.colortex.cn

Ruby: JSON.parse(s)
来源：http://tt.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rb.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://fk.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iw.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://de.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mj.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fr.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zg.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mx.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://in.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://is.colortex.cn

[K04] 读取 JSON 文件
来源：http://qt.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cz.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hx.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wc.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tg.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://da.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rw.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ee.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ld.muxihuayi.cn

[K05] 深拷贝对象
来源：http://rb.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://dv.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://tq.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://op.gzmigu.cn

TS:   structuredClone(obj)
来源：http://gq.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nr.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jy.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mm.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ex.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://ed.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pl.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tz.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://du.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zm.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pp.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ho.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qj.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vo.shxzskj.cn

[K07] 进制转换
来源：http://qi.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nj.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wy.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yz.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dp.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nk.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sr.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gy.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ws.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yj.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://dc.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sn.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://iq.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ye.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yd.huixinmuqiang.cn

Go:   encoding/gob
来源：http://wd.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://cy.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zk.szsharing.cn

================================================================================
来源：http://wd.lnxyls.cn

L. 网络请求
来源：http://lu.jianghongdianzi.cn

================================================================================
来源：http://xy.huanxung.cn

[L01] 发送 GET 请求
来源：http://rx.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gn.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ey.hnjuh.cn

JS:   await fetch(url)
来源：http://qb.bjjhwx.cn

TS:   await fetch(url)
来源：http://he.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oe.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://nv.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oa.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yz.lnxyls.cn

[L02] 发送 POST JSON
来源：http://vo.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xy.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lr.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ep.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uw.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nz.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xz.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wa.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gd.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://se.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kt.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sl.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zd.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qg.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kz.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wt.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://px.shxzukj.cn

[L04] 设置超时
来源：http://xh.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ul.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yp.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cg.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uf.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fo.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://td.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hp.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pk.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://og.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ht.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yf.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ex.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wa.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ut.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vr.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wx.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://tp.nicolike.cn

Py:   resp.json()
来源：http://se.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://ez.shtwfgs.cn

JS:   await resp.json()
来源：http://ux.shxzukj.cn

TS:   await resp.json()
来源：http://wa.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ty.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cd.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://lv.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ux.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://hs.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bf.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cv.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://gc.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://jv.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://vs.shxzukj.cn

Go:   resp.StatusCode
来源：http://xd.hnjuh.cn

Ruby: resp.code.to_i
来源：http://uq.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://wz.nicolike.cn

[L08] 并发请求多个地址
来源：http://qk.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xe.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://cv.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eu.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mo.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zt.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lw.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vt.bookmarksfly.cn

================================================================================
来源：http://ui.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://xh.bookmarksfly.cn

================================================================================
来源：http://cb.nicolike.cn

[M01] 读取命令行参数
来源：http://kr.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://kr.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://nt.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://rz.521024.cn

TS:   process.argv.slice(2)
来源：http://wj.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://sc.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://dy.panjiajie.cn

Ruby: ARGV
来源：http://ii.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://in.asd995.cn

[M02] 读取环境变量
来源：http://gj.colortex.cn

Py:   os.environ.get("HOME")
来源：http://hc.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://op.bookmarksfly.cn

JS:   process.env.HOME
来源：http://oy.panjiajie.cn

TS:   process.env.HOME
来源：http://cq.nicolike.cn

Java: System.getenv("HOME")
来源：http://zz.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hh.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://li.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rr.9csxet.cn

[M03] 执行外部命令
来源：http://hn.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://id.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zv.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fw.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bk.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gu.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rz.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://za.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://jq.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ln.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://jq.bjjhwx.cn

PHP:  getcwd();
来源：http://mm.chemitech.net.cn

JS:   process.cwd()
来源：http://ju.lnxyls.cn

TS:   process.cwd()
来源：http://ol.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://pn.hahajie.cn

Go:   os.Getwd()
来源：http://ne.haigaiapp.cn

Ruby: Dir.pwd
来源：http://co.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://da.muxihuayi.cn

[M05] 设置退出码
来源：http://nn.hahajie.cn

Py:   sys.exit(1)
来源：http://gq.shxzukj.cn

PHP:  exit(1);
来源：http://fe.lnxyls.cn

JS:   process.exit(1)
来源：http://ur.bookmarksfly.cn

TS:   process.exit(1)
来源：http://mg.shtwfgs.cn

Java: System.exit(1)
来源：http://oe.chemitech.net.cn

Go:   os.Exit(1)
来源：http://xv.bjjhwx.cn

Ruby: exit 1
来源：http://om.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wh.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://fi.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://qz.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rx.szsharing.cn

JS:   console.error("err")
来源：http://iq.huanxung.cn

TS:   console.error("err")
来源：http://lb.521024.cn

Java: System.err.println("err")
来源：http://ed.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bs.shtwfgs.cn

Ruby: warn "err"
来源：http://ur.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://jq.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://uh.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://zv.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ef.hnjuh.cn

JS:   require.main === module
来源：http://qm.muxihuayi.cn

TS:   require.main === module
来源：http://im.asd995.cn

Java: public static void main(String[] args)
来源：http://tt.jianghongdianzi.cn

Go:   func main()
来源：http://fx.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wd.newstarts.cn

C#:   static void Main(string[] args)
来源：http://yv.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://jl.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://at.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://se.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://hd.gzmigu.cn

TS:   process.platform;  process.version
来源：http://ls.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ew.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dh.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fk.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gd.hahajie.cn

================================================================================
来源：http://wk.szxytkj.cn

N. 数据结构与算法
来源：http://qr.szxytkj.cn

================================================================================
来源：http://ci.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://xv.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://in.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kj.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dt.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://km.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xf.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xc.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sd.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uf.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://hx.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xz.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gh.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vw.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jy.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ba.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://aw.9csxet.cn

Ruby: arr.sort
来源：http://yf.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fc.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://gq.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cg.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://uu.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eb.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mh.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gd.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mk.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ls.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ne.wgjwhj.cn

[N04] 斐波那契数列
来源：http://ks.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xl.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dr.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ni.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ol.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mt.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uy.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jt.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vc.gzmigu.cn

[N05] 最大公约数
来源：http://cd.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://su.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rb.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bi.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ga.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://be.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://db.newstarts.cn

Ruby: a.gcd(b)
来源：http://qn.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cw.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://gv.newstarts.cn

Py:   s == s[::-1]
来源：http://ue.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://ve.chemitech.net.cn


<!-- 参考信息 -->