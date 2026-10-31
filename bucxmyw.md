代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://kr.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://dw.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lb.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kq.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ud.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hn.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dv.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uo.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vh.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://md.muxihuayi.cn

[J09] 时区处理
来源：http://pi.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wl.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fr.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ct.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mq.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ay.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bz.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ci.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bj.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://xe.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xa.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wc.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sw.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ke.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lm.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fk.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mk.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gd.hnjuh.cn

================================================================================
来源：http://dz.shtwfgs.cn

K. JSON 与序列化
来源：http://jr.huanxung.cn

================================================================================
来源：http://py.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://hl.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bq.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yt.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ij.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://or.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gt.newstarts.cn

Go:   json.Marshal(obj)
来源：http://sm.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oj.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nw.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://qv.hahajie.cn

Py:   json.loads(s)
来源：http://cl.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vm.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ex.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://ix.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fw.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://hh.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://rf.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pp.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://km.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://be.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tz.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rl.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ly.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ul.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kp.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ot.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tw.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://xs.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zj.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uz.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ac.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vq.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ah.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tr.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mh.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vm.wgjwhj.cn

[K05] 深拷贝对象
来源：http://pp.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://zz.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://wq.shxzskj.cn

JS:   structuredClone(obj)
来源：http://gx.colortex.cn

TS:   structuredClone(obj)
来源：http://mg.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qg.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hs.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xq.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yf.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://zu.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cw.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gx.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vx.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ex.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ba.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pn.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dw.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ha.9csxet.cn

[K07] 进制转换
来源：http://tr.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hg.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ha.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ta.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mm.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ra.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cw.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ir.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jx.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://os.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://rz.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dh.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://oi.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://nz.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aq.521024.cn

Go:   encoding/gob
来源：http://oq.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://cu.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://di.shxzskj.cn

================================================================================
来源：http://le.shtwfgs.cn

L. 网络请求
来源：http://ak.szxytkj.cn

================================================================================
来源：http://tx.521024.cn

[L01] 发送 GET 请求
来源：http://we.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qf.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nf.shtwfgs.cn

JS:   await fetch(url)
来源：http://sc.huixiangedu.cn

TS:   await fetch(url)
来源：http://bu.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ob.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://wk.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nd.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yk.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://xu.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jg.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qg.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sm.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bv.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sh.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ue.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dz.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ze.panjiajie.cn

[L03] 设置自定义请求头
来源：http://fw.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dh.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mi.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cu.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rr.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yy.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wv.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wu.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uq.bjjhwx.cn

[L04] 设置超时
来源：http://no.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://vy.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fw.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aa.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://om.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ee.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ys.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yr.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ex.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://ws.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dt.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zy.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cb.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ai.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hs.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oo.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ak.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gz.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://wp.bookmarksfly.cn

Py:   resp.json()
来源：http://os.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://le.asd995.cn

JS:   await resp.json()
来源：http://ij.jctech888.com.cn

TS:   await resp.json()
来源：http://ug.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oh.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://le.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://il.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ve.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://na.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ku.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ra.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://dx.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://bx.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://sw.huanxung.cn

Go:   resp.StatusCode
来源：http://rj.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://fh.521024.cn

C#:   (int)resp.StatusCode
来源：http://jn.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://ce.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bq.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://pz.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://er.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://er.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://er.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://te.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yj.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gi.9csxet.cn

================================================================================
来源：http://ie.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://zc.lnxyls.cn

================================================================================
来源：http://ei.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ob.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://sn.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://zu.huanxung.cn

JS:   process.argv.slice(2)
来源：http://vs.521024.cn

TS:   process.argv.slice(2)
来源：http://yu.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://oe.bjjhwx.cn

Go:   os.Args[1:]
来源：http://on.nszjky.cn

Ruby: ARGV
来源：http://yi.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://mf.newstarts.cn

[M02] 读取环境变量
来源：http://rs.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://fc.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yw.shxzskj.cn

JS:   process.env.HOME
来源：http://le.shxzskj.cn

TS:   process.env.HOME
来源：http://ry.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://xx.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yg.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://kc.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ey.panjiajie.cn

[M03] 执行外部命令
来源：http://io.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lk.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mm.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nb.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pp.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ov.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://re.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rg.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://si.panjiajie.cn

[M04] 获取当前工作目录
来源：http://tf.yuexingan06.cn

Py:   os.getcwd()
来源：http://hf.yuntaijiaju.cn

PHP:  getcwd();
来源：http://tv.nicolike.cn

JS:   process.cwd()
来源：http://dc.haigaiapp.cn

TS:   process.cwd()
来源：http://lv.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ht.wgjwhj.cn

Go:   os.Getwd()
来源：http://tf.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://qj.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zm.muxihuayi.cn

[M05] 设置退出码
来源：http://xc.jctech888.com.cn

Py:   sys.exit(1)
来源：http://yp.hahajie.cn

PHP:  exit(1);
来源：http://qp.shxzukj.cn

JS:   process.exit(1)
来源：http://pr.jctech888.com.cn

TS:   process.exit(1)
来源：http://yy.muxihuayi.cn

Java: System.exit(1)
来源：http://eb.9csxet.cn

Go:   os.Exit(1)
来源：http://ib.asd995.cn

Ruby: exit 1
来源：http://na.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iu.szxytkj.cn

[M06] 向标准错误输出
来源：http://wy.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://ct.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oq.chemitech.net.cn

JS:   console.error("err")
来源：http://rx.muxihuayi.cn

TS:   console.error("err")
来源：http://bu.szxytkj.cn

Java: System.err.println("err")
来源：http://fa.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zd.huixinmuqiang.cn

Ruby: warn "err"
来源：http://ke.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://on.newstarts.cn

[M07] 判断是否为主入口
来源：http://pz.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://el.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://co.yuexingan06.cn

JS:   require.main === module
来源：http://ub.shxzskj.cn

TS:   require.main === module
来源：http://pj.newstarts.cn

Java: public static void main(String[] args)
来源：http://hm.yuexingan06.cn

Go:   func main()
来源：http://bf.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xn.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ke.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://hy.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://qe.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://lk.9csxet.cn

JS:   process.platform;  process.version
来源：http://bv.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://tv.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sr.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cy.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://os.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mm.bookmarksfly.cn

================================================================================
来源：http://th.huanxung.cn

N. 数据结构与算法
来源：http://hi.hahajie.cn

================================================================================
来源：http://gf.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://cr.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ic.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nu.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rr.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sr.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cs.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://ym.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qk.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hm.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://sy.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lh.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nw.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kk.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gv.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://hj.huixiangedu.cn

Ruby: arr.sort
来源：http://ed.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bj.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://ic.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nn.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://xw.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ne.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ac.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://of.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tv.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fn.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iw.wgjwhj.cn

[N04] 斐波那契数列
来源：http://vl.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sb.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lr.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dv.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://va.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gf.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dq.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ga.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uk.yuexingan06.cn

[N05] 最大公约数
来源：http://rn.521024.cn

Py:   math.gcd(a, b)
来源：http://qf.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bi.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tb.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pv.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ei.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rq.newstarts.cn

Ruby: a.gcd(b)
来源：http://ia.bookmarksfly.cn


<!-- 参考信息 -->