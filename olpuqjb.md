代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://at.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://sv.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://is.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ld.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ez.nicolike.cn

TS:   /error/gim
来源：http://ee.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dx.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mv.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://wk.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hn.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://pu.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mg.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://es.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sr.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wt.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yp.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ag.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pi.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jp.newstarts.cn

================================================================================
来源：http://kk.gzmigu.cn

J. 日期与时间
来源：http://up.gzmigu.cn

================================================================================
来源：http://ed.bookmarksfly.cn

[J01] 获取当前时间
来源：http://mn.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tj.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gn.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://yt.huanxung.cn

TS:   new Date();  Date.now()
来源：http://eq.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ss.shxzskj.cn

Go:   time.Now()
来源：http://dc.shtwfgs.cn

Ruby: Time.now
来源：http://qx.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pf.nicolike.cn

[J02] 格式化输出
来源：http://gk.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rd.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tl.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://it.shxzskj.cn

TS:   d.toISOString()
来源：http://ab.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bp.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://no.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qc.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xe.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://lj.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sh.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jn.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://es.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://qy.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ln.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nm.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://sd.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sv.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://oj.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rh.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sn.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vu.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bt.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gn.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sl.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tc.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hw.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://cd.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://wu.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mi.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jn.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wi.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://dc.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yt.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ay.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ll.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ha.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://ih.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ee.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ju.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lh.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://do.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://yx.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://xk.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ji.shxzukj.cn

[J07] 比较两个日期
来源：http://jk.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ys.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ac.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pw.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cj.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uj.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mo.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ef.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://fi.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://bl.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lv.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hp.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iu.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xm.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zx.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ia.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gf.jianghongdianzi.cn

[J09] 时区处理
来源：http://xo.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gi.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rb.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dw.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mm.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jh.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ph.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pq.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://pb.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zt.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oa.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nm.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bc.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ih.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ux.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aa.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://vb.jctech888.com.cn

K. JSON 与序列化
来源：http://ap.nicolike.cn

================================================================================
来源：http://df.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://pt.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uv.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://te.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://qo.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://df.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qn.nicolike.cn

Go:   json.Marshal(obj)
来源：http://td.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zw.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lo.asd995.cn

[K02] JSON 字符串转对象
来源：http://ax.panjiajie.cn

Py:   json.loads(s)
来源：http://ei.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kh.nszjky.cn

JS:   JSON.parse(s)
来源：http://ze.shxzskj.cn

TS:   JSON.parse(s)
来源：http://iz.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ue.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://xk.521024.cn

Ruby: JSON.parse(s)
来源：http://pv.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://et.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://yc.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pk.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qx.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hq.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cz.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yl.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://da.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uj.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wa.9csxet.cn

[K04] 读取 JSON 文件
来源：http://ds.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mb.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lz.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yy.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ad.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vk.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fd.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zj.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ae.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://wg.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://wk.shxzukj.cn

JS:   structuredClone(obj)
来源：http://ar.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://on.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://np.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ds.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tt.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lm.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://wd.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zv.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sz.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://js.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ec.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pd.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cv.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://da.wgjwhj.cn

[K07] 进制转换
来源：http://pc.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xd.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://id.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ru.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bs.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aw.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://py.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://th.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ha.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://pe.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://fs.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://du.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ep.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://tj.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ds.yuntaijiaju.cn

Go:   encoding/gob
来源：http://ir.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://tg.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hs.bjjhwx.cn

================================================================================
来源：http://hf.szsharing.cn

L. 网络请求
来源：http://tb.hahajie.cn

================================================================================
来源：http://mi.newstarts.cn

[L01] 发送 GET 请求
来源：http://zv.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://as.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iq.huanxung.cn

JS:   await fetch(url)
来源：http://sy.szsharing.cn

TS:   await fetch(url)
来源：http://iz.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tg.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://cq.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lh.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aa.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://em.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://to.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://si.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yo.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eb.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fm.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oi.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mb.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tg.9csxet.cn

[L03] 设置自定义请求头
来源：http://ed.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gk.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wh.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ka.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tv.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bx.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ga.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jm.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bq.shxzskj.cn

[L04] 设置超时
来源：http://gn.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://xx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bj.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bb.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://co.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://so.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kd.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tl.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://no.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://cw.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kd.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jx.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dc.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://te.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dw.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rt.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dw.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rd.hahajie.cn

[L06] 解析响应为 JSON
来源：http://mp.szsharing.cn

Py:   resp.json()
来源：http://tv.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ou.521024.cn

JS:   await resp.json()
来源：http://kh.haigaiapp.cn

TS:   await resp.json()
来源：http://lb.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vf.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ul.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://mk.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kj.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://pd.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lj.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qn.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://mt.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://av.gzmigu.cn

Java: resp.statusCode()
来源：http://ay.asd995.cn

Go:   resp.StatusCode
来源：http://wd.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://om.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://gz.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://yp.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bh.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ef.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://js.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ct.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eg.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://re.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ro.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sm.yuntaijiaju.cn

================================================================================
来源：http://zu.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://sp.9csxet.cn

================================================================================
来源：http://wo.haigaiapp.cn

[M01] 读取命令行参数
来源：http://fa.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://po.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://is.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://do.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://wu.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://wt.colortex.cn

Go:   os.Args[1:]
来源：http://bj.muxihuayi.cn

Ruby: ARGV
来源：http://jr.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://bo.chemitech.net.cn

[M02] 读取环境变量
来源：http://cp.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://df.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xu.asd995.cn

JS:   process.env.HOME
来源：http://te.panjiajie.cn

TS:   process.env.HOME
来源：http://ug.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://tt.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://js.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://bs.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hd.nszjky.cn

[M03] 执行外部命令
来源：http://pi.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tq.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zl.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jd.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zw.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kh.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rt.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ny.huanxung.cn

[M04] 获取当前工作目录
来源：http://qo.nszjky.cn

Py:   os.getcwd()
来源：http://or.shtwfgs.cn

PHP:  getcwd();
来源：http://wp.yuexingan06.cn

JS:   process.cwd()
来源：http://cq.chemitech.net.cn

TS:   process.cwd()
来源：http://fq.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ba.wgjwhj.cn

Go:   os.Getwd()
来源：http://tk.hnjuh.cn

Ruby: Dir.pwd
来源：http://kv.bjjhwx.cn


<!-- 参考信息 -->