代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ip.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://id.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vg.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uo.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fq.chemitech.net.cn

TS:   /error/gim
来源：http://hk.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dy.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ia.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://ly.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yt.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://fc.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qo.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iv.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zi.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://no.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lk.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://so.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ks.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gb.haigaiapp.cn

================================================================================
来源：http://ne.hahajie.cn

J. 日期与时间
来源：http://ly.newstarts.cn

================================================================================
来源：http://pr.panjiajie.cn

[J01] 获取当前时间
来源：http://su.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://di.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dn.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://gu.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://uj.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sz.huanxung.cn

Go:   time.Now()
来源：http://yr.9csxet.cn

Ruby: Time.now
来源：http://ki.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ij.nicolike.cn

[J02] 格式化输出
来源：http://ee.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rm.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ps.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hm.nicolike.cn

TS:   d.toISOString()
来源：http://ox.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sp.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xe.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fg.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://oz.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nm.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ny.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://yy.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ct.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jx.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xk.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://nu.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://is.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://oi.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://to.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vo.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dj.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gp.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ni.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://er.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vz.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rp.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://bh.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://cn.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ip.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cf.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tc.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://sp.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ba.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://hq.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hx.chemitech.net.cn

[J06] 计算两时间之差
来源：http://zq.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://di.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://en.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bt.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sp.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hl.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://db.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://fx.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://lz.huixiangedu.cn

[J07] 比较两个日期
来源：http://lf.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://pn.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ev.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ie.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jx.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tb.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dl.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vz.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ui.521024.cn

[J08] 提取年月日与星期
来源：http://ra.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hx.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://us.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://su.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ft.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eu.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jy.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://be.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dj.panjiajie.cn

[J09] 时区处理
来源：http://lq.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eo.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cv.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ev.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://od.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bz.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zg.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://at.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vl.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://lq.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tc.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://la.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tz.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mz.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mw.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mf.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hs.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://va.colortex.cn

================================================================================
来源：http://cx.hnjuh.cn

K. JSON 与序列化
来源：http://vn.szxytkj.cn

================================================================================
来源：http://yv.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://gz.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vt.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ta.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://zj.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://vx.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ic.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://im.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wh.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zu.521024.cn

[K02] JSON 字符串转对象
来源：http://cq.bjjhwx.cn

Py:   json.loads(s)
来源：http://ai.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tn.nicolike.cn

JS:   JSON.parse(s)
来源：http://lt.lnxyls.cn

TS:   JSON.parse(s)
来源：http://vx.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cj.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://lf.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://qk.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mf.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://oy.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mp.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ui.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mr.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jy.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ol.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://px.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pi.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://gg.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cy.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ki.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cd.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fv.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://om.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aw.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ib.lnxyls.cn

[K05] 深拷贝对象
来源：http://vj.521024.cn

Py:   copy.deepcopy(obj)
来源：http://gh.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://io.9csxet.cn

JS:   structuredClone(obj)
来源：http://br.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://rh.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ly.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bh.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://al.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dr.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://pn.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wd.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ns.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ba.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pi.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gf.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://re.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ea.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hs.9csxet.cn

[K07] 进制转换
来源：http://kb.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iu.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qh.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gz.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xo.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jz.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ln.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gr.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sh.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://gh.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://lb.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ll.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://vu.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://la.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fj.szxytkj.cn

Go:   encoding/gob
来源：http://hq.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://zg.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xc.asd995.cn

================================================================================
来源：http://ck.yuexingan06.cn

L. 网络请求
来源：http://eq.hnjuh.cn

================================================================================
来源：http://nh.newstarts.cn

[L01] 发送 GET 请求
来源：http://xb.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zg.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://se.bjjhwx.cn

JS:   await fetch(url)
来源：http://rt.shxzskj.cn

TS:   await fetch(url)
来源：http://xq.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tm.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://nv.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rx.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yr.huanxung.cn

[L02] 发送 POST JSON
来源：http://kv.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ql.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wj.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://le.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gu.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wj.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ee.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://te.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vy.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://wm.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eg.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cx.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ay.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ye.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bw.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rn.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gj.gzmigu.cn

[L04] 设置超时
来源：http://pu.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ag.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dt.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aj.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xt.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wd.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zy.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jz.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mf.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ll.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ri.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://se.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zk.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ao.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jg.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ew.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bg.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://id.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://ts.huixiangedu.cn

Py:   resp.json()
来源：http://uh.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://eu.521024.cn

JS:   await resp.json()
来源：http://ab.shxzskj.cn

TS:   await resp.json()
来源：http://nk.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ra.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vr.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://jg.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pf.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://uw.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vf.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://rd.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://ak.bjjhwx.cn

Java: resp.statusCode()
来源：http://ku.shxzukj.cn

Go:   resp.StatusCode
来源：http://mz.lnxyls.cn

Ruby: resp.code.to_i
来源：http://mn.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://wh.asd995.cn

[L08] 并发请求多个地址
来源：http://nl.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hx.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://mr.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hr.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qc.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bw.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wg.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qc.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yh.jianghongdianzi.cn

================================================================================
来源：http://tl.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ti.bjjhwx.cn

================================================================================
来源：http://qw.szsharing.cn

[M01] 读取命令行参数
来源：http://wm.shxzskj.cn

Py:   sys.argv[1:]
来源：http://mt.nszjky.cn

PHP:  $argv;  $argc;
来源：http://im.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://sp.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://hq.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://bh.wgjwhj.cn

Go:   os.Args[1:]
来源：http://gt.bjjhwx.cn

Ruby: ARGV
来源：http://de.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ef.hnjuh.cn

[M02] 读取环境变量
来源：http://ot.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://in.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ql.szsharing.cn

JS:   process.env.HOME
来源：http://ux.szxytkj.cn

TS:   process.env.HOME
来源：http://je.521024.cn

Java: System.getenv("HOME")
来源：http://sc.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vy.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://jo.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uo.shxzukj.cn

[M03] 执行外部命令
来源：http://gv.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jn.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eo.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kf.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oh.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vi.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vq.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yi.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://hg.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://cy.asd995.cn

Py:   os.getcwd()
来源：http://st.colortex.cn

PHP:  getcwd();
来源：http://tw.jianghongdianzi.cn

JS:   process.cwd()
来源：http://gz.wgjwhj.cn

TS:   process.cwd()
来源：http://aj.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ay.muxihuayi.cn

Go:   os.Getwd()
来源：http://su.huanxung.cn

Ruby: Dir.pwd
来源：http://og.shxzskj.cn


<!-- 参考信息 -->