代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rq.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tv.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dc.gzmigu.cn

TS:   d.toISOString()
来源：http://kq.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fi.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qp.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hb.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hk.9csxet.cn

[J03] 字符串解析为日期
来源：http://ox.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wt.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ae.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://wb.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://oo.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://db.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xy.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://jw.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gd.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://rr.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eu.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vt.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xo.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xk.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bz.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sd.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nn.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sm.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://rc.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://tn.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zs.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zq.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nc.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://et.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://io.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://md.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dd.nicolike.cn

[J06] 计算两时间之差
来源：http://dd.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://yy.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://nk.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jh.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vs.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ha.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://fn.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://yv.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://mg.9csxet.cn

[J07] 比较两个日期
来源：http://sk.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://vw.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ya.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wy.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kd.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xe.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lz.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wt.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ok.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://wl.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gy.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://py.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ei.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rq.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rh.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yi.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wb.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bp.colortex.cn

[J09] 时区处理
来源：http://pz.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kz.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ww.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sk.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ml.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sj.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ly.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gk.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rs.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://kp.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fx.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wp.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jo.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ud.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ak.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wm.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hu.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vu.huixiangedu.cn

================================================================================
来源：http://ul.huixiangedu.cn

K. JSON 与序列化
来源：http://hw.hahajie.cn

================================================================================
来源：http://nq.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://ft.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ai.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cy.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://xh.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://fn.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://en.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://ms.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ay.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kf.huanxung.cn

[K02] JSON 字符串转对象
来源：http://tn.521024.cn

Py:   json.loads(s)
来源：http://nu.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://si.colortex.cn

JS:   JSON.parse(s)
来源：http://og.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://kx.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tp.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://uv.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://di.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gy.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ns.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kx.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tr.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pc.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yb.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xh.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zb.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fg.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://we.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ta.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ic.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dr.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bk.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vo.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fy.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ic.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fk.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jx.521024.cn

[K05] 深拷贝对象
来源：http://dr.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://uy.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://tc.lnxyls.cn

JS:   structuredClone(obj)
来源：http://jj.gzmigu.cn

TS:   structuredClone(obj)
来源：http://op.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tv.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vz.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dc.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ji.9csxet.cn

[K06] 解析 URL 查询串
来源：http://jt.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lo.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ys.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nk.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hb.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fo.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qp.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cg.huixiangedu.cn

[K07] 进制转换
来源：http://mf.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qr.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ek.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zj.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bk.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bk.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tk.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qw.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://da.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://vp.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://us.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qg.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://fp.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://sd.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bv.newstarts.cn

Go:   encoding/gob
来源：http://vz.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://iq.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pk.szsharing.cn

================================================================================
来源：http://yo.yuexingan06.cn

L. 网络请求
来源：http://qv.hnjuh.cn

================================================================================
来源：http://xg.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://ll.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xp.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ik.521024.cn

JS:   await fetch(url)
来源：http://fg.shtwfgs.cn

TS:   await fetch(url)
来源：http://eh.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rd.521024.cn

Go:   resp, err := http.Get(url)
来源：http://qp.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vi.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sy.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://mm.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ju.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://in.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gg.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hh.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pz.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bb.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xw.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yl.521024.cn

[L03] 设置自定义请求头
来源：http://se.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cs.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aa.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jo.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sy.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://in.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pu.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qq.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://va.colortex.cn

[L04] 设置超时
来源：http://rs.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://df.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ns.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jc.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://le.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ag.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jd.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sn.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vf.521024.cn

[L05] 上传文件（multipart）
来源：http://rg.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hw.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ew.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cp.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oh.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://py.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pv.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zp.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mu.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://lq.gzmigu.cn

Py:   resp.json()
来源：http://ou.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://ch.muxihuayi.cn

JS:   await resp.json()
来源：http://kv.nicolike.cn

TS:   await resp.json()
来源：http://xn.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yv.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qd.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://fx.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wr.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://xx.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ih.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ad.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://bl.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ku.haigaiapp.cn

Java: resp.statusCode()
来源：http://is.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ul.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ny.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://mo.shxzskj.cn

[L08] 并发请求多个地址
来源：http://yh.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ar.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://we.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yf.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vo.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ys.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://be.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rk.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gc.szsharing.cn

================================================================================
来源：http://vv.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://ov.gzmigu.cn

================================================================================
来源：http://ef.yuexingan06.cn

[M01] 读取命令行参数
来源：http://eu.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ca.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://dy.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://pu.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://bf.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://mg.hahajie.cn

Go:   os.Args[1:]
来源：http://xc.bookmarksfly.cn

Ruby: ARGV
来源：http://nm.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://nz.asd995.cn

[M02] 读取环境变量
来源：http://ql.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://my.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gp.shtwfgs.cn

JS:   process.env.HOME
来源：http://zs.muxihuayi.cn

TS:   process.env.HOME
来源：http://mk.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://pu.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cg.colortex.cn

Ruby: ENV["HOME"]
来源：http://rd.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sq.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://hi.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ft.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://di.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yo.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://na.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fu.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xg.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vh.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ny.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://id.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://og.huixinmuqiang.cn

PHP:  getcwd();
来源：http://qp.jianghongdianzi.cn

JS:   process.cwd()
来源：http://pv.bjjhwx.cn

TS:   process.cwd()
来源：http://mb.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://lo.hnjuh.cn

Go:   os.Getwd()
来源：http://bx.huanxung.cn

Ruby: Dir.pwd
来源：http://jg.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cd.bookmarksfly.cn

[M05] 设置退出码
来源：http://jd.muxihuayi.cn

Py:   sys.exit(1)
来源：http://to.shtwfgs.cn

PHP:  exit(1);
来源：http://nm.colortex.cn

JS:   process.exit(1)
来源：http://qv.jctech888.com.cn

TS:   process.exit(1)
来源：http://ns.szsharing.cn

Java: System.exit(1)
来源：http://wx.szsharing.cn

Go:   os.Exit(1)
来源：http://tr.shtwfgs.cn

Ruby: exit 1
来源：http://jc.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pu.hahajie.cn

[M06] 向标准错误输出
来源：http://zt.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://vg.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ax.szxytkj.cn

JS:   console.error("err")
来源：http://wo.hnjuh.cn

TS:   console.error("err")
来源：http://ub.gzmigu.cn

Java: System.err.println("err")
来源：http://hr.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://op.wgjwhj.cn

Ruby: warn "err"
来源：http://ec.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://fn.hahajie.cn

[M07] 判断是否为主入口
来源：http://ax.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://zw.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fi.nszjky.cn

JS:   require.main === module
来源：http://il.bookmarksfly.cn

TS:   require.main === module
来源：http://ws.asd995.cn

Java: public static void main(String[] args)
来源：http://em.haigaiapp.cn

Go:   func main()
来源：http://pa.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hx.colortex.cn

C#:   static void Main(string[] args)
来源：http://wd.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://mf.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://jh.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ro.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://uc.nszjky.cn


<!-- 参考信息 -->