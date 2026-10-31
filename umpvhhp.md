代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xk.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gd.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pg.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vs.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wo.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zl.bookmarksfly.cn

[J09] 时区处理
来源：http://zw.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ak.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ur.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bo.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ak.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vy.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jh.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hw.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sz.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://hd.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dq.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ic.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zu.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sn.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ag.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bx.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bd.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fc.colortex.cn

================================================================================
来源：http://zw.huixinmuqiang.cn

K. JSON 与序列化
来源：http://vu.nicolike.cn

================================================================================
来源：http://aa.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://gq.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wz.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ub.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://xa.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://vw.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ss.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://qn.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sw.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hf.szsharing.cn

[K02] JSON 字符串转对象
来源：http://wh.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ju.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dw.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://mr.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://oq.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ih.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://fs.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://is.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://an.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://jw.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jp.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kh.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kd.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sv.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ic.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hr.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aq.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ce.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://cm.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ep.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://du.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uz.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ec.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://en.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vt.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aw.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zu.huanxung.cn

[K05] 深拷贝对象
来源：http://az.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://bp.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://jz.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://xt.shxzskj.cn

TS:   structuredClone(obj)
来源：http://as.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yq.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pq.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bq.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kv.asd995.cn

[K06] 解析 URL 查询串
来源：http://sg.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jb.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tl.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hp.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cq.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ub.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gd.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fk.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mz.bjjhwx.cn

[K07] 进制转换
来源：http://qy.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xb.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eq.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pk.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gh.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ma.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pw.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fr.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kd.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://pi.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://pq.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ok.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://wt.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://sq.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://om.bookmarksfly.cn

Go:   encoding/gob
来源：http://nx.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://wi.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://da.chemitech.net.cn

================================================================================
来源：http://fs.newstarts.cn

L. 网络请求
来源：http://sa.9csxet.cn

================================================================================
来源：http://jw.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ba.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gd.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ey.huixiangedu.cn

JS:   await fetch(url)
来源：http://qx.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://di.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ka.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ju.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sr.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fo.szsharing.cn

[L02] 发送 POST JSON
来源：http://pr.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ru.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cd.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vn.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uq.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fh.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ip.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://th.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xh.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://vy.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vc.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zr.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ls.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oc.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://az.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yf.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oi.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ej.wgjwhj.cn

[L04] 设置超时
来源：http://vv.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://lt.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pi.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fs.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ar.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bq.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fn.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yg.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pl.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ly.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mw.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tb.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ns.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uc.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yo.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kv.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gr.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kf.huanxung.cn

[L06] 解析响应为 JSON
来源：http://gp.yuexingan06.cn

Py:   resp.json()
来源：http://xr.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://yv.chemitech.net.cn

JS:   await resp.json()
来源：http://dt.hahajie.cn

TS:   await resp.json()
来源：http://cw.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mf.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zn.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://yr.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xy.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://gr.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aq.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xg.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://sr.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ox.jctech888.com.cn

Java: resp.statusCode()
来源：http://yy.jctech888.com.cn

Go:   resp.StatusCode
来源：http://pj.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://ww.asd995.cn

C#:   (int)resp.StatusCode
来源：http://ug.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://rq.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wq.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://nb.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zg.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://os.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zu.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nu.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eh.colortex.cn

================================================================================
来源：http://fe.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://zy.szsharing.cn

================================================================================
来源：http://xh.muxihuayi.cn

[M01] 读取命令行参数
来源：http://hl.newstarts.cn

Py:   sys.argv[1:]
来源：http://ng.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://mh.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://mm.hahajie.cn

TS:   process.argv.slice(2)
来源：http://hm.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://eb.shxzskj.cn

Go:   os.Args[1:]
来源：http://gk.9csxet.cn

Ruby: ARGV
来源：http://ay.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://zj.bookmarksfly.cn

[M02] 读取环境变量
来源：http://vj.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://jd.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pz.huanxung.cn

JS:   process.env.HOME
来源：http://di.colortex.cn

TS:   process.env.HOME
来源：http://vs.newstarts.cn

Java: System.getenv("HOME")
来源：http://ji.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vl.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://jm.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eb.hahajie.cn

[M03] 执行外部命令
来源：http://uf.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bd.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kd.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bi.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xo.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nk.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ar.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ap.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://pi.9csxet.cn

[M04] 获取当前工作目录
来源：http://na.bjjhwx.cn

Py:   os.getcwd()
来源：http://en.9csxet.cn

PHP:  getcwd();
来源：http://qn.jianghongdianzi.cn

JS:   process.cwd()
来源：http://ci.jctech888.com.cn

TS:   process.cwd()
来源：http://do.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://tx.szsharing.cn

Go:   os.Getwd()
来源：http://aa.lnxyls.cn

Ruby: Dir.pwd
来源：http://kp.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wk.shxzskj.cn

[M05] 设置退出码
来源：http://bg.gzmigu.cn

Py:   sys.exit(1)
来源：http://mx.asd995.cn

PHP:  exit(1);
来源：http://ey.gzmigu.cn

JS:   process.exit(1)
来源：http://ss.muxihuayi.cn

TS:   process.exit(1)
来源：http://in.huixinmuqiang.cn

Java: System.exit(1)
来源：http://lt.nszjky.cn

Go:   os.Exit(1)
来源：http://cp.9csxet.cn

Ruby: exit 1
来源：http://sg.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hm.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ch.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://ix.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xl.yuexingan06.cn

JS:   console.error("err")
来源：http://ds.szxytkj.cn

TS:   console.error("err")
来源：http://jz.muxihuayi.cn

Java: System.err.println("err")
来源：http://qz.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lo.jianghongdianzi.cn

Ruby: warn "err"
来源：http://ys.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ea.szsharing.cn

[M07] 判断是否为主入口
来源：http://kw.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://rv.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ep.panjiajie.cn

JS:   require.main === module
来源：http://on.huixinmuqiang.cn

TS:   require.main === module
来源：http://xj.newstarts.cn

Java: public static void main(String[] args)
来源：http://cq.huixiangedu.cn

Go:   func main()
来源：http://ez.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fs.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://ua.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://qk.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://fd.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://st.panjiajie.cn

JS:   process.platform;  process.version
来源：http://es.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://bq.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ee.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pv.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ob.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gc.shtwfgs.cn

================================================================================
来源：http://xm.asd995.cn

N. 数据结构与算法
来源：http://gi.szxytkj.cn

================================================================================
来源：http://pp.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://mi.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ym.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cw.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sb.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hn.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://du.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://js.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wl.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fs.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://gn.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://nd.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gk.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gb.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tn.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xo.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://al.nszjky.cn

Ruby: arr.sort
来源：http://tj.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dc.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://tt.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lv.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://xr.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hc.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ib.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ri.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pj.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kn.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tq.shxzukj.cn

[N04] 斐波那契数列
来源：http://rv.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cs.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uz.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cc.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cz.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bu.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://io.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://co.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jt.chemitech.net.cn

[N05] 最大公约数
来源：http://xv.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://pk.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zl.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ah.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ln.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qi.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://il.521024.cn

Ruby: a.gcd(b)
来源：http://hm.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yf.shxzukj.cn

[N06] 判断回文字符串
来源：http://je.muxihuayi.cn

Py:   s == s[::-1]
来源：http://pm.asd995.cn

PHP:  $s === strrev($s);
来源：http://ev.huixinmuqiang.cn


<!-- 参考信息 -->