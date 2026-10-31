代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yt.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pr.haigaiapp.cn

TS:   d.toISOString()
来源：http://zg.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://it.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tl.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wi.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hx.shxzukj.cn

[J03] 字符串解析为日期
来源：http://vy.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ud.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ju.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://xi.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://wi.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nh.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bf.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://to.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sb.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://cy.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ps.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rr.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bb.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ar.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gh.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ye.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qe.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lc.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://wd.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ea.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fd.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ux.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mc.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://jj.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oh.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://ng.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vu.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://mv.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://vc.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://po.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yo.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://co.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dh.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ll.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://mt.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://jx.szxytkj.cn

[J07] 比较两个日期
来源：http://nm.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xt.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ui.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vd.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rh.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zk.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fh.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ke.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://et.colortex.cn

[J08] 提取年月日与星期
来源：http://ke.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tb.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gg.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kn.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zl.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nc.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fk.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vj.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dp.hnjuh.cn

[J09] 时区处理
来源：http://go.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://et.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ac.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fo.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://td.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kw.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gx.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mg.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://um.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://fm.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://op.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ab.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lb.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pr.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wi.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qn.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vs.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dg.jianghongdianzi.cn

================================================================================
来源：http://yr.jctech888.com.cn

K. JSON 与序列化
来源：http://sn.yuexingan06.cn

================================================================================
来源：http://lh.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://tr.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fs.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nh.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://co.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://xl.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ex.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ae.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bc.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rm.nicolike.cn

[K02] JSON 字符串转对象
来源：http://nw.shxzukj.cn

Py:   json.loads(s)
来源：http://ll.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bx.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://cd.hahajie.cn

TS:   JSON.parse(s)
来源：http://wd.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rh.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://bl.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://mw.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ib.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ud.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ig.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vz.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://do.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zn.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xg.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yy.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mz.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pe.hahajie.cn

[K04] 读取 JSON 文件
来源：http://vx.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gf.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zc.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://je.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kt.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nz.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wd.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wt.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sw.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://yv.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://aa.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://is.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://vc.colortex.cn

TS:   structuredClone(obj)
来源：http://zb.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://id.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jx.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ef.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yw.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://vq.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sx.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bo.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://as.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ea.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sc.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yw.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eq.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eh.szxytkj.cn

[K07] 进制转换
来源：http://qf.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ef.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rj.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gn.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wi.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://by.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fk.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ba.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qt.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://qd.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://yf.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ck.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://td.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://qn.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ww.yuntaijiaju.cn

Go:   encoding/gob
来源：http://rb.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://qr.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gt.nszjky.cn

================================================================================
来源：http://od.shxzskj.cn

L. 网络请求
来源：http://ba.haigaiapp.cn

================================================================================
来源：http://bm.hnjuh.cn

[L01] 发送 GET 请求
来源：http://tq.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pn.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kg.nicolike.cn

JS:   await fetch(url)
来源：http://nx.hnjuh.cn

TS:   await fetch(url)
来源：http://mc.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uh.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://ay.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xp.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zm.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://qu.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wy.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sg.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wl.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oc.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ea.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qi.hahajie.cn

[L03] 设置自定义请求头
来源：http://zj.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rz.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rw.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://us.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ir.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gc.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lm.bjjhwx.cn

[L04] 设置超时
来源：http://ht.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://tq.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ki.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pu.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vj.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ii.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lq.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xa.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sn.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://hc.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fr.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nc.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ou.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xc.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yj.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://td.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xw.colortex.cn

[L06] 解析响应为 JSON
来源：http://ed.gzmigu.cn

Py:   resp.json()
来源：http://ol.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ya.asd995.cn

JS:   await resp.json()
来源：http://rf.9csxet.cn

TS:   await resp.json()
来源：http://lg.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dg.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jj.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ia.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dl.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://gl.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lh.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yp.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://km.colortex.cn

TS:   resp.ok;  resp.status
来源：http://bh.nicolike.cn

Java: resp.statusCode()
来源：http://qo.newstarts.cn

Go:   resp.StatusCode
来源：http://uz.szxytkj.cn

Ruby: resp.code.to_i
来源：http://oo.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://jr.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://lo.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ly.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://kq.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fx.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jd.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qu.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pb.muxihuayi.cn

================================================================================
来源：http://te.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://ps.huanxung.cn

================================================================================
来源：http://qu.jctech888.com.cn

[M01] 读取命令行参数
来源：http://cv.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://px.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://vi.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://ye.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ms.colortex.cn

Java: args 数组（main 方法参数）
来源：http://hw.haigaiapp.cn

Go:   os.Args[1:]
来源：http://de.szxytkj.cn

Ruby: ARGV
来源：http://fc.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://gg.bookmarksfly.cn

[M02] 读取环境变量
来源：http://zo.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://bo.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yu.nicolike.cn

JS:   process.env.HOME
来源：http://xc.bookmarksfly.cn

TS:   process.env.HOME
来源：http://zk.lnxyls.cn

Java: System.getenv("HOME")
来源：http://qm.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ii.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://bx.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dv.shtwfgs.cn

[M03] 执行外部命令
来源：http://wp.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pw.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://od.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mf.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sy.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jl.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://np.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sw.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://az.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://if.shtwfgs.cn

Py:   os.getcwd()
来源：http://ba.muxihuayi.cn

PHP:  getcwd();
来源：http://vp.yuntaijiaju.cn

JS:   process.cwd()
来源：http://wf.shxzskj.cn

TS:   process.cwd()
来源：http://ck.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://qb.shxzukj.cn

Go:   os.Getwd()
来源：http://ov.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://pe.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ma.yuexingan06.cn

[M05] 设置退出码
来源：http://yb.huixiangedu.cn

Py:   sys.exit(1)
来源：http://hg.jctech888.com.cn

PHP:  exit(1);
来源：http://eg.huixiangedu.cn

JS:   process.exit(1)
来源：http://ws.521024.cn

TS:   process.exit(1)
来源：http://jh.huixinmuqiang.cn

Java: System.exit(1)
来源：http://vt.asd995.cn

Go:   os.Exit(1)
来源：http://ps.521024.cn

Ruby: exit 1
来源：http://ma.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://to.nicolike.cn

[M06] 向标准错误输出
来源：http://ft.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://pk.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mj.nicolike.cn

JS:   console.error("err")
来源：http://iw.lnxyls.cn

TS:   console.error("err")
来源：http://dw.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://cv.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.panjiajie.cn

Ruby: warn "err"
来源：http://br.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://tr.hahajie.cn

[M07] 判断是否为主入口
来源：http://bo.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://zg.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iy.jianghongdianzi.cn

JS:   require.main === module
来源：http://gy.huanxung.cn

TS:   require.main === module
来源：http://oh.hnjuh.cn

Java: public static void main(String[] args)
来源：http://af.huanxung.cn

Go:   func main()
来源：http://to.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fb.hahajie.cn

C#:   static void Main(string[] args)
来源：http://ym.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://vt.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://if.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://fu.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://gn.asd995.cn


<!-- 参考信息 -->