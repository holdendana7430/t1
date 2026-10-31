代发 wailian999

TS:   new Date("2024-01-02")
来源：http://tz.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mr.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eb.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://jr.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ic.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://bo.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qd.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uj.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vd.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lx.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wu.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ak.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nr.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eu.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://lg.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://kk.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fu.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vu.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ro.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ho.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://lc.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wi.shxzskj.cn

[J06] 计算两时间之差
来源：http://um.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://qc.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://lf.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wl.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mh.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gq.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://ae.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://xo.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://qf.hnjuh.cn

[J07] 比较两个日期
来源：http://of.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://gu.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aj.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ri.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uo.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ab.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gy.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ro.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://zr.nicolike.cn

[J08] 提取年月日与星期
来源：http://iq.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hc.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rn.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yu.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ux.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eg.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xr.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wl.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ot.jianghongdianzi.cn

[J09] 时区处理
来源：http://ww.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://km.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ne.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iz.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qp.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fe.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pc.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hx.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lx.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://wx.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://js.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xi.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sq.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mg.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://au.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://it.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gd.bjjhwx.cn

================================================================================
来源：http://bj.nicolike.cn

K. JSON 与序列化
来源：http://vi.colortex.cn

================================================================================
来源：http://hi.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://jn.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zn.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yj.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://sj.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://qc.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ny.asd995.cn

Go:   json.Marshal(obj)
来源：http://gg.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wy.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vw.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://vk.9csxet.cn

Py:   json.loads(s)
来源：http://bc.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bd.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ok.hahajie.cn

TS:   JSON.parse(s)
来源：http://fd.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zm.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://yj.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://tb.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wg.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wf.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hh.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ov.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tw.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wy.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://et.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zd.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gh.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xs.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://jh.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://df.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iw.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kw.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ze.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ud.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vi.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bn.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pw.yuexingan06.cn

[K05] 深拷贝对象
来源：http://kl.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://dq.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://hq.newstarts.cn

JS:   structuredClone(obj)
来源：http://in.newstarts.cn

TS:   structuredClone(obj)
来源：http://ll.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bz.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ll.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tu.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fj.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://fn.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://za.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sl.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ff.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bx.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gt.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wh.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hp.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tj.wgjwhj.cn

[K07] 进制转换
来源：http://fb.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://on.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qk.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://th.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tk.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gq.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uv.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dv.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ws.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://lv.521024.cn

Py:   pickle.dumps(obj)
来源：http://vx.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://at.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://li.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://hm.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ob.huixiangedu.cn

Go:   encoding/gob
来源：http://ch.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://wa.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fu.bjjhwx.cn

================================================================================
来源：http://jc.panjiajie.cn

L. 网络请求
来源：http://vc.nicolike.cn

================================================================================
来源：http://tu.newstarts.cn

[L01] 发送 GET 请求
来源：http://ty.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yy.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ez.nszjky.cn

JS:   await fetch(url)
来源：http://pf.shxzskj.cn

TS:   await fetch(url)
来源：http://hk.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://if.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://gg.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ro.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cc.nicolike.cn

[L02] 发送 POST JSON
来源：http://gz.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vj.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vx.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xs.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://db.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pc.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bd.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hq.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ox.9csxet.cn

[L03] 设置自定义请求头
来源：http://am.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://po.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gh.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vs.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://as.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lm.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ht.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eb.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dx.jctech888.com.cn

[L04] 设置超时
来源：http://wt.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://ke.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ur.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gh.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wu.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ej.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oz.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lh.nszjky.cn

[L05] 上传文件（multipart）
来源：http://zw.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ww.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pu.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ko.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ps.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mk.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hb.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ng.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rm.nicolike.cn

[L06] 解析响应为 JSON
来源：http://yp.panjiajie.cn

Py:   resp.json()
来源：http://up.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://oc.huixinmuqiang.cn

JS:   await resp.json()
来源：http://sa.yuntaijiaju.cn

TS:   await resp.json()
来源：http://ga.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://br.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pp.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ih.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pl.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://kq.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ch.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ud.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://gt.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://dg.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://nq.yuexingan06.cn

Go:   resp.StatusCode
来源：http://dg.521024.cn

Ruby: resp.code.to_i
来源：http://oi.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://hg.szsharing.cn

[L08] 并发请求多个地址
来源：http://hd.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pb.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://bv.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ru.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ad.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mb.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aa.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fz.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xu.szxytkj.cn

================================================================================
来源：http://zh.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ft.shtwfgs.cn

================================================================================
来源：http://jt.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://zq.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://gb.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://es.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://xx.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://yu.521024.cn

Java: args 数组（main 方法参数）
来源：http://ry.colortex.cn

Go:   os.Args[1:]
来源：http://mg.shtwfgs.cn

Ruby: ARGV
来源：http://ku.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://pm.hnjuh.cn

[M02] 读取环境变量
来源：http://sy.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://jn.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vs.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://zw.huanxung.cn

TS:   process.env.HOME
来源：http://zf.gzmigu.cn

Java: System.getenv("HOME")
来源：http://jp.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rq.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://kp.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hd.shxzskj.cn

[M03] 执行外部命令
来源：http://me.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ot.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gj.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tv.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://du.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fh.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wf.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yt.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://zv.shxzukj.cn

[M04] 获取当前工作目录
来源：http://wf.szxytkj.cn

Py:   os.getcwd()
来源：http://ux.wgjwhj.cn

PHP:  getcwd();
来源：http://ep.bookmarksfly.cn

JS:   process.cwd()
来源：http://lj.panjiajie.cn

TS:   process.cwd()
来源：http://ag.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://yj.muxihuayi.cn

Go:   os.Getwd()
来源：http://hz.shxzukj.cn

Ruby: Dir.pwd
来源：http://cq.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qy.hnjuh.cn

[M05] 设置退出码
来源：http://fz.jctech888.com.cn

Py:   sys.exit(1)
来源：http://nr.hnjuh.cn

PHP:  exit(1);
来源：http://cn.shxzskj.cn

JS:   process.exit(1)
来源：http://en.asd995.cn

TS:   process.exit(1)
来源：http://xi.hnjuh.cn

Java: System.exit(1)
来源：http://es.nicolike.cn

Go:   os.Exit(1)
来源：http://tj.nszjky.cn

Ruby: exit 1
来源：http://my.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hs.jctech888.com.cn

[M06] 向标准错误输出
来源：http://fx.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://qp.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jl.jianghongdianzi.cn

JS:   console.error("err")
来源：http://vn.bookmarksfly.cn

TS:   console.error("err")
来源：http://db.haigaiapp.cn

Java: System.err.println("err")
来源：http://en.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zl.lnxyls.cn

Ruby: warn "err"
来源：http://at.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://on.gzmigu.cn

[M07] 判断是否为主入口
来源：http://xa.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://ul.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tt.gzmigu.cn

JS:   require.main === module
来源：http://eh.szsharing.cn

TS:   require.main === module
来源：http://qc.newstarts.cn

Java: public static void main(String[] args)
来源：http://nd.colortex.cn

Go:   func main()
来源：http://im.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jl.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://iu.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ve.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ts.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://we.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ej.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://ko.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yq.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yg.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ws.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lz.wgjwhj.cn

================================================================================
来源：http://ox.szsharing.cn

N. 数据结构与算法
来源：http://zh.nszjky.cn

================================================================================
来源：http://pq.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://bk.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kp.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ty.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ed.colortex.cn


<!-- 参考信息 -->