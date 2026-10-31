代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dr.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://cl.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xb.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eh.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xc.jianghongdianzi.cn

TS:   /error/gim
来源：http://eq.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yh.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cw.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://fw.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sm.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://eg.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pf.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fu.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rg.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ca.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eq.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hv.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eb.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ff.chemitech.net.cn

================================================================================
来源：http://wf.521024.cn

J. 日期与时间
来源：http://lh.panjiajie.cn

================================================================================
来源：http://og.asd995.cn

[J01] 获取当前时间
来源：http://rb.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vl.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pq.szsharing.cn

JS:   new Date();  Date.now()
来源：http://et.hahajie.cn

TS:   new Date();  Date.now()
来源：http://tt.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fs.szsharing.cn

Go:   time.Now()
来源：http://rs.gzmigu.cn

Ruby: Time.now
来源：http://na.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vs.yuexingan06.cn

[J02] 格式化输出
来源：http://oo.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ld.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://db.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ia.szxytkj.cn

TS:   d.toISOString()
来源：http://kg.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ui.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://re.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ur.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bs.huanxung.cn

[J03] 字符串解析为日期
来源：http://iw.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sd.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bf.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://dx.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://we.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qf.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uy.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://op.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jx.9csxet.cn

[J04] 时间戳与日期互转
来源：http://jq.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dj.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bo.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ub.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rp.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xl.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hi.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hu.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xu.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://tb.colortex.cn

Py:   now + timedelta(days=7)
来源：http://yd.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://do.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ei.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sn.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ut.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gi.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://mj.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cy.haigaiapp.cn

[J06] 计算两时间之差
来源：http://xw.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ju.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://kb.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pq.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ja.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ec.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://wv.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://xy.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ab.colortex.cn

[J07] 比较两个日期
来源：http://pm.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://vx.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pc.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ux.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dg.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yc.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yu.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gd.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://mt.nicolike.cn

[J08] 提取年月日与星期
来源：http://io.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wh.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fo.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cs.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sc.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kl.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uj.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xb.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mr.muxihuayi.cn

[J09] 时区处理
来源：http://yu.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yw.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lt.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mq.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ui.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fl.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bi.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yl.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xr.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://vh.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ip.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pn.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yc.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rd.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zd.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ew.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jy.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ml.hnjuh.cn

================================================================================
来源：http://aq.shxzukj.cn

K. JSON 与序列化
来源：http://cm.nszjky.cn

================================================================================
来源：http://tr.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://wu.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yu.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://my.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://sc.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://vy.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pu.hahajie.cn

Go:   json.Marshal(obj)
来源：http://cw.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xi.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ca.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://xa.colortex.cn

Py:   json.loads(s)
来源：http://qi.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://as.shxzukj.cn

JS:   JSON.parse(s)
来源：http://io.9csxet.cn

TS:   JSON.parse(s)
来源：http://dr.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wf.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://xq.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://fd.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bv.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://nl.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cg.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nz.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nd.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hv.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mj.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gz.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kk.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cp.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://mh.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jx.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://za.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ue.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lt.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sl.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xp.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ub.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://oy.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://qx.hnjuh.cn

JS:   structuredClone(obj)
来源：http://eg.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://wc.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cy.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cr.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cx.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bi.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://ss.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ch.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fl.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gr.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pq.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yw.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bo.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pg.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ru.haigaiapp.cn

[K07] 进制转换
来源：http://mh.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lt.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ec.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qw.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bm.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uu.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rs.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://au.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ln.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://ic.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ob.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://xj.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://xp.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mx.huixinmuqiang.cn

Go:   encoding/gob
来源：http://rx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://fl.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qk.szxytkj.cn

================================================================================
来源：http://qk.jianghongdianzi.cn

L. 网络请求
来源：http://js.panjiajie.cn

================================================================================
来源：http://ly.9csxet.cn

[L01] 发送 GET 请求
来源：http://cs.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jw.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pi.colortex.cn

JS:   await fetch(url)
来源：http://md.colortex.cn

TS:   await fetch(url)
来源：http://yo.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://li.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://qz.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ew.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://es.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://tp.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gj.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hg.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pv.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gg.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pi.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nk.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://rz.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tf.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ht.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tx.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ay.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oy.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ei.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ul.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ic.chemitech.net.cn

[L04] 设置超时
来源：http://xd.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://fj.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xb.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lv.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qy.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ur.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lx.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fh.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://py.newstarts.cn

[L05] 上传文件（multipart）
来源：http://sk.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kt.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://us.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xp.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zw.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qt.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bm.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wz.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yg.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://wy.jctech888.com.cn

Py:   resp.json()
来源：http://uc.huanxung.cn

PHP:  json_decode($body, true);
来源：http://db.panjiajie.cn

JS:   await resp.json()
来源：http://lx.hnjuh.cn

TS:   await resp.json()
来源：http://my.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fq.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tz.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://pn.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://or.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://id.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ze.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gg.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://pt.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://zs.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://nu.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ir.nszjky.cn

Ruby: resp.code.to_i
来源：http://ig.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://gc.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://vh.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pg.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://sc.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vg.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gz.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zv.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ti.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ed.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ek.colortex.cn

================================================================================
来源：http://uq.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://hd.shxzskj.cn

================================================================================
来源：http://ro.shxzskj.cn

[M01] 读取命令行参数
来源：http://dn.panjiajie.cn

Py:   sys.argv[1:]
来源：http://sl.colortex.cn

PHP:  $argv;  $argc;
来源：http://ym.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://ce.newstarts.cn

TS:   process.argv.slice(2)
来源：http://qx.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://an.lnxyls.cn

Go:   os.Args[1:]
来源：http://ir.yuntaijiaju.cn

Ruby: ARGV
来源：http://ta.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://dm.szxytkj.cn

[M02] 读取环境变量
来源：http://dj.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://lj.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zz.nszjky.cn

JS:   process.env.HOME
来源：http://nf.nszjky.cn

TS:   process.env.HOME
来源：http://lx.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://qv.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gp.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://pd.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mu.huixiangedu.cn

[M03] 执行外部命令
来源：http://hw.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fi.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eb.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ss.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xw.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ji.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mt.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vg.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://xr.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ee.nicolike.cn

Py:   os.getcwd()
来源：http://ip.bjjhwx.cn

PHP:  getcwd();
来源：http://xz.haigaiapp.cn

JS:   process.cwd()
来源：http://jc.shtwfgs.cn

TS:   process.cwd()
来源：http://fh.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://jt.jctech888.com.cn

Go:   os.Getwd()
来源：http://qs.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ms.521024.cn


<!-- 参考信息 -->