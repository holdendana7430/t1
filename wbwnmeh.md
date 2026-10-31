代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ub.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gx.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qd.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ym.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://mt.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ut.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lt.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://hh.asd995.cn

TS:   new Date("2024-01-02")
来源：http://ns.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fj.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zd.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://cq.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xp.521024.cn

[J04] 时间戳与日期互转
来源：http://cd.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ye.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hb.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jx.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kt.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://os.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sh.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dq.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gr.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://ra.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://bk.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vc.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wy.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gm.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://zq.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mv.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://dd.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://am.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://fo.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://pw.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://jj.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ao.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sm.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://go.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://lr.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://ml.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://gn.shtwfgs.cn

[J07] 比较两个日期
来源：http://vi.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qr.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qd.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bg.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uz.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://as.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xe.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pz.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zh.9csxet.cn

[J08] 提取年月日与星期
来源：http://ww.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hx.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zz.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mb.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fc.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gs.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ju.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://px.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xb.521024.cn

[J09] 时区处理
来源：http://sv.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vu.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xm.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yr.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lj.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pp.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gn.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ny.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ac.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://eb.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lb.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zb.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mw.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://px.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ux.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ic.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ik.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sd.huixiangedu.cn

================================================================================
来源：http://dk.bookmarksfly.cn

K. JSON 与序列化
来源：http://tw.bookmarksfly.cn

================================================================================
来源：http://yv.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://db.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hb.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://bi.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ls.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wf.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://bc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cv.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kx.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://mv.bookmarksfly.cn

Py:   json.loads(s)
来源：http://cu.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jh.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ty.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://zd.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tr.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://eu.nszjky.cn

Ruby: JSON.parse(s)
来源：http://sx.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sv.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://wz.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tk.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oz.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fu.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vs.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ss.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gd.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gz.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qb.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://ma.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tg.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hi.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qq.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ph.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jm.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bg.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://to.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yh.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://pz.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://ag.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://cy.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://ic.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://wb.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ao.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gj.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vr.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rz.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ap.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xr.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ss.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mq.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bq.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oj.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fj.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ae.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ef.muxihuayi.cn

[K07] 进制转换
来源：http://wg.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hu.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oc.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bp.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ra.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wy.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wf.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ud.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oi.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qe.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://oe.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xj.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://yo.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://yo.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ul.shxzskj.cn

Go:   encoding/gob
来源：http://ig.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ng.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ph.9csxet.cn

================================================================================
来源：http://ov.jianghongdianzi.cn

L. 网络请求
来源：http://mp.muxihuayi.cn

================================================================================
来源：http://ea.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://qy.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tr.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xd.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ef.haigaiapp.cn

TS:   await fetch(url)
来源：http://ix.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://id.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://io.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qj.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://op.shxzskj.cn

[L02] 发送 POST JSON
来源：http://dm.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://we.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oc.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://an.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ml.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wy.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ku.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bj.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pj.panjiajie.cn

[L03] 设置自定义请求头
来源：http://zu.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aw.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mw.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ie.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fz.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rf.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gr.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tb.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yw.newstarts.cn

[L04] 设置超时
来源：http://tc.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://xx.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zl.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rn.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yt.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://am.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hh.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uw.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://cf.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xy.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mh.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yh.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://se.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ho.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wq.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sd.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://al.panjiajie.cn

Py:   resp.json()
来源：http://jv.colortex.cn

PHP:  json_decode($body, true);
来源：http://ck.jctech888.com.cn

JS:   await resp.json()
来源：http://ya.panjiajie.cn

TS:   await resp.json()
来源：http://vn.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yj.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nf.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://to.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://up.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://cs.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nj.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://av.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://jq.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://kp.bookmarksfly.cn

Java: resp.statusCode()
来源：http://dh.yuexingan06.cn

Go:   resp.StatusCode
来源：http://fz.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://uf.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://bl.szsharing.cn

[L08] 并发请求多个地址
来源：http://xm.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nk.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://wc.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://da.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cl.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xb.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pd.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yz.shxzukj.cn

================================================================================
来源：http://jh.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ul.haigaiapp.cn

================================================================================
来源：http://in.chemitech.net.cn

[M01] 读取命令行参数
来源：http://cw.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://ps.nicolike.cn

PHP:  $argv;  $argc;
来源：http://tt.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://fq.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://ly.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://um.nicolike.cn

Go:   os.Args[1:]
来源：http://jh.huanxung.cn

Ruby: ARGV
来源：http://jh.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://fu.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ds.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://yf.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bf.hahajie.cn

JS:   process.env.HOME
来源：http://vb.9csxet.cn

TS:   process.env.HOME
来源：http://oo.nszjky.cn

Java: System.getenv("HOME")
来源：http://js.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://be.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://rk.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pu.yuexingan06.cn

[M03] 执行外部命令
来源：http://xw.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nk.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ao.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ra.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eu.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mv.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://br.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ar.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://tn.521024.cn

[M04] 获取当前工作目录
来源：http://gx.nszjky.cn

Py:   os.getcwd()
来源：http://ra.shtwfgs.cn

PHP:  getcwd();
来源：http://wj.bjjhwx.cn

JS:   process.cwd()
来源：http://vi.szsharing.cn

TS:   process.cwd()
来源：http://lh.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bf.shtwfgs.cn

Go:   os.Getwd()
来源：http://iq.colortex.cn

Ruby: Dir.pwd
来源：http://ph.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zy.hahajie.cn

[M05] 设置退出码
来源：http://ob.jctech888.com.cn

Py:   sys.exit(1)
来源：http://bi.muxihuayi.cn

PHP:  exit(1);
来源：http://yp.colortex.cn

JS:   process.exit(1)
来源：http://bh.shtwfgs.cn

TS:   process.exit(1)
来源：http://xa.bjjhwx.cn

Java: System.exit(1)
来源：http://rz.szsharing.cn

Go:   os.Exit(1)
来源：http://kx.yuntaijiaju.cn

Ruby: exit 1
来源：http://oi.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yh.nicolike.cn

[M06] 向标准错误输出
来源：http://iz.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://kc.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jq.bookmarksfly.cn

JS:   console.error("err")
来源：http://kq.lnxyls.cn

TS:   console.error("err")
来源：http://xy.asd995.cn

Java: System.err.println("err")
来源：http://xn.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pv.521024.cn

Ruby: warn "err"
来源：http://ge.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://pd.nszjky.cn

[M07] 判断是否为主入口
来源：http://my.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://sp.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ct.muxihuayi.cn

JS:   require.main === module
来源：http://sw.lnxyls.cn

TS:   require.main === module
来源：http://ap.521024.cn

Java: public static void main(String[] args)
来源：http://ym.panjiajie.cn

Go:   func main()
来源：http://ys.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xt.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://tw.521024.cn

[M08] 获取系统与运行时信息
来源：http://bn.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ze.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ji.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://ie.nszjky.cn

TS:   process.platform;  process.version
来源：http://sj.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://th.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oh.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qi.gzmigu.cn


<!-- 参考信息 -->