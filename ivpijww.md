代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://or.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://az.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qa.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fw.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vm.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gi.521024.cn

[J05] 时间加减（加 7 天）
来源：http://cs.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://sy.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xe.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iy.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ca.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ot.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ey.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ui.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ia.lnxyls.cn

[J06] 计算两时间之差
来源：http://lu.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://sg.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://yo.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vs.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mt.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ko.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://rl.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://uy.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://lx.lnxyls.cn

[J07] 比较两个日期
来源：http://tx.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://eo.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://al.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rd.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yv.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ge.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aw.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dc.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ws.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://gd.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sj.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oz.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sv.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yv.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ks.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oc.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wm.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rr.asd995.cn

[J09] 时区处理
来源：http://lv.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qy.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://az.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gi.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oj.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fj.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yu.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kd.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uy.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://fw.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nt.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yv.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ie.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ns.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gg.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://av.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eo.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dg.bookmarksfly.cn

================================================================================
来源：http://kw.asd995.cn

K. JSON 与序列化
来源：http://fi.bjjhwx.cn

================================================================================
来源：http://pt.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://jy.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wp.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ji.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ta.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://sy.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pl.huanxung.cn

Go:   json.Marshal(obj)
来源：http://pe.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jr.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qp.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://gw.muxihuayi.cn

Py:   json.loads(s)
来源：http://ah.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.nicolike.cn

JS:   JSON.parse(s)
来源：http://on.nszjky.cn

TS:   JSON.parse(s)
来源：http://mk.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fd.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://bq.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://un.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xy.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://fx.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ym.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hu.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cp.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yr.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://da.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tm.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vj.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eb.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://co.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vw.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://il.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ee.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ux.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sg.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tc.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yh.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pj.shtwfgs.cn

[K05] 深拷贝对象
来源：http://yd.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://iz.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://jd.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://ka.9csxet.cn

TS:   structuredClone(obj)
来源：http://ry.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bn.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jo.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ub.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vv.asd995.cn

[K06] 解析 URL 查询串
来源：http://mi.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gk.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ly.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mg.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gt.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ip.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ez.shxzskj.cn

[K07] 进制转换
来源：http://xn.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nz.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ub.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nq.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ad.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gx.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aj.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ir.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://wq.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://us.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lp.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ke.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://io.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lu.gzmigu.cn

Go:   encoding/gob
来源：http://kd.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://og.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tc.gzmigu.cn

================================================================================
来源：http://ur.szxytkj.cn

L. 网络请求
来源：http://mg.shtwfgs.cn

================================================================================
来源：http://ih.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ch.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://to.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lo.hahajie.cn

JS:   await fetch(url)
来源：http://kx.bookmarksfly.cn

TS:   await fetch(url)
来源：http://ge.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ik.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://bp.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ve.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zh.newstarts.cn

[L02] 发送 POST JSON
来源：http://og.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sd.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qi.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lu.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sd.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uj.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nb.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zv.gzmigu.cn

[L03] 设置自定义请求头
来源：http://kf.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rs.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bn.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kw.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ly.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ai.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://at.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zo.lnxyls.cn

[L04] 设置超时
来源：http://ra.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://iy.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mt.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ai.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gc.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sa.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://or.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jq.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xn.newstarts.cn

[L05] 上传文件（multipart）
来源：http://uf.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://si.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mt.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ou.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tg.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lj.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kb.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zy.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://av.newstarts.cn

Py:   resp.json()
来源：http://cz.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://vz.bjjhwx.cn

JS:   await resp.json()
来源：http://xg.yuntaijiaju.cn

TS:   await resp.json()
来源：http://su.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fg.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zc.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://qv.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xk.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://wk.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tv.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oz.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://ko.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://wr.colortex.cn

Java: resp.statusCode()
来源：http://fw.haigaiapp.cn

Go:   resp.StatusCode
来源：http://vy.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://xr.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://gq.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://jd.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xb.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://dp.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xj.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rt.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jm.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ta.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ze.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ma.huixiangedu.cn

================================================================================
来源：http://bb.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://vj.bjjhwx.cn

================================================================================
来源：http://fl.nszjky.cn

[M01] 读取命令行参数
来源：http://dq.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://je.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://no.szsharing.cn

JS:   process.argv.slice(2)
来源：http://cl.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://wg.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://ri.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://zq.nicolike.cn

Ruby: ARGV
来源：http://xx.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://aj.hnjuh.cn

[M02] 读取环境变量
来源：http://ar.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://cs.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xg.521024.cn

JS:   process.env.HOME
来源：http://is.muxihuayi.cn

TS:   process.env.HOME
来源：http://nb.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://ij.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cd.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://wa.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://em.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://db.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ab.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lh.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xw.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gq.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ce.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eu.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pm.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://he.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://qb.shtwfgs.cn

Py:   os.getcwd()
来源：http://kc.panjiajie.cn

PHP:  getcwd();
来源：http://nc.huixiangedu.cn

JS:   process.cwd()
来源：http://lv.yuntaijiaju.cn

TS:   process.cwd()
来源：http://vc.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://mu.colortex.cn

Go:   os.Getwd()
来源：http://lt.szsharing.cn

Ruby: Dir.pwd
来源：http://ka.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bi.haigaiapp.cn

[M05] 设置退出码
来源：http://yc.nszjky.cn

Py:   sys.exit(1)
来源：http://cr.shxzukj.cn

PHP:  exit(1);
来源：http://au.nszjky.cn

JS:   process.exit(1)
来源：http://dy.nszjky.cn

TS:   process.exit(1)
来源：http://pz.yuexingan06.cn

Java: System.exit(1)
来源：http://mw.chemitech.net.cn

Go:   os.Exit(1)
来源：http://ix.huixiangedu.cn

Ruby: exit 1
来源：http://xf.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gy.wgjwhj.cn

[M06] 向标准错误输出
来源：http://uw.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ge.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gj.wgjwhj.cn

JS:   console.error("err")
来源：http://xj.521024.cn

TS:   console.error("err")
来源：http://vq.panjiajie.cn

Java: System.err.println("err")
来源：http://sc.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ca.huixiangedu.cn

Ruby: warn "err"
来源：http://sv.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://zf.521024.cn

[M07] 判断是否为主入口
来源：http://qc.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://of.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pg.shxzukj.cn

JS:   require.main === module
来源：http://aq.hahajie.cn

TS:   require.main === module
来源：http://sm.asd995.cn

Java: public static void main(String[] args)
来源：http://yv.szxytkj.cn

Go:   func main()
来源：http://mf.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://np.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://bg.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://dq.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://la.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://by.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://td.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://yo.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://km.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gv.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mn.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yg.newstarts.cn

================================================================================
来源：http://kl.hnjuh.cn

N. 数据结构与算法
来源：http://mg.nszjky.cn

================================================================================
来源：http://yt.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://yu.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tu.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uu.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ym.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cm.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uc.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://kw.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vc.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uo.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://pq.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wf.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iz.muxihuayi.cn


<!-- 参考信息 -->