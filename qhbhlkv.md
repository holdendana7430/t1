代发 wailian999

Ruby: s.scan(/error/i)
来源：http://gr.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cr.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://zh.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mg.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uz.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wn.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zx.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://et.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ph.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://px.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sp.lnxyls.cn

================================================================================
来源：http://xz.jctech888.com.cn

J. 日期与时间
来源：http://zl.gzmigu.cn

================================================================================
来源：http://qg.wgjwhj.cn

[J01] 获取当前时间
来源：http://tn.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fx.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ac.newstarts.cn

JS:   new Date();  Date.now()
来源：http://gq.szsharing.cn

TS:   new Date();  Date.now()
来源：http://nj.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ip.wgjwhj.cn

Go:   time.Now()
来源：http://zx.panjiajie.cn

Ruby: Time.now
来源：http://yd.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zt.shxzukj.cn

[J02] 格式化输出
来源：http://jm.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hq.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hb.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ba.bookmarksfly.cn

TS:   d.toISOString()
来源：http://hg.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cs.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yb.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://up.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jt.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://ah.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lf.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vi.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://eq.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://tm.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rb.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bo.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ss.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bb.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ee.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fq.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tn.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qv.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vt.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pb.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ly.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ge.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ue.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://em.colortex.cn

Py:   now + timedelta(days=7)
来源：http://pv.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gr.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zk.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qy.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://pf.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://va.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dk.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://js.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://uq.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://cg.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ft.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://el.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hy.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://yo.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://mt.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://xl.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://fv.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://gu.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ig.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cl.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jj.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qq.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bn.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uh.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://na.huanxung.cn

[J08] 提取年月日与星期
来源：http://le.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nr.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ut.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gq.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kd.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ae.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dl.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bq.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hb.bjjhwx.cn

[J09] 时区处理
来源：http://md.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gq.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dg.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hs.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zg.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lx.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://no.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dp.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yc.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://hz.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://im.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nv.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://se.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fu.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ae.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ej.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vu.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yk.bookmarksfly.cn

================================================================================
来源：http://yc.asd995.cn

K. JSON 与序列化
来源：http://qu.hahajie.cn

================================================================================
来源：http://ij.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://hr.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cz.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cp.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://nn.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://yv.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dn.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://vt.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vm.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wc.szsharing.cn

[K02] JSON 字符串转对象
来源：http://tn.colortex.cn

Py:   json.loads(s)
来源：http://xj.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dw.hahajie.cn

JS:   JSON.parse(s)
来源：http://ts.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://cf.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sw.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://rw.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://jl.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mp.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ua.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xn.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jj.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qn.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://si.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tz.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xs.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pf.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xu.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ic.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iy.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ib.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dh.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ol.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mx.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ap.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://us.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://js.jctech888.com.cn

[K05] 深拷贝对象
来源：http://dr.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://kc.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://nf.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://pd.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://wd.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mj.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wz.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kl.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ln.hahajie.cn

[K06] 解析 URL 查询串
来源：http://ky.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tg.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ju.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fh.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vo.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mi.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hu.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://st.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://os.jctech888.com.cn

[K07] 进制转换
来源：http://vd.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eb.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oi.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://po.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wa.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mj.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pm.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tn.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://yz.521024.cn

Py:   pickle.dumps(obj)
来源：http://hp.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tt.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://mo.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://po.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yc.huixiangedu.cn

Go:   encoding/gob
来源：http://vr.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ra.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nk.colortex.cn

================================================================================
来源：http://ts.chemitech.net.cn

L. 网络请求
来源：http://ma.nicolike.cn

================================================================================
来源：http://vn.shxzskj.cn

[L01] 发送 GET 请求
来源：http://bj.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hn.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bu.bjjhwx.cn

JS:   await fetch(url)
来源：http://ki.shxzskj.cn

TS:   await fetch(url)
来源：http://vg.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mg.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://sk.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zj.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ic.huanxung.cn

[L02] 发送 POST JSON
来源：http://ly.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://um.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bu.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ja.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qe.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qi.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fi.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dv.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ip.asd995.cn

[L03] 设置自定义请求头
来源：http://nx.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zo.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cw.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bt.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://om.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vm.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rw.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rt.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nc.shxzskj.cn

[L04] 设置超时
来源：http://hy.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://mj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sl.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oq.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lw.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wb.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ta.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://my.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nl.colortex.cn

[L05] 上传文件（multipart）
来源：http://mn.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ul.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lg.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ct.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iu.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ta.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eo.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gk.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://td.9csxet.cn

[L06] 解析响应为 JSON
来源：http://nk.jctech888.com.cn

Py:   resp.json()
来源：http://fr.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://ej.gzmigu.cn

JS:   await resp.json()
来源：http://ru.bookmarksfly.cn

TS:   await resp.json()
来源：http://qv.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://je.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ya.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://kj.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zp.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://bm.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vq.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://us.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://tm.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://rf.hnjuh.cn

Java: resp.statusCode()
来源：http://eg.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://mi.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://th.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ul.newstarts.cn

[L08] 并发请求多个地址
来源：http://vf.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lb.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://kg.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bx.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yy.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nh.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ub.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hy.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sy.521024.cn

================================================================================
来源：http://uk.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://vk.jctech888.com.cn

================================================================================
来源：http://ay.hnjuh.cn

[M01] 读取命令行参数
来源：http://qk.hnjuh.cn

Py:   sys.argv[1:]
来源：http://mu.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://jq.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://lw.hahajie.cn

TS:   process.argv.slice(2)
来源：http://uh.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://rz.lnxyls.cn

Go:   os.Args[1:]
来源：http://af.panjiajie.cn

Ruby: ARGV
来源：http://am.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://cs.chemitech.net.cn

[M02] 读取环境变量
来源：http://to.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://qy.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sl.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://ut.nicolike.cn

TS:   process.env.HOME
来源：http://ir.gzmigu.cn

Java: System.getenv("HOME")
来源：http://mb.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vz.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ch.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mf.jctech888.com.cn

[M03] 执行外部命令
来源：http://bx.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gn.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://id.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dk.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://on.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ry.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tc.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ys.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://ow.shxzskj.cn

[M04] 获取当前工作目录
来源：http://wv.shxzukj.cn

Py:   os.getcwd()
来源：http://rw.wgjwhj.cn

PHP:  getcwd();
来源：http://xx.shxzskj.cn

JS:   process.cwd()
来源：http://pb.hahajie.cn

TS:   process.cwd()
来源：http://fr.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://py.asd995.cn

Go:   os.Getwd()
来源：http://sj.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://gu.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uy.jctech888.com.cn

[M05] 设置退出码
来源：http://pi.hnjuh.cn

Py:   sys.exit(1)
来源：http://iq.521024.cn

PHP:  exit(1);
来源：http://uk.shxzskj.cn

JS:   process.exit(1)
来源：http://wo.9csxet.cn

TS:   process.exit(1)
来源：http://dt.shxzskj.cn

Java: System.exit(1)
来源：http://ff.muxihuayi.cn

Go:   os.Exit(1)
来源：http://ql.muxihuayi.cn


<!-- 参考信息 -->