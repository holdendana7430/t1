代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lg.panjiajie.cn

TS:   /error/gim
来源：http://gx.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fz.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://es.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://zk.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ol.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://xa.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vr.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nr.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ot.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ai.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://au.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://da.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://au.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vd.bookmarksfly.cn

================================================================================
来源：http://xf.haigaiapp.cn

J. 日期与时间
来源：http://hz.asd995.cn

================================================================================
来源：http://uw.bookmarksfly.cn

[J01] 获取当前时间
来源：http://zp.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cy.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bx.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://bo.9csxet.cn

TS:   new Date();  Date.now()
来源：http://gk.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://br.huanxung.cn

Go:   time.Now()
来源：http://uu.panjiajie.cn

Ruby: Time.now
来源：http://pi.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eh.szxytkj.cn

[J02] 格式化输出
来源：http://ee.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gp.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://su.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bo.panjiajie.cn

TS:   d.toISOString()
来源：http://za.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iz.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ye.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yw.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vu.nicolike.cn

[J03] 字符串解析为日期
来源：http://pm.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uf.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rm.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://nn.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://df.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ii.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kl.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://iw.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://so.hahajie.cn

[J04] 时间戳与日期互转
来源：http://qs.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://si.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wc.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uv.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tb.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kb.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vu.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yz.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ya.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://qx.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://te.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yk.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lm.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wa.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://te.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fk.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://mp.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ie.haigaiapp.cn

[J06] 计算两时间之差
来源：http://kp.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://ko.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://sy.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wv.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vg.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pn.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://tu.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://kt.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://pb.colortex.cn

[J07] 比较两个日期
来源：http://fi.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://yw.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ua.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qt.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qe.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ik.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jj.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rk.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://pm.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://ds.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hr.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ku.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://it.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pj.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fj.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cl.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wc.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zo.chemitech.net.cn

[J09] 时区处理
来源：http://cz.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gd.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lk.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sd.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://px.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hd.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://be.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dm.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lc.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://av.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mo.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mr.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://go.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bb.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fp.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eb.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://at.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vf.yuexingan06.cn

================================================================================
来源：http://to.haigaiapp.cn

K. JSON 与序列化
来源：http://sg.asd995.cn

================================================================================
来源：http://fu.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://qc.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fd.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oe.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://gm.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://da.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qn.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://lb.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tk.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bi.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://lv.chemitech.net.cn

Py:   json.loads(s)
来源：http://kj.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tb.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://pf.shxzukj.cn

TS:   JSON.parse(s)
来源：http://sn.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ea.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://yt.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ug.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pw.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://st.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://am.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ex.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dn.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fl.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qi.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vz.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vk.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lb.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://jt.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mg.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ey.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ey.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://an.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://il.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jp.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qx.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mm.huanxung.cn

[K05] 深拷贝对象
来源：http://wy.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://nx.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://tq.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://cn.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://ml.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://na.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ah.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wa.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://up.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://sc.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://li.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qt.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://an.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cv.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tk.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ex.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fc.newstarts.cn

[K07] 进制转换
来源：http://em.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kd.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cu.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ew.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kv.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gz.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zd.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uv.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ck.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://yu.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://oz.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ja.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ja.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://mq.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dr.9csxet.cn

Go:   encoding/gob
来源：http://nr.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://za.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://da.panjiajie.cn

================================================================================
来源：http://ck.yuntaijiaju.cn

L. 网络请求
来源：http://jd.asd995.cn

================================================================================
来源：http://uq.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ct.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vf.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://th.gzmigu.cn

JS:   await fetch(url)
来源：http://gh.panjiajie.cn

TS:   await fetch(url)
来源：http://uk.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ub.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://li.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bi.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ym.521024.cn

[L02] 发送 POST JSON
来源：http://ck.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ly.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oz.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zc.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://st.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pc.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ir.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lq.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://au.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://gg.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ta.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yg.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jb.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tn.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://li.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hv.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jk.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kj.nicolike.cn

[L04] 设置超时
来源：http://ns.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://fy.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://il.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dr.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ue.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zd.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kz.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ck.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ce.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://va.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qn.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vw.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ay.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://li.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ay.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zi.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wm.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oj.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://kd.wgjwhj.cn

Py:   resp.json()
来源：http://gq.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ys.yuntaijiaju.cn

JS:   await resp.json()
来源：http://jg.panjiajie.cn

TS:   await resp.json()
来源：http://vi.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rl.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gi.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ag.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lz.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://se.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://js.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://to.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://ag.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://il.521024.cn

Java: resp.statusCode()
来源：http://sf.newstarts.cn

Go:   resp.StatusCode
来源：http://ff.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://hk.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://je.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://kt.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wv.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://xh.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fd.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ij.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ve.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ju.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zo.521024.cn

================================================================================
来源：http://lu.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://zu.huanxung.cn

================================================================================
来源：http://up.bjjhwx.cn

[M01] 读取命令行参数
来源：http://hg.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ms.newstarts.cn

PHP:  $argv;  $argc;
来源：http://us.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://in.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://di.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ew.hnjuh.cn

Go:   os.Args[1:]
来源：http://fx.newstarts.cn

Ruby: ARGV
来源：http://xm.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://gq.gzmigu.cn

[M02] 读取环境变量
来源：http://cc.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://or.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dn.shxzukj.cn

JS:   process.env.HOME
来源：http://kx.9csxet.cn

TS:   process.env.HOME
来源：http://zk.nicolike.cn

Java: System.getenv("HOME")
来源：http://eq.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oq.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://hj.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qh.gzmigu.cn

[M03] 执行外部命令
来源：http://qu.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gg.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lt.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ny.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://io.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kc.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://et.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rj.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://nn.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://hg.panjiajie.cn

Py:   os.getcwd()
来源：http://lb.yuexingan06.cn

PHP:  getcwd();
来源：http://ic.colortex.cn

JS:   process.cwd()
来源：http://fo.9csxet.cn

TS:   process.cwd()
来源：http://qf.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://gy.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://oa.nicolike.cn

Ruby: Dir.pwd
来源：http://fb.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uk.shtwfgs.cn

[M05] 设置退出码
来源：http://gg.asd995.cn

Py:   sys.exit(1)
来源：http://cy.lnxyls.cn

PHP:  exit(1);
来源：http://nk.huanxung.cn


<!-- 参考信息 -->