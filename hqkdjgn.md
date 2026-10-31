代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bt.asd995.cn

TS:   /error/gim
来源：http://ru.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mo.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yc.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://jv.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ak.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://xj.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bl.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eo.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ss.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qk.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pa.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ib.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ne.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rm.hnjuh.cn

================================================================================
来源：http://pz.gzmigu.cn

J. 日期与时间
来源：http://co.hahajie.cn

================================================================================
来源：http://ly.yuexingan06.cn

[J01] 获取当前时间
来源：http://hv.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vu.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ng.colortex.cn

JS:   new Date();  Date.now()
来源：http://yv.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ed.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bc.newstarts.cn

Go:   time.Now()
来源：http://yc.9csxet.cn

Ruby: Time.now
来源：http://nj.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://da.bookmarksfly.cn

[J02] 格式化输出
来源：http://zl.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vh.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wj.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ed.jctech888.com.cn

TS:   d.toISOString()
来源：http://gi.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kh.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ap.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mk.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://af.lnxyls.cn

[J03] 字符串解析为日期
来源：http://nr.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yb.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uo.colortex.cn

JS:   new Date("2024-01-02")
来源：http://br.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://at.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sw.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ht.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ck.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tl.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://yf.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nu.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ng.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ch.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mz.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://se.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://et.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ws.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tz.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://ld.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://pc.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vv.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cz.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tv.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ad.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ka.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://gj.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yx.hnjuh.cn

[J06] 计算两时间之差
来源：http://qz.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://ha.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ip.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jn.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ph.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ha.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://pg.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://jy.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://ny.szxytkj.cn

[J07] 比较两个日期
来源：http://rc.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://jb.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yj.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ta.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fw.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pp.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rt.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://go.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zm.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://vp.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iq.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ki.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ff.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rt.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tl.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cs.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nh.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tt.hnjuh.cn

[J09] 时区处理
来源：http://py.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qp.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pd.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qw.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bs.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hd.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mc.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wb.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nm.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://zy.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ab.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dm.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yd.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wf.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ou.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nh.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kc.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vt.muxihuayi.cn

================================================================================
来源：http://rn.szsharing.cn

K. JSON 与序列化
来源：http://sa.9csxet.cn

================================================================================
来源：http://xd.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://ah.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yi.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jz.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://xm.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://or.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zc.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://uh.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mm.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lg.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://co.nszjky.cn

Py:   json.loads(s)
来源：http://zb.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eo.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://uy.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://by.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jo.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://fx.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://yi.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jm.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://fm.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rl.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ss.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sj.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ty.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://af.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vy.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iz.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zs.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://mg.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uv.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iz.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mx.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wq.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ye.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ay.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rf.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fo.shxzskj.cn

[K05] 深拷贝对象
来源：http://iw.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://jn.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://lg.newstarts.cn

JS:   structuredClone(obj)
来源：http://ge.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://au.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mb.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xg.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rq.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wj.nicolike.cn

[K06] 解析 URL 查询串
来源：http://tk.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sn.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ek.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pk.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xg.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qx.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eb.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xj.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fu.hahajie.cn

[K07] 进制转换
来源：http://ti.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kd.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nf.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ma.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://va.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://md.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://en.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wj.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://os.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ra.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://bs.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ot.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ei.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://yv.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wy.shtwfgs.cn

Go:   encoding/gob
来源：http://mk.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ml.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mq.huanxung.cn

================================================================================
来源：http://nr.huixinmuqiang.cn

L. 网络请求
来源：http://ua.hahajie.cn

================================================================================
来源：http://fj.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://da.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qn.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hu.panjiajie.cn

JS:   await fetch(url)
来源：http://hr.9csxet.cn

TS:   await fetch(url)
来源：http://ji.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mk.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://nm.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ox.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://en.huanxung.cn

[L02] 发送 POST JSON
来源：http://bv.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cd.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qw.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ne.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xf.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nz.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://go.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yu.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yr.shxzskj.cn

[L03] 设置自定义请求头
来源：http://bd.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hs.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://br.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nw.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cz.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sg.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yj.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://et.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yx.huixinmuqiang.cn

[L04] 设置超时
来源：http://yx.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://vx.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nm.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pd.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vg.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ko.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ab.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pm.asd995.cn

[L05] 上传文件（multipart）
来源：http://fl.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ux.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sp.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dg.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ih.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nc.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wi.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ca.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hw.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sc.yuntaijiaju.cn

Py:   resp.json()
来源：http://vw.nicolike.cn

PHP:  json_decode($body, true);
来源：http://lz.yuntaijiaju.cn

JS:   await resp.json()
来源：http://ol.yuexingan06.cn

TS:   await resp.json()
来源：http://ka.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wy.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://de.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://cr.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nv.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://km.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ge.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xk.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://df.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://rx.shxzskj.cn

Java: resp.statusCode()
来源：http://hc.shxzukj.cn

Go:   resp.StatusCode
来源：http://pk.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://gf.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://or.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://ha.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://me.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://ys.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ad.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wg.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vp.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ji.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hc.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pu.yuntaijiaju.cn

================================================================================
来源：http://nf.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://fu.asd995.cn

================================================================================
来源：http://ry.yuexingan06.cn

[M01] 读取命令行参数
来源：http://mb.gzmigu.cn

Py:   sys.argv[1:]
来源：http://yv.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://tw.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://sm.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ec.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://zp.nicolike.cn

Go:   os.Args[1:]
来源：http://lv.bookmarksfly.cn

Ruby: ARGV
来源：http://qy.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://fb.jctech888.com.cn

[M02] 读取环境变量
来源：http://iw.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ia.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ee.hnjuh.cn

JS:   process.env.HOME
来源：http://qc.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ba.9csxet.cn

Java: System.getenv("HOME")
来源：http://ba.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ll.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ac.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sp.bookmarksfly.cn

[M03] 执行外部命令
来源：http://hc.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ep.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yb.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nf.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gj.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ee.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gx.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pk.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://yu.hahajie.cn

[M04] 获取当前工作目录
来源：http://kw.wgjwhj.cn

Py:   os.getcwd()
来源：http://xz.asd995.cn

PHP:  getcwd();
来源：http://zc.hahajie.cn

JS:   process.cwd()
来源：http://ok.lnxyls.cn

TS:   process.cwd()
来源：http://tm.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ap.newstarts.cn

Go:   os.Getwd()
来源：http://du.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ua.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vo.shtwfgs.cn

[M05] 设置退出码
来源：http://kg.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://vj.szsharing.cn

PHP:  exit(1);
来源：http://eh.jctech888.com.cn


<!-- 参考信息 -->