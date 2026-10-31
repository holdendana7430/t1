代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://lu.shxzukj.cn

[J08] 提取年月日与星期
来源：http://eb.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pf.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kc.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ij.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gv.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nx.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qj.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sw.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lo.shxzukj.cn

[J09] 时区处理
来源：http://bj.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uh.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jv.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://he.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yt.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://km.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wh.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qo.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://gw.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mp.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cl.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ec.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kj.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xk.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gn.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qu.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yk.panjiajie.cn

================================================================================
来源：http://pc.shxzskj.cn

K. JSON 与序列化
来源：http://el.asd995.cn

================================================================================
来源：http://sj.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://xk.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dc.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fz.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://qw.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://oe.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nk.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://rn.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nh.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jj.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://or.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://dk.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ho.shxzukj.cn

JS:   JSON.parse(s)
来源：http://jc.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://oh.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gg.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://au.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://qz.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ct.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ck.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ng.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yy.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mb.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vx.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zh.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://km.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lb.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://al.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://fx.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bn.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sn.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ei.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xq.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zp.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nu.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oi.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iq.hnjuh.cn

[K05] 深拷贝对象
来源：http://fq.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://vb.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://bt.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ld.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://ec.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://om.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sl.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://su.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://es.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ie.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lc.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rd.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pb.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cw.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dm.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cx.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oc.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cy.szsharing.cn

[K07] 进制转换
来源：http://xu.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vb.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uy.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gn.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pl.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ka.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oc.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uz.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ig.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://oi.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://bi.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bd.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://yg.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://qx.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bh.shxzskj.cn

Go:   encoding/gob
来源：http://zt.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ff.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qs.521024.cn

================================================================================
来源：http://zi.muxihuayi.cn

L. 网络请求
来源：http://yb.bjjhwx.cn

================================================================================
来源：http://os.shxzukj.cn

[L01] 发送 GET 请求
来源：http://vd.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nu.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bq.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://kw.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://lk.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xq.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://ky.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nv.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cn.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://qi.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bb.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qo.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ei.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aq.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xk.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pd.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lu.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://ad.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ix.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ii.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ds.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ng.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hw.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vd.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xl.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ac.jianghongdianzi.cn

[L04] 设置超时
来源：http://tm.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://cg.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uw.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mv.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qb.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zo.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zw.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xs.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lt.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://gm.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ra.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lg.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://co.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qf.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pq.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ba.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rs.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zc.9csxet.cn

[L06] 解析响应为 JSON
来源：http://uo.asd995.cn

Py:   resp.json()
来源：http://pk.colortex.cn

PHP:  json_decode($body, true);
来源：http://hg.yuntaijiaju.cn

JS:   await resp.json()
来源：http://ww.nszjky.cn

TS:   await resp.json()
来源：http://rc.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kf.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gb.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://ft.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oe.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://vw.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vk.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mf.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ai.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://qg.gzmigu.cn

Java: resp.statusCode()
来源：http://qz.colortex.cn

Go:   resp.StatusCode
来源：http://kn.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://rl.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://us.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://xu.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lz.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://nm.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tb.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qu.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nv.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sx.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bm.huixinmuqiang.cn

================================================================================
来源：http://as.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://gd.9csxet.cn

================================================================================
来源：http://sy.asd995.cn

[M01] 读取命令行参数
来源：http://ng.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ih.521024.cn

PHP:  $argv;  $argc;
来源：http://tr.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://ja.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://mb.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://hg.muxihuayi.cn

Go:   os.Args[1:]
来源：http://ld.bookmarksfly.cn

Ruby: ARGV
来源：http://dr.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://dx.panjiajie.cn

[M02] 读取环境变量
来源：http://st.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://la.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sk.muxihuayi.cn

JS:   process.env.HOME
来源：http://ln.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://ls.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://xb.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://os.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://wy.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dc.nszjky.cn

[M03] 执行外部命令
来源：http://xg.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uw.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jd.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mb.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cb.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ta.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tk.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cc.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://la.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://kk.gzmigu.cn

Py:   os.getcwd()
来源：http://vo.yuntaijiaju.cn

PHP:  getcwd();
来源：http://uu.jctech888.com.cn

JS:   process.cwd()
来源：http://jq.shtwfgs.cn

TS:   process.cwd()
来源：http://ov.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://mv.wgjwhj.cn

Go:   os.Getwd()
来源：http://kc.huanxung.cn

Ruby: Dir.pwd
来源：http://rg.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://na.bookmarksfly.cn

[M05] 设置退出码
来源：http://zv.nicolike.cn

Py:   sys.exit(1)
来源：http://zl.hahajie.cn

PHP:  exit(1);
来源：http://zw.muxihuayi.cn

JS:   process.exit(1)
来源：http://qr.colortex.cn

TS:   process.exit(1)
来源：http://lb.yuntaijiaju.cn

Java: System.exit(1)
来源：http://go.hahajie.cn

Go:   os.Exit(1)
来源：http://dv.gzmigu.cn

Ruby: exit 1
来源：http://iu.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ks.asd995.cn

[M06] 向标准错误输出
来源：http://le.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://xp.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ww.shtwfgs.cn

JS:   console.error("err")
来源：http://zf.muxihuayi.cn

TS:   console.error("err")
来源：http://oq.shtwfgs.cn

Java: System.err.println("err")
来源：http://vp.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xc.yuexingan06.cn

Ruby: warn "err"
来源：http://mi.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://mt.hnjuh.cn

[M07] 判断是否为主入口
来源：http://vq.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://wk.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yq.nicolike.cn

JS:   require.main === module
来源：http://yp.colortex.cn

TS:   require.main === module
来源：http://tg.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://jr.huixinmuqiang.cn

Go:   func main()
来源：http://ls.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jr.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://ye.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://kt.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://dy.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://po.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://uw.colortex.cn

TS:   process.platform;  process.version
来源：http://oj.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oo.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bw.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ue.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ci.nszjky.cn

================================================================================
来源：http://aj.chemitech.net.cn

N. 数据结构与算法
来源：http://qu.shxzukj.cn

================================================================================
来源：http://jl.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://vm.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kr.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yw.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sa.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nu.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://av.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://lt.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://es.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yz.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://tx.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://mm.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nb.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ui.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ki.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lw.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://cl.lnxyls.cn

Ruby: arr.sort
来源：http://ws.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hh.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://wo.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xg.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://lw.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tg.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://um.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://px.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pf.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fw.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wj.shxzukj.cn

[N04] 斐波那契数列
来源：http://ez.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uk.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mu.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sa.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aw.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vs.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wa.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dn.haigaiapp.cn

[N05] 最大公约数
来源：http://ax.nicolike.cn

Py:   math.gcd(a, b)
来源：http://mc.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yl.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yi.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yx.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wq.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yk.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://lr.hahajie.cn


<!-- 参考信息 -->