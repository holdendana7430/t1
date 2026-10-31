代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://vb.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ti.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qb.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fr.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://on.colortex.cn

[J08] 提取年月日与星期
来源：http://gz.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wx.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rv.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wi.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mp.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cp.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bv.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ry.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mp.nszjky.cn

[J09] 时区处理
来源：http://xy.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xo.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ra.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jf.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ep.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sl.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sz.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://bc.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ki.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qv.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ng.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kx.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aq.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dr.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jg.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fj.newstarts.cn

================================================================================
来源：http://sb.yuexingan06.cn

K. JSON 与序列化
来源：http://hz.nicolike.cn

================================================================================
来源：http://em.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://dn.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cu.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dx.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://wa.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://nn.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yo.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://wk.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hi.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://xu.gzmigu.cn

Py:   json.loads(s)
来源：http://gm.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://az.panjiajie.cn

JS:   JSON.parse(s)
来源：http://yx.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ny.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://li.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://hj.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://hn.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mm.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://rb.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cv.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cq.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vt.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ug.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dg.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ff.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zx.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nw.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://th.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mr.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fa.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yy.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dw.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nb.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bx.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://we.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nt.haigaiapp.cn

[K05] 深拷贝对象
来源：http://bb.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://tg.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://if.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://kq.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://mo.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ow.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://un.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sm.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tn.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://hh.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ji.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ha.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xx.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qy.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ev.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hl.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tl.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mv.shxzukj.cn

[K07] 进制转换
来源：http://ei.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lf.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wf.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vu.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qq.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fr.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ay.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sx.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uo.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://on.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://cl.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yb.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://th.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://no.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kz.521024.cn

Go:   encoding/gob
来源：http://nv.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://xr.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lw.yuexingan06.cn

================================================================================
来源：http://zv.newstarts.cn

L. 网络请求
来源：http://kr.jianghongdianzi.cn

================================================================================
来源：http://zn.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://gs.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bs.colortex.cn

JS:   await fetch(url)
来源：http://zq.bjjhwx.cn

TS:   await fetch(url)
来源：http://ki.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qt.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://yf.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nm.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://gg.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yt.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kc.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mp.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://su.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ho.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pu.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hj.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://am.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://wo.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fk.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tf.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gi.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://to.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nk.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lx.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://um.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gw.hnjuh.cn

[L04] 设置超时
来源：http://wd.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ia.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eo.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tc.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sf.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://en.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ql.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kx.colortex.cn

[L05] 上传文件（multipart）
来源：http://cq.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ej.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mj.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fu.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://es.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zr.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ib.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lu.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ip.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://tf.muxihuayi.cn

Py:   resp.json()
来源：http://oz.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://ji.panjiajie.cn

JS:   await resp.json()
来源：http://me.huixiangedu.cn

TS:   await resp.json()
来源：http://pd.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dq.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ms.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://fj.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ak.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://qs.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kf.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gr.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://lf.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://do.hnjuh.cn

Java: resp.statusCode()
来源：http://hs.9csxet.cn

Go:   resp.StatusCode
来源：http://ux.colortex.cn

Ruby: resp.code.to_i
来源：http://ct.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://op.521024.cn

[L08] 并发请求多个地址
来源：http://rq.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tl.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://mt.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yx.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xk.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yd.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://th.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gy.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://el.muxihuayi.cn

================================================================================
来源：http://yq.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ek.hahajie.cn

================================================================================
来源：http://su.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://gq.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://pl.asd995.cn

PHP:  $argv;  $argc;
来源：http://pl.nicolike.cn

JS:   process.argv.slice(2)
来源：http://oi.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ti.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ub.colortex.cn

Go:   os.Args[1:]
来源：http://gn.muxihuayi.cn

Ruby: ARGV
来源：http://rf.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://sp.9csxet.cn

[M02] 读取环境变量
来源：http://ig.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://sf.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nf.9csxet.cn

JS:   process.env.HOME
来源：http://be.colortex.cn

TS:   process.env.HOME
来源：http://nk.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://wm.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dj.newstarts.cn

Ruby: ENV["HOME"]
来源：http://wk.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nd.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://kv.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://be.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iz.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qh.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yq.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iv.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ji.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ml.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://ir.asd995.cn

[M04] 获取当前工作目录
来源：http://wi.wgjwhj.cn

Py:   os.getcwd()
来源：http://bi.haigaiapp.cn

PHP:  getcwd();
来源：http://ag.lnxyls.cn

JS:   process.cwd()
来源：http://sq.hahajie.cn

TS:   process.cwd()
来源：http://gc.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://qd.9csxet.cn

Go:   os.Getwd()
来源：http://in.panjiajie.cn

Ruby: Dir.pwd
来源：http://ma.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ao.szsharing.cn

[M05] 设置退出码
来源：http://px.lnxyls.cn

Py:   sys.exit(1)
来源：http://zy.hnjuh.cn

PHP:  exit(1);
来源：http://jy.521024.cn

JS:   process.exit(1)
来源：http://oe.bookmarksfly.cn

TS:   process.exit(1)
来源：http://qm.panjiajie.cn

Java: System.exit(1)
来源：http://yo.asd995.cn

Go:   os.Exit(1)
来源：http://jn.jctech888.com.cn

Ruby: exit 1
来源：http://bu.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qz.gzmigu.cn

[M06] 向标准错误输出
来源：http://qp.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://yz.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kw.panjiajie.cn

JS:   console.error("err")
来源：http://ij.szsharing.cn

TS:   console.error("err")
来源：http://on.wgjwhj.cn

Java: System.err.println("err")
来源：http://gr.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iy.muxihuayi.cn

Ruby: warn "err"
来源：http://uw.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ei.gzmigu.cn

[M07] 判断是否为主入口
来源：http://jv.521024.cn

Py:   if __name__ == "__main__":
来源：http://ng.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kp.jianghongdianzi.cn

JS:   require.main === module
来源：http://oy.jctech888.com.cn

TS:   require.main === module
来源：http://is.hnjuh.cn

Java: public static void main(String[] args)
来源：http://oh.bookmarksfly.cn

Go:   func main()
来源：http://xa.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wt.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://qw.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://br.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://db.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://aw.gzmigu.cn

JS:   process.platform;  process.version
来源：http://mh.lnxyls.cn

TS:   process.platform;  process.version
来源：http://aa.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ge.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wx.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kh.nszjky.cn

================================================================================
来源：http://qd.gzmigu.cn

N. 数据结构与算法
来源：http://bk.yuexingan06.cn

================================================================================
来源：http://hx.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://ce.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ou.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xv.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ma.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sq.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jw.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://lj.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aa.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kp.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://nm.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ij.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rf.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lo.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zb.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sz.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://ov.nicolike.cn

Ruby: arr.sort
来源：http://il.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ll.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ja.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qa.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://te.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zo.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ml.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://na.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gn.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nu.gzmigu.cn

[N04] 斐波那契数列
来源：http://mi.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vt.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ir.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tk.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jk.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qm.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ec.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bc.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tc.9csxet.cn

[N05] 最大公约数
来源：http://fq.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ct.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sg.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zr.hahajie.cn


<!-- 参考信息 -->