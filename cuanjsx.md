代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://ya.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://kq.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kk.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zg.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dd.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://if.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vh.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ah.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mp.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://km.bookmarksfly.cn

[J09] 时区处理
来源：http://ml.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hu.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qc.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vr.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qx.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ak.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kq.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wn.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sp.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://dn.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wy.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hv.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ny.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ad.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ds.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cy.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pw.nicolike.cn

================================================================================
来源：http://bp.haigaiapp.cn

K. JSON 与序列化
来源：http://fn.jctech888.com.cn

================================================================================
来源：http://rt.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://la.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bm.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hk.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://dv.521024.cn

TS:   JSON.stringify(obj)
来源：http://ap.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hh.huanxung.cn

Go:   json.Marshal(obj)
来源：http://mw.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wa.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pp.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://sy.bjjhwx.cn

Py:   json.loads(s)
来源：http://tv.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://np.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://za.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://uk.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ck.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://qn.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://nm.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zd.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://ft.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://if.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yr.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tz.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ku.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://in.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ef.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bz.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xo.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ur.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kp.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mb.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pr.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dj.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lj.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zb.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wg.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bf.colortex.cn

[K05] 深拷贝对象
来源：http://ie.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://mw.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://xa.shxzukj.cn

JS:   structuredClone(obj)
来源：http://bn.asd995.cn

TS:   structuredClone(obj)
来源：http://uj.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wg.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://km.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bm.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lk.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://hg.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pv.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ll.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xe.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://po.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ie.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zp.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xx.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qr.asd995.cn

[K07] 进制转换
来源：http://yt.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cm.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ve.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ru.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ky.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dl.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cx.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://va.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ii.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://zf.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://io.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gy.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://hy.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://vs.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zm.jianghongdianzi.cn

Go:   encoding/gob
来源：http://az.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://tg.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://de.bjjhwx.cn

================================================================================
来源：http://qf.jctech888.com.cn

L. 网络请求
来源：http://ob.huixinmuqiang.cn

================================================================================
来源：http://fh.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://fa.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bj.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ae.shxzukj.cn

JS:   await fetch(url)
来源：http://ve.wgjwhj.cn

TS:   await fetch(url)
来源：http://xb.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hs.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://cf.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yg.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://se.hnjuh.cn

[L02] 发送 POST JSON
来源：http://tu.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rd.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hi.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vj.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mb.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kj.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gj.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sb.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ka.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://tk.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rf.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ww.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ta.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ab.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tv.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qv.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kt.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zc.jianghongdianzi.cn

[L04] 设置超时
来源：http://ji.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://cd.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://au.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yh.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tt.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ty.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vb.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tk.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wz.nicolike.cn

[L05] 上传文件（multipart）
来源：http://vf.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zi.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zq.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kf.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ts.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ol.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oi.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kr.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yk.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://vw.huixiangedu.cn

Py:   resp.json()
来源：http://ry.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://xo.newstarts.cn

JS:   await resp.json()
来源：http://om.muxihuayi.cn

TS:   await resp.json()
来源：http://ga.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dd.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vp.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ga.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xv.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://sy.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ch.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ve.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ge.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ua.nszjky.cn

Java: resp.statusCode()
来源：http://tx.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ln.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://cf.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://qh.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://cl.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ut.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://wk.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lf.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jm.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nr.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yq.gzmigu.cn

================================================================================
来源：http://zt.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://kw.521024.cn

================================================================================
来源：http://ym.bjjhwx.cn

[M01] 读取命令行参数
来源：http://cf.shxzukj.cn

Py:   sys.argv[1:]
来源：http://jd.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://xv.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://yk.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://wn.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://oo.chemitech.net.cn

Go:   os.Args[1:]
来源：http://kp.huanxung.cn

Ruby: ARGV
来源：http://iw.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://oj.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ef.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://eg.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oi.shxzskj.cn

JS:   process.env.HOME
来源：http://rw.bookmarksfly.cn

TS:   process.env.HOME
来源：http://bj.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://he.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pd.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://ad.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jw.bookmarksfly.cn

[M03] 执行外部命令
来源：http://zu.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wh.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xx.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vv.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zh.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bk.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://di.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rq.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://kh.asd995.cn

[M04] 获取当前工作目录
来源：http://vn.yuexingan06.cn

Py:   os.getcwd()
来源：http://vm.hahajie.cn

PHP:  getcwd();
来源：http://ob.jianghongdianzi.cn

JS:   process.cwd()
来源：http://hv.yuexingan06.cn

TS:   process.cwd()
来源：http://ap.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://uo.asd995.cn

Go:   os.Getwd()
来源：http://iu.shxzskj.cn

Ruby: Dir.pwd
来源：http://ui.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nj.newstarts.cn

[M05] 设置退出码
来源：http://yx.521024.cn

Py:   sys.exit(1)
来源：http://sd.521024.cn

PHP:  exit(1);
来源：http://db.wgjwhj.cn

JS:   process.exit(1)
来源：http://bg.szxytkj.cn

TS:   process.exit(1)
来源：http://pe.hnjuh.cn

Java: System.exit(1)
来源：http://hi.gzmigu.cn

Go:   os.Exit(1)
来源：http://jt.shxzskj.cn

Ruby: exit 1
来源：http://kb.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ii.gzmigu.cn

[M06] 向标准错误输出
来源：http://je.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://gp.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pf.hnjuh.cn

JS:   console.error("err")
来源：http://gd.haigaiapp.cn

TS:   console.error("err")
来源：http://il.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://sk.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cw.haigaiapp.cn

Ruby: warn "err"
来源：http://kl.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://yn.nszjky.cn

[M07] 判断是否为主入口
来源：http://cy.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://vv.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zb.haigaiapp.cn

JS:   require.main === module
来源：http://ja.huanxung.cn

TS:   require.main === module
来源：http://vg.521024.cn

Java: public static void main(String[] args)
来源：http://rv.9csxet.cn

Go:   func main()
来源：http://vr.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mf.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://la.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://iy.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ht.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://wi.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://nc.nicolike.cn

TS:   process.platform;  process.version
来源：http://as.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://da.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sd.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ye.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ec.panjiajie.cn

================================================================================
来源：http://yb.colortex.cn

N. 数据结构与算法
来源：http://ig.gzmigu.cn

================================================================================
来源：http://qo.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://mj.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dt.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pg.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tt.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hs.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uj.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://vr.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zc.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ez.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://nl.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ti.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rt.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://da.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pt.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://go.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://sr.9csxet.cn

Ruby: arr.sort
来源：http://js.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wd.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://si.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cm.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://wz.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pu.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://la.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bl.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ib.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ol.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://li.lnxyls.cn

[N04] 斐波那契数列
来源：http://vv.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vo.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bo.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gc.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cc.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ig.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zp.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ki.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jt.bookmarksfly.cn

[N05] 最大公约数
来源：http://wb.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://kf.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wv.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sp.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vh.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qt.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bm.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://qs.shxzskj.cn


<!-- 参考信息 -->