代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wv.wgjwhj.cn

TS:   /error/gim
来源：http://yf.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dy.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fu.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://sl.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fe.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://li.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ej.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ml.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xw.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tk.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pf.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cd.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iv.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dv.bjjhwx.cn

================================================================================
来源：http://sy.haigaiapp.cn

J. 日期与时间
来源：http://al.szxytkj.cn

================================================================================
来源：http://ni.9csxet.cn

[J01] 获取当前时间
来源：http://mc.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fl.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ht.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://dm.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ad.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iw.asd995.cn

Go:   time.Now()
来源：http://ym.chemitech.net.cn

Ruby: Time.now
来源：http://lz.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dr.wgjwhj.cn

[J02] 格式化输出
来源：http://qz.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rc.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dg.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://by.gzmigu.cn

TS:   d.toISOString()
来源：http://te.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xl.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ox.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sd.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kt.521024.cn

[J03] 字符串解析为日期
来源：http://qu.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zj.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qv.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ny.colortex.cn

TS:   new Date("2024-01-02")
来源：http://cp.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://se.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ki.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ia.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qc.9csxet.cn

[J04] 时间戳与日期互转
来源：http://qa.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://du.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pb.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jd.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://si.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lq.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ll.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hu.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ls.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://da.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://wq.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ea.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ds.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fw.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ai.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://av.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ji.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://on.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://wa.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://ej.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://uh.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ji.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jq.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mx.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://cm.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://tn.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://kw.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://tc.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ql.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://av.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vv.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jp.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ap.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://em.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nj.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://tq.panjiajie.cn

[J08] 提取年月日与星期
来源：http://mt.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sq.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ee.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qb.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://si.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hj.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hw.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bm.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://na.newstarts.cn

[J09] 时区处理
来源：http://rg.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ty.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ar.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uq.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iy.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jj.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zi.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xy.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rq.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://yg.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mq.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fz.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uz.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://on.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gd.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yh.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oc.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xu.nszjky.cn

================================================================================
来源：http://yu.huanxung.cn

K. JSON 与序列化
来源：http://mo.hahajie.cn

================================================================================
来源：http://ig.521024.cn

[K01] 对象转 JSON 字符串
来源：http://ba.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yd.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ks.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://di.colortex.cn

TS:   JSON.stringify(obj)
来源：http://ip.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tj.9csxet.cn

Go:   json.Marshal(obj)
来源：http://as.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kq.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://al.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://xv.nicolike.cn

Py:   json.loads(s)
来源：http://hq.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pw.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ol.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://mg.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yl.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ne.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://ng.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ug.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://az.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uh.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yk.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pl.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://af.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://he.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ru.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xx.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eb.hahajie.cn

[K04] 读取 JSON 文件
来源：http://ls.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dg.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ht.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sb.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ej.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ge.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ci.lnxyls.cn

[K05] 深拷贝对象
来源：http://mt.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ir.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ap.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ol.hnjuh.cn

TS:   structuredClone(obj)
来源：http://eb.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cj.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tz.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mg.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://qt.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sc.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ua.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pd.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lc.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ye.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dx.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fx.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yf.521024.cn

[K07] 进制转换
来源：http://fn.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bm.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mt.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vx.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kx.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ky.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rz.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ua.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pv.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://go.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://uq.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bl.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://sv.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://gv.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tm.wgjwhj.cn

Go:   encoding/gob
来源：http://vx.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://il.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vn.bjjhwx.cn

================================================================================
来源：http://zy.shtwfgs.cn

L. 网络请求
来源：http://la.szxytkj.cn

================================================================================
来源：http://fh.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://it.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rx.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ni.szxytkj.cn

JS:   await fetch(url)
来源：http://ug.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ti.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lj.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://cy.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nh.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qp.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://hs.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ih.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qv.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pr.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://np.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wc.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ho.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tl.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qz.hahajie.cn

[L03] 设置自定义请求头
来源：http://cd.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jo.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://he.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eb.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sg.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zi.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bd.huixinmuqiang.cn

[L04] 设置超时
来源：http://ut.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://zj.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hr.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yx.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://id.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ck.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ot.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eh.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://qg.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cw.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dv.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cr.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jx.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ai.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fc.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://br.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://jc.yuexingan06.cn

Py:   resp.json()
来源：http://kc.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://tz.yuexingan06.cn

JS:   await resp.json()
来源：http://nx.asd995.cn

TS:   await resp.json()
来源：http://pz.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sz.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lb.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://be.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ct.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://dd.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kl.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kq.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://qp.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://pv.nicolike.cn

Java: resp.statusCode()
来源：http://lp.wgjwhj.cn

Go:   resp.StatusCode
来源：http://yy.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://yv.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://bf.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://we.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uf.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://sy.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wz.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mo.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://it.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yu.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ws.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gq.wgjwhj.cn

================================================================================
来源：http://zp.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://of.szxytkj.cn

================================================================================
来源：http://hb.szxytkj.cn

[M01] 读取命令行参数
来源：http://fy.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://qb.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ix.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://nf.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ju.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://rn.nicolike.cn

Go:   os.Args[1:]
来源：http://zz.szsharing.cn

Ruby: ARGV
来源：http://ci.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://pu.hahajie.cn

[M02] 读取环境变量
来源：http://ea.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://lv.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://th.bookmarksfly.cn

JS:   process.env.HOME
来源：http://nk.yuexingan06.cn

TS:   process.env.HOME
来源：http://tc.hnjuh.cn

Java: System.getenv("HOME")
来源：http://eq.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mc.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://fn.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zl.shxzskj.cn

[M03] 执行外部命令
来源：http://sg.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nh.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hi.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://td.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zr.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wr.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lr.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hw.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ve.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://hw.hnjuh.cn

Py:   os.getcwd()
来源：http://gh.huixinmuqiang.cn

PHP:  getcwd();
来源：http://zn.nszjky.cn

JS:   process.cwd()
来源：http://bn.colortex.cn

TS:   process.cwd()
来源：http://ow.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://jv.bjjhwx.cn

Go:   os.Getwd()
来源：http://em.szsharing.cn

Ruby: Dir.pwd
来源：http://xi.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ch.shxzskj.cn

[M05] 设置退出码
来源：http://uz.shxzukj.cn

Py:   sys.exit(1)
来源：http://ma.lnxyls.cn

PHP:  exit(1);
来源：http://uc.huixiangedu.cn


<!-- 参考信息 -->