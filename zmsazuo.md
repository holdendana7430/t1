代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://ac.521024.cn

[J08] 提取年月日与星期
来源：http://az.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cq.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://de.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mg.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://os.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rj.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dd.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mt.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dv.szxytkj.cn

[J09] 时区处理
来源：http://ew.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rj.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://na.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dz.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jf.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://et.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bh.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://db.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ip.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://il.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dt.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://my.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xb.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lu.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nz.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ys.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cn.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sz.hnjuh.cn

================================================================================
来源：http://fd.haigaiapp.cn

K. JSON 与序列化
来源：http://ga.newstarts.cn

================================================================================
来源：http://tr.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ru.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sc.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ek.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://jd.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ha.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gb.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://rs.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aw.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://di.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ay.colortex.cn

Py:   json.loads(s)
来源：http://ux.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wi.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://fr.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://eh.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zf.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://nw.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://oe.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://er.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://wq.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kx.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yr.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ld.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lu.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ld.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zi.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xk.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hv.newstarts.cn

[K04] 读取 JSON 文件
来源：http://hb.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ng.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ug.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://da.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mm.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ee.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zb.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eo.huanxung.cn

[K05] 深拷贝对象
来源：http://tr.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://qx.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://ic.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://uf.newstarts.cn

TS:   structuredClone(obj)
来源：http://pc.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vx.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://js.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ja.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uk.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://lq.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://am.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pz.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vh.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ox.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bi.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ol.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vl.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yg.nicolike.cn

[K07] 进制转换
来源：http://ld.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pk.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dn.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ya.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hc.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mu.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://of.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://px.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wo.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://te.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://rz.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mz.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://oj.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://aj.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uo.bookmarksfly.cn

Go:   encoding/gob
来源：http://om.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://pl.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uu.nszjky.cn

================================================================================
来源：http://hd.bjjhwx.cn

L. 网络请求
来源：http://zx.nicolike.cn

================================================================================
来源：http://qs.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://rm.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sv.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sj.szsharing.cn

JS:   await fetch(url)
来源：http://be.nicolike.cn

TS:   await fetch(url)
来源：http://pw.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qc.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://fs.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dc.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ja.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://cn.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gs.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wo.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wx.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://co.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fp.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ey.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ay.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xg.newstarts.cn

[L03] 设置自定义请求头
来源：http://za.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kq.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jd.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rw.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wj.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nu.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jk.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vj.szxytkj.cn

[L04] 设置超时
来源：http://dv.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://jz.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bb.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://su.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ul.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gc.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oa.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wv.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tj.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://wq.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aq.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ty.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lz.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fy.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xt.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pw.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zx.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://rt.bjjhwx.cn

Py:   resp.json()
来源：http://de.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://st.szxytkj.cn

JS:   await resp.json()
来源：http://uw.huixiangedu.cn

TS:   await resp.json()
来源：http://at.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iq.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ow.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://pg.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bg.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://hi.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://er.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ys.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://fb.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://ov.panjiajie.cn

Java: resp.statusCode()
来源：http://mq.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://nz.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://tb.asd995.cn

C#:   (int)resp.StatusCode
来源：http://qh.szxytkj.cn

[L08] 并发请求多个地址
来源：http://hh.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sl.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://sq.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bd.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://to.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://st.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fr.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lu.bookmarksfly.cn

================================================================================
来源：http://ak.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://pn.chemitech.net.cn

================================================================================
来源：http://eo.nszjky.cn

[M01] 读取命令行参数
来源：http://hc.hahajie.cn

Py:   sys.argv[1:]
来源：http://cd.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://iz.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://zt.szsharing.cn

TS:   process.argv.slice(2)
来源：http://ge.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://ub.521024.cn

Go:   os.Args[1:]
来源：http://bb.gzmigu.cn

Ruby: ARGV
来源：http://gv.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://as.jctech888.com.cn

[M02] 读取环境变量
来源：http://zu.colortex.cn

Py:   os.environ.get("HOME")
来源：http://dv.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nb.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://uc.newstarts.cn

TS:   process.env.HOME
来源：http://xj.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://cu.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gf.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://of.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://df.9csxet.cn

[M03] 执行外部命令
来源：http://lr.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hb.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yd.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://za.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ug.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zu.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lg.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://va.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://vk.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://zf.colortex.cn

Py:   os.getcwd()
来源：http://na.asd995.cn

PHP:  getcwd();
来源：http://id.9csxet.cn

JS:   process.cwd()
来源：http://lc.bjjhwx.cn

TS:   process.cwd()
来源：http://va.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://vz.jctech888.com.cn

Go:   os.Getwd()
来源：http://ap.bjjhwx.cn

Ruby: Dir.pwd
来源：http://qk.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nr.asd995.cn

[M05] 设置退出码
来源：http://sl.hnjuh.cn

Py:   sys.exit(1)
来源：http://au.bookmarksfly.cn

PHP:  exit(1);
来源：http://xn.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://za.hahajie.cn

TS:   process.exit(1)
来源：http://wi.shxzskj.cn

Java: System.exit(1)
来源：http://zb.gzmigu.cn

Go:   os.Exit(1)
来源：http://tj.jianghongdianzi.cn

Ruby: exit 1
来源：http://ad.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ed.shtwfgs.cn

[M06] 向标准错误输出
来源：http://rm.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ve.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cg.shtwfgs.cn

JS:   console.error("err")
来源：http://zi.lnxyls.cn

TS:   console.error("err")
来源：http://ou.hnjuh.cn

Java: System.err.println("err")
来源：http://ce.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gj.gzmigu.cn

Ruby: warn "err"
来源：http://po.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vx.huanxung.cn

[M07] 判断是否为主入口
来源：http://vu.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://ch.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pm.newstarts.cn

JS:   require.main === module
来源：http://ow.colortex.cn

TS:   require.main === module
来源：http://zr.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://fq.huixiangedu.cn

Go:   func main()
来源：http://pb.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bf.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ue.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://og.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://kl.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://et.szxytkj.cn

JS:   process.platform;  process.version
来源：http://qt.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://nj.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zc.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ug.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ym.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qi.nicolike.cn

================================================================================
来源：http://zc.nicolike.cn

N. 数据结构与算法
来源：http://ct.wgjwhj.cn

================================================================================
来源：http://cr.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://wu.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gn.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dw.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ah.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gv.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://bu.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eo.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://th.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://jw.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://yx.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kr.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gu.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ht.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qc.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ig.haigaiapp.cn

Ruby: arr.sort
来源：http://fe.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kd.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://pk.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wl.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://qw.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kt.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yh.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lv.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://on.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tw.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://bu.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jp.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fm.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jd.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hq.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dv.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rw.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uk.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://du.yuexingan06.cn

[N05] 最大公约数
来源：http://zh.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://qy.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ll.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jk.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ar.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hk.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vt.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://qq.wgjwhj.cn


<!-- 参考信息 -->