代发 wailian999

Ruby: s.scan(/error/i)
来源：http://ff.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ef.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://va.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ze.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vi.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ib.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gg.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ju.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rm.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pa.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wc.huanxung.cn

================================================================================
来源：http://ra.haigaiapp.cn

J. 日期与时间
来源：http://po.jctech888.com.cn

================================================================================
来源：http://rx.521024.cn

[J01] 获取当前时间
来源：http://im.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hh.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yo.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://oo.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://nx.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wc.huanxung.cn

Go:   time.Now()
来源：http://dp.asd995.cn

Ruby: Time.now
来源：http://sp.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yh.jianghongdianzi.cn

[J02] 格式化输出
来源：http://mj.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vx.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qm.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qd.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://hr.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xk.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://io.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://re.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lx.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://ru.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://io.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zh.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://dp.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://qg.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tn.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ub.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://fe.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jj.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://pb.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ut.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sz.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tp.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sf.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ev.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://es.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nv.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oi.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ua.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://hz.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nh.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nw.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mk.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://ov.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uk.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://oe.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kf.huanxung.cn

[J06] 计算两时间之差
来源：http://sn.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://dg.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://fv.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wq.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bo.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nf.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://pt.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://nw.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://hx.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://go.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://sj.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jo.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nn.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mn.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gi.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xh.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ft.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xa.nicolike.cn

[J08] 提取年月日与星期
来源：http://cd.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lu.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sp.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sj.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ke.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gd.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qz.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ua.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ds.shxzukj.cn

[J09] 时区处理
来源：http://nv.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ip.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kp.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ip.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pu.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wn.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ai.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mv.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fu.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ul.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hd.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ie.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vr.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zc.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iv.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lg.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zu.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cr.shxzskj.cn

================================================================================
来源：http://mf.bookmarksfly.cn

K. JSON 与序列化
来源：http://dr.asd995.cn

================================================================================
来源：http://wg.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://fc.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cb.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pq.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ye.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ht.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cg.newstarts.cn

Go:   json.Marshal(obj)
来源：http://cg.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bu.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yl.nicolike.cn

[K02] JSON 字符串转对象
来源：http://rm.muxihuayi.cn

Py:   json.loads(s)
来源：http://og.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cm.newstarts.cn

JS:   JSON.parse(s)
来源：http://yu.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://li.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://of.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://jh.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://od.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://de.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://fb.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vu.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://im.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://as.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ek.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wn.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ti.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jb.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mr.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://tz.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cb.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lp.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bo.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rq.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jd.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zp.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mw.yuexingan06.cn

[K05] 深拷贝对象
来源：http://wp.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://pq.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://xm.newstarts.cn

JS:   structuredClone(obj)
来源：http://yi.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ct.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sq.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://og.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mk.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hm.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://sn.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qd.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hc.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iz.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://np.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yb.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pq.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aa.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wv.newstarts.cn

[K07] 进制转换
来源：http://ox.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xn.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xk.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://px.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mv.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mg.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://es.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://id.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gi.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://hk.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://fg.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yp.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://qc.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://fs.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sn.muxihuayi.cn

Go:   encoding/gob
来源：http://rj.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://yb.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cf.jianghongdianzi.cn

================================================================================
来源：http://ni.521024.cn

L. 网络请求
来源：http://tw.9csxet.cn

================================================================================
来源：http://pq.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://gu.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ua.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yh.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://un.huixiangedu.cn

TS:   await fetch(url)
来源：http://dz.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ks.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://kl.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://in.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iz.panjiajie.cn

[L02] 发送 POST JSON
来源：http://to.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://px.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vz.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bn.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fo.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bx.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mv.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bk.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://px.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://su.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://in.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vf.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hl.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pe.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://io.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pw.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pd.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qb.huixiangedu.cn

[L04] 设置超时
来源：http://dd.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://hd.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://np.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uz.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tg.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pj.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nm.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qe.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://du.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://af.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hw.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://go.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xa.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ou.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rr.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qy.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qt.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://in.panjiajie.cn

Py:   resp.json()
来源：http://vs.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ox.lnxyls.cn

JS:   await resp.json()
来源：http://dx.yuexingan06.cn

TS:   await resp.json()
来源：http://ft.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ub.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yu.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://gm.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fn.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://xt.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vj.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eh.521024.cn

JS:   resp.ok;  resp.status
来源：http://rd.colortex.cn

TS:   resp.ok;  resp.status
来源：http://bq.gzmigu.cn

Java: resp.statusCode()
来源：http://ih.jctech888.com.cn

Go:   resp.StatusCode
来源：http://jd.9csxet.cn

Ruby: resp.code.to_i
来源：http://eb.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://aq.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://ys.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xw.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://qs.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pd.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vv.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ph.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://si.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cp.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://my.hahajie.cn

================================================================================
来源：http://dd.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ty.bookmarksfly.cn

================================================================================
来源：http://ef.shxzskj.cn

[M01] 读取命令行参数
来源：http://fe.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://wz.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://ah.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ph.szsharing.cn

TS:   process.argv.slice(2)
来源：http://sq.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://uf.hnjuh.cn

Go:   os.Args[1:]
来源：http://ze.huixiangedu.cn

Ruby: ARGV
来源：http://uy.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://od.haigaiapp.cn

[M02] 读取环境变量
来源：http://dr.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://to.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://py.yuexingan06.cn

JS:   process.env.HOME
来源：http://td.huanxung.cn

TS:   process.env.HOME
来源：http://ep.521024.cn

Java: System.getenv("HOME")
来源：http://xg.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://av.hahajie.cn

Ruby: ENV["HOME"]
来源：http://uz.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ev.shxzskj.cn

[M03] 执行外部命令
来源：http://jn.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ew.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ov.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wn.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nv.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pa.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yv.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gj.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://mo.gzmigu.cn

[M04] 获取当前工作目录
来源：http://lt.colortex.cn

Py:   os.getcwd()
来源：http://tt.jianghongdianzi.cn

PHP:  getcwd();
来源：http://mi.haigaiapp.cn

JS:   process.cwd()
来源：http://lu.nszjky.cn

TS:   process.cwd()
来源：http://dr.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://lh.lnxyls.cn

Go:   os.Getwd()
来源：http://di.9csxet.cn

Ruby: Dir.pwd
来源：http://yb.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ce.lnxyls.cn

[M05] 设置退出码
来源：http://cr.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://nn.bookmarksfly.cn

PHP:  exit(1);
来源：http://pf.9csxet.cn

JS:   process.exit(1)
来源：http://au.gzmigu.cn

TS:   process.exit(1)
来源：http://sv.yuexingan06.cn

Java: System.exit(1)
来源：http://uz.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ed.shxzskj.cn


<!-- 参考信息 -->