代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://lu.newstarts.cn

[J08] 提取年月日与星期
来源：http://qr.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yv.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oa.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aa.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://by.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kz.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wi.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bn.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ss.yuntaijiaju.cn

[J09] 时区处理
来源：http://kw.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xp.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://si.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zq.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nh.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kj.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gd.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qa.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jq.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://ld.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jb.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vv.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gv.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kn.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nj.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bd.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yq.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oi.shtwfgs.cn

================================================================================
来源：http://wg.hnjuh.cn

K. JSON 与序列化
来源：http://cn.shxzukj.cn

================================================================================
来源：http://kz.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://nv.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ji.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bk.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://qf.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://cq.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ak.nicolike.cn

Go:   json.Marshal(obj)
来源：http://of.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dj.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ki.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ux.asd995.cn

Py:   json.loads(s)
来源：http://yc.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dz.newstarts.cn

JS:   JSON.parse(s)
来源：http://ur.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://za.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lw.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://mc.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://qo.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yx.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://dx.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ni.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fr.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aa.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ef.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nv.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://va.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rv.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pr.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://fb.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pl.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wg.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://on.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://py.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wu.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kv.muxihuayi.cn

[K05] 深拷贝对象
来源：http://cd.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://vw.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://ht.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://bn.asd995.cn

TS:   structuredClone(obj)
来源：http://ty.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gl.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sd.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ri.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ty.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://bo.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uw.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gt.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iz.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mh.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lf.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bl.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ui.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jw.huixinmuqiang.cn

[K07] 进制转换
来源：http://jc.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vx.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bo.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fu.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hr.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yj.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pb.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wb.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cf.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://vs.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://qo.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uz.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ig.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ue.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lt.shxzskj.cn

Go:   encoding/gob
来源：http://ck.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://mg.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://re.shxzskj.cn

================================================================================
来源：http://gx.jianghongdianzi.cn

L. 网络请求
来源：http://ki.szsharing.cn

================================================================================
来源：http://ot.nicolike.cn

[L01] 发送 GET 请求
来源：http://aq.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ju.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yx.asd995.cn

JS:   await fetch(url)
来源：http://jf.shxzukj.cn

TS:   await fetch(url)
来源：http://on.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cy.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://fu.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zs.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wr.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://mf.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://au.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oz.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wf.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ta.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kz.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zz.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wp.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pq.szsharing.cn

[L03] 设置自定义请求头
来源：http://bg.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ve.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rh.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tx.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ay.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nm.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nm.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fe.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jv.shtwfgs.cn

[L04] 设置超时
来源：http://nt.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://qh.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ev.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zh.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nt.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yy.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qi.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://et.newstarts.cn

[L05] 上传文件（multipart）
来源：http://ul.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://li.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ts.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lz.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ro.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xq.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dt.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hd.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kq.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://rt.muxihuayi.cn

Py:   resp.json()
来源：http://zv.nicolike.cn

PHP:  json_decode($body, true);
来源：http://cv.wgjwhj.cn

JS:   await resp.json()
来源：http://je.muxihuayi.cn

TS:   await resp.json()
来源：http://fa.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ek.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yo.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://bw.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ee.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://av.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iu.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ja.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://hi.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ja.panjiajie.cn

Java: resp.statusCode()
来源：http://ga.asd995.cn

Go:   resp.StatusCode
来源：http://kv.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ix.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://gk.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://ix.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kv.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://xa.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mo.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fq.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vk.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yg.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ix.asd995.cn

================================================================================
来源：http://fk.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://nb.gzmigu.cn

================================================================================
来源：http://ck.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://na.hnjuh.cn

Py:   sys.argv[1:]
来源：http://mw.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://oz.hahajie.cn

JS:   process.argv.slice(2)
来源：http://ne.hahajie.cn

TS:   process.argv.slice(2)
来源：http://uo.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://pf.521024.cn

Go:   os.Args[1:]
来源：http://rt.chemitech.net.cn

Ruby: ARGV
来源：http://aa.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://sm.asd995.cn

[M02] 读取环境变量
来源：http://ua.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://vi.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kn.jctech888.com.cn

JS:   process.env.HOME
来源：http://lf.nicolike.cn

TS:   process.env.HOME
来源：http://gi.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://wl.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://it.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://aq.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rb.nszjky.cn

[M03] 执行外部命令
来源：http://ve.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rb.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gk.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://en.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yd.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ra.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pk.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ue.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://pz.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://up.muxihuayi.cn

Py:   os.getcwd()
来源：http://ex.nszjky.cn

PHP:  getcwd();
来源：http://xj.yuntaijiaju.cn

JS:   process.cwd()
来源：http://cq.bjjhwx.cn

TS:   process.cwd()
来源：http://yu.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://zb.haigaiapp.cn

Go:   os.Getwd()
来源：http://mv.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ee.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hl.bjjhwx.cn

[M05] 设置退出码
来源：http://or.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://ic.hnjuh.cn

PHP:  exit(1);
来源：http://kw.haigaiapp.cn

JS:   process.exit(1)
来源：http://ml.panjiajie.cn

TS:   process.exit(1)
来源：http://kv.nszjky.cn

Java: System.exit(1)
来源：http://ta.chemitech.net.cn

Go:   os.Exit(1)
来源：http://in.szsharing.cn

Ruby: exit 1
来源：http://ug.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fa.chemitech.net.cn

[M06] 向标准错误输出
来源：http://xi.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://bw.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://td.haigaiapp.cn

JS:   console.error("err")
来源：http://af.chemitech.net.cn

TS:   console.error("err")
来源：http://la.lnxyls.cn

Java: System.err.println("err")
来源：http://es.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pl.haigaiapp.cn

Ruby: warn "err"
来源：http://sy.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://jz.szxytkj.cn

[M07] 判断是否为主入口
来源：http://hi.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://ni.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ka.bjjhwx.cn

JS:   require.main === module
来源：http://ci.szsharing.cn

TS:   require.main === module
来源：http://si.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://we.bookmarksfly.cn

Go:   func main()
来源：http://ii.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ox.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://od.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://gw.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://ln.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://la.szxytkj.cn

JS:   process.platform;  process.version
来源：http://wl.9csxet.cn

TS:   process.platform;  process.version
来源：http://qn.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ks.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uv.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lk.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ki.nicolike.cn

================================================================================
来源：http://gk.521024.cn

N. 数据结构与算法
来源：http://zq.hahajie.cn

================================================================================
来源：http://hv.colortex.cn

[N01] 二分查找（有序数组）
来源：http://ci.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kj.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rw.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eb.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ns.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ax.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://fv.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://du.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mx.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bi.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://hg.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://va.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cp.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://no.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://le.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://hw.asd995.cn

Ruby: arr.sort
来源：http://oy.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wv.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://qq.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gk.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://db.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jk.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rm.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://za.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://up.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qd.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bq.huanxung.cn

[N04] 斐波那契数列
来源：http://ea.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qe.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hn.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zp.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sy.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yv.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vd.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sn.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hf.colortex.cn

[N05] 最大公约数
来源：http://fs.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ct.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gr.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ki.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://td.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qf.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://am.newstarts.cn

Ruby: a.gcd(b)
来源：http://kt.szsharing.cn


<!-- 参考信息 -->