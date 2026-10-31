代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://wf.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ee.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yr.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wo.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wc.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ib.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yj.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kd.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eo.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mc.newstarts.cn

[J09] 时区处理
来源：http://vg.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rx.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xq.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dv.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cl.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ew.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mq.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ax.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kp.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://si.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rv.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wf.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qb.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ji.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xt.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ch.bjjhwx.cn

================================================================================
来源：http://lf.hnjuh.cn

K. JSON 与序列化
来源：http://cc.gzmigu.cn

================================================================================
来源：http://sr.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://kz.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yx.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tu.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://km.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://kz.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kv.nszjky.cn

Go:   json.Marshal(obj)
来源：http://pn.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://af.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nm.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://fl.szsharing.cn

Py:   json.loads(s)
来源：http://ka.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gy.hnjuh.cn

JS:   JSON.parse(s)
来源：http://yb.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://wi.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zi.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://di.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://ak.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xg.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://nq.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://em.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mg.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ak.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qi.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ft.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://da.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zw.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zl.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://vg.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mo.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qn.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nk.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ow.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gu.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gq.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ep.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ho.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://dc.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://ao.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://qu.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://ux.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://zf.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hm.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iv.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yb.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pv.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://pk.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gb.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ll.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tx.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tq.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rv.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ye.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vy.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jm.muxihuayi.cn

[K07] 进制转换
来源：http://wh.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://an.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pe.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ec.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://on.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uo.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wp.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lr.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://tk.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://el.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://my.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://zf.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ek.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zw.szxytkj.cn

Go:   encoding/gob
来源：http://gd.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://gc.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://te.szxytkj.cn

================================================================================
来源：http://mv.gzmigu.cn

L. 网络请求
来源：http://cj.muxihuayi.cn

================================================================================
来源：http://qp.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ii.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nq.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qd.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://rp.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://lc.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iv.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ae.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uf.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hq.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://od.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wb.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://it.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bl.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hu.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lh.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ti.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://ct.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cx.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wa.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wl.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ci.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gy.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pv.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ej.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ww.jianghongdianzi.cn

[L04] 设置超时
来源：http://ht.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://wv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nu.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xl.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qw.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rb.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qf.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ja.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dc.huanxung.cn

[L05] 上传文件（multipart）
来源：http://wq.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://op.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hy.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nn.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bs.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uf.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ay.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bd.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://av.colortex.cn

Py:   resp.json()
来源：http://ig.newstarts.cn

PHP:  json_decode($body, true);
来源：http://pr.yuexingan06.cn

JS:   await resp.json()
来源：http://ao.lnxyls.cn

TS:   await resp.json()
来源：http://mc.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gl.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uv.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ew.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ky.521024.cn

[L07] 处理 HTTP 状态码
来源：http://rp.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qk.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mp.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://fm.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://tq.bookmarksfly.cn

Java: resp.statusCode()
来源：http://cy.shtwfgs.cn

Go:   resp.StatusCode
来源：http://mr.huanxung.cn

Ruby: resp.code.to_i
来源：http://hm.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://iv.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ol.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yn.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://km.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mb.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sz.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://un.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vk.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ll.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zf.hahajie.cn

================================================================================
来源：http://yn.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://ms.huixiangedu.cn

================================================================================
来源：http://ba.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ri.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://um.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://hl.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://tk.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://np.521024.cn

Java: args 数组（main 方法参数）
来源：http://os.newstarts.cn

Go:   os.Args[1:]
来源：http://qk.bookmarksfly.cn

Ruby: ARGV
来源：http://gz.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://cf.nicolike.cn

[M02] 读取环境变量
来源：http://ig.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://gs.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://go.muxihuayi.cn

JS:   process.env.HOME
来源：http://xw.shxzukj.cn

TS:   process.env.HOME
来源：http://nq.lnxyls.cn

Java: System.getenv("HOME")
来源：http://sp.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mt.9csxet.cn

Ruby: ENV["HOME"]
来源：http://di.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tg.huixiangedu.cn

[M03] 执行外部命令
来源：http://ca.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lw.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kv.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wj.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vg.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nr.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gk.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oj.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://lf.asd995.cn

[M04] 获取当前工作目录
来源：http://nu.nicolike.cn

Py:   os.getcwd()
来源：http://gg.hnjuh.cn

PHP:  getcwd();
来源：http://tq.nicolike.cn

JS:   process.cwd()
来源：http://ab.panjiajie.cn

TS:   process.cwd()
来源：http://xs.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://qr.colortex.cn

Go:   os.Getwd()
来源：http://ep.jctech888.com.cn

Ruby: Dir.pwd
来源：http://lw.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fq.521024.cn

[M05] 设置退出码
来源：http://hc.panjiajie.cn

Py:   sys.exit(1)
来源：http://ag.jctech888.com.cn

PHP:  exit(1);
来源：http://am.nicolike.cn

JS:   process.exit(1)
来源：http://it.haigaiapp.cn

TS:   process.exit(1)
来源：http://vl.huixinmuqiang.cn

Java: System.exit(1)
来源：http://yi.haigaiapp.cn

Go:   os.Exit(1)
来源：http://rk.huanxung.cn

Ruby: exit 1
来源：http://ro.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qv.nicolike.cn

[M06] 向标准错误输出
来源：http://ta.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://cu.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aw.muxihuayi.cn

JS:   console.error("err")
来源：http://wz.shxzskj.cn

TS:   console.error("err")
来源：http://hw.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://cn.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.yuntaijiaju.cn

Ruby: warn "err"
来源：http://re.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://rq.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://cn.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://bc.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://va.colortex.cn

JS:   require.main === module
来源：http://sh.wgjwhj.cn

TS:   require.main === module
来源：http://lg.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://op.wgjwhj.cn

Go:   func main()
来源：http://nc.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nw.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://vg.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://hg.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://wd.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ro.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://cf.szsharing.cn

TS:   process.platform;  process.version
来源：http://aq.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nx.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qq.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yp.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qr.nszjky.cn

================================================================================
来源：http://zm.muxihuayi.cn

N. 数据结构与算法
来源：http://wx.bookmarksfly.cn

================================================================================
来源：http://sk.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://dm.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kr.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ik.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fa.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gy.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bs.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ca.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yk.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jm.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://rv.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://gw.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ex.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://im.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://su.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://km.hahajie.cn

Go:   slices.Sort(arr)
来源：http://ws.wgjwhj.cn

Ruby: arr.sort
来源：http://il.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gz.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://up.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mg.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ru.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ch.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zb.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mn.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://id.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://la.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://em.9csxet.cn

[N04] 斐波那契数列
来源：http://ge.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oi.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ci.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bq.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hu.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bi.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rr.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rl.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://od.nicolike.cn

[N05] 最大公约数
来源：http://jy.colortex.cn

Py:   math.gcd(a, b)
来源：http://lb.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vy.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sq.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zr.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ny.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://km.9csxet.cn

Ruby: a.gcd(b)
来源：http://vz.chemitech.net.cn


<!-- 参考信息 -->