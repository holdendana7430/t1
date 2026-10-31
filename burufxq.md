代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ld.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eg.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vy.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jv.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yp.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://iz.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cj.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iv.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hc.chemitech.net.cn

TS:   /error/gim
来源：http://sl.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fb.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pg.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ek.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vb.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://js.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ip.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bd.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iv.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mq.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yh.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ww.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mt.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zk.jianghongdianzi.cn

================================================================================
来源：http://li.asd995.cn

J. 日期与时间
来源：http://ag.szxytkj.cn

================================================================================
来源：http://hu.nszjky.cn

[J01] 获取当前时间
来源：http://cv.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hm.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mt.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://mk.huanxung.cn

TS:   new Date();  Date.now()
来源：http://xn.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gl.haigaiapp.cn

Go:   time.Now()
来源：http://gn.lnxyls.cn

Ruby: Time.now
来源：http://hr.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bk.9csxet.cn

[J02] 格式化输出
来源：http://cy.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cy.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mw.haigaiapp.cn

TS:   d.toISOString()
来源：http://bm.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://at.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ae.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://un.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wb.9csxet.cn

[J03] 字符串解析为日期
来源：http://mo.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ne.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ja.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://qf.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://sl.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iu.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ce.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ld.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rq.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://et.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://by.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://do.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ha.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gs.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ll.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://we.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tv.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ft.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ei.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://jr.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ty.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rq.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ia.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gz.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://vl.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ih.yuexingan06.cn

[J06] 计算两时间之差
来源：http://jp.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://qk.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://sc.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gr.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nd.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dw.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://yn.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://na.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://pk.yuexingan06.cn

[J07] 比较两个日期
来源：http://jf.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://bl.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gi.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rd.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ci.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ca.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ei.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ru.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://zm.asd995.cn

[J08] 提取年月日与星期
来源：http://bu.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nw.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xw.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hg.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ws.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sv.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fx.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sn.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nm.chemitech.net.cn

[J09] 时区处理
来源：http://bn.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dv.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uo.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ch.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ay.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oh.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://up.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xr.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://qq.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tf.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vv.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zp.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yr.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lo.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rj.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://om.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gr.gzmigu.cn

================================================================================
来源：http://na.nszjky.cn

K. JSON 与序列化
来源：http://ow.jctech888.com.cn

================================================================================
来源：http://wk.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://sc.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vh.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wt.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://yy.521024.cn

TS:   JSON.stringify(obj)
来源：http://xx.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yb.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://au.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ad.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xl.hahajie.cn

[K02] JSON 字符串转对象
来源：http://qu.nszjky.cn

Py:   json.loads(s)
来源：http://mq.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cg.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://qr.nicolike.cn

TS:   JSON.parse(s)
来源：http://lo.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ky.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://pr.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://dh.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ui.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://nh.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pc.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xb.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://be.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mp.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dn.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ve.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://os.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qf.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://qq.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cj.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kt.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gj.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vu.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://va.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nn.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ke.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jx.huixiangedu.cn

[K05] 深拷贝对象
来源：http://il.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://ze.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ov.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://qf.shxzukj.cn

TS:   structuredClone(obj)
来源：http://gc.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jk.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pi.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gq.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wn.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://le.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ot.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fw.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yv.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://md.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fx.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://om.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fr.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zp.hahajie.cn

[K07] 进制转换
来源：http://sc.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pr.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lp.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bk.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fo.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://se.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ah.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bv.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ow.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://es.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://yv.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ov.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://oh.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fv.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tc.jianghongdianzi.cn

Go:   encoding/gob
来源：http://xw.521024.cn

Ruby: Marshal.dump(obj)
来源：http://pe.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kk.gzmigu.cn

================================================================================
来源：http://xm.jianghongdianzi.cn

L. 网络请求
来源：http://um.huixiangedu.cn

================================================================================
来源：http://jh.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ww.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lr.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wm.jctech888.com.cn

JS:   await fetch(url)
来源：http://ry.shtwfgs.cn

TS:   await fetch(url)
来源：http://dv.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gl.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://nb.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://on.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ay.hahajie.cn

[L02] 发送 POST JSON
来源：http://wz.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pl.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://by.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ar.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://af.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nc.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rk.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hx.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ee.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://en.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ky.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kz.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://np.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gw.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dr.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tb.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gl.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uu.shxzskj.cn

[L04] 设置超时
来源：http://tb.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ma.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tc.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qj.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oh.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nn.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cw.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ju.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nh.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://rk.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pv.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fl.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gw.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xn.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ln.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://or.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zr.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rm.hahajie.cn

[L06] 解析响应为 JSON
来源：http://ot.nicolike.cn

Py:   resp.json()
来源：http://cm.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://zc.shxzukj.cn

JS:   await resp.json()
来源：http://cq.haigaiapp.cn

TS:   await resp.json()
来源：http://ej.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vz.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qm.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://rq.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rw.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://vh.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bu.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vo.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://zw.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://em.panjiajie.cn

Java: resp.statusCode()
来源：http://kt.gzmigu.cn

Go:   resp.StatusCode
来源：http://sk.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://fd.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://wa.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://nb.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://em.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://yi.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sw.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://er.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rk.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cd.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ho.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://at.shxzukj.cn

================================================================================
来源：http://fu.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://iy.chemitech.net.cn

================================================================================
来源：http://vi.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://vz.newstarts.cn

Py:   sys.argv[1:]
来源：http://vk.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://lb.nszjky.cn

JS:   process.argv.slice(2)
来源：http://wi.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://ah.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://dr.newstarts.cn

Go:   os.Args[1:]
来源：http://xf.yuntaijiaju.cn

Ruby: ARGV
来源：http://df.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://cz.shtwfgs.cn

[M02] 读取环境变量
来源：http://fs.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://qx.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hu.asd995.cn

JS:   process.env.HOME
来源：http://uo.panjiajie.cn

TS:   process.env.HOME
来源：http://mn.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://vw.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lw.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://sy.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vq.hnjuh.cn

[M03] 执行外部命令
来源：http://vu.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://km.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mw.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vd.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eb.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pm.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cd.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wb.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://jf.hahajie.cn

[M04] 获取当前工作目录
来源：http://gi.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://ai.lnxyls.cn

PHP:  getcwd();
来源：http://ml.muxihuayi.cn

JS:   process.cwd()
来源：http://rk.lnxyls.cn


<!-- 参考信息 -->