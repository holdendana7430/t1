代发 wailian999

Ruby: s.scan(/error/i)
来源：http://nu.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://il.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://cy.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ev.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tr.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mo.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jv.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mp.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kw.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jl.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ys.asd995.cn

================================================================================
来源：http://xg.hnjuh.cn

J. 日期与时间
来源：http://mw.bjjhwx.cn

================================================================================
来源：http://bs.szxytkj.cn

[J01] 获取当前时间
来源：http://kp.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zg.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ng.hahajie.cn

JS:   new Date();  Date.now()
来源：http://ct.nicolike.cn

TS:   new Date();  Date.now()
来源：http://vh.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kj.huanxung.cn

Go:   time.Now()
来源：http://jz.nszjky.cn

Ruby: Time.now
来源：http://rc.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://as.newstarts.cn

[J02] 格式化输出
来源：http://qb.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wk.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kl.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ay.bookmarksfly.cn

TS:   d.toISOString()
来源：http://uj.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ln.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://av.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yw.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vo.szxytkj.cn

[J03] 字符串解析为日期
来源：http://pr.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lx.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uy.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://vz.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://pc.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oi.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hf.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://db.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uu.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://iw.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vx.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mi.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vk.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fk.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kc.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pn.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xp.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://na.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://jn.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://uf.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nv.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mk.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ra.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://eg.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ib.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://fi.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fp.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ue.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://vq.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://dw.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gl.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kk.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jw.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://gd.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://tn.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://oh.szxytkj.cn

[J07] 比较两个日期
来源：http://rg.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://vi.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tc.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fs.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aa.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zn.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lt.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cl.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://pz.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://xl.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iq.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pm.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kt.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cr.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://an.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nj.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://th.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hy.newstarts.cn

[J09] 时区处理
来源：http://ma.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sn.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://me.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://we.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kc.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://li.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jd.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zu.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://wc.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kw.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kr.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://up.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zu.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gl.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ui.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yg.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fa.newstarts.cn

================================================================================
来源：http://ts.yuexingan06.cn

K. JSON 与序列化
来源：http://qh.hahajie.cn

================================================================================
来源：http://qa.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://oo.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wy.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bm.colortex.cn

JS:   JSON.stringify(obj)
来源：http://cy.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://vy.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cu.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://yw.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bd.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lx.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://sf.shtwfgs.cn

Py:   json.loads(s)
来源：http://hc.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mm.newstarts.cn

JS:   JSON.parse(s)
来源：http://ec.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://js.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vs.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://lg.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ey.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ix.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://sm.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hx.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kl.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ay.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tv.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uw.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hr.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kd.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hy.asd995.cn

[K04] 读取 JSON 文件
来源：http://jp.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hp.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cg.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ma.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sl.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mp.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zg.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ds.jctech888.com.cn

[K05] 深拷贝对象
来源：http://gr.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ao.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://zy.newstarts.cn

JS:   structuredClone(obj)
来源：http://qf.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://zy.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oj.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ei.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vs.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ak.521024.cn

[K06] 解析 URL 查询串
来源：http://qa.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yw.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qz.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kt.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ii.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pz.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tb.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://md.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wf.bjjhwx.cn

[K07] 进制转换
来源：http://lo.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://my.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ic.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wi.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fq.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dz.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oe.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pb.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bv.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ff.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ge.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kq.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ay.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://oe.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://md.haigaiapp.cn

Go:   encoding/gob
来源：http://fo.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://sx.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ft.haigaiapp.cn

================================================================================
来源：http://hs.nszjky.cn

L. 网络请求
来源：http://ox.nszjky.cn

================================================================================
来源：http://xb.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://cn.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ow.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://me.gzmigu.cn

JS:   await fetch(url)
来源：http://al.wgjwhj.cn

TS:   await fetch(url)
来源：http://if.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xo.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://jb.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://us.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vg.huanxung.cn

[L02] 发送 POST JSON
来源：http://kl.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ty.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qi.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oc.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yk.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kk.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oc.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ae.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pk.huanxung.cn

[L03] 设置自定义请求头
来源：http://pt.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fb.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oe.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kr.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ds.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rb.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cr.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pl.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nf.chemitech.net.cn

[L04] 设置超时
来源：http://vb.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://ln.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://db.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yp.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hq.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dt.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xb.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zj.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://rt.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yz.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sn.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qe.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qt.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gw.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jq.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://se.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vk.9csxet.cn

[L06] 解析响应为 JSON
来源：http://yw.szxytkj.cn

Py:   resp.json()
来源：http://yd.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://cc.szxytkj.cn

JS:   await resp.json()
来源：http://nn.bjjhwx.cn

TS:   await resp.json()
来源：http://ks.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jw.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://be.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://dn.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gw.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://ef.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uo.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ps.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://pf.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ru.chemitech.net.cn

Java: resp.statusCode()
来源：http://wp.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://sm.lnxyls.cn

Ruby: resp.code.to_i
来源：http://fq.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://li.huanxung.cn

[L08] 并发请求多个地址
来源：http://wp.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vz.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://re.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wq.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rf.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ph.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kj.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ax.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tb.yuexingan06.cn

================================================================================
来源：http://iw.521024.cn

M. 命令行 / 进程 / 环境
来源：http://dv.521024.cn

================================================================================
来源：http://gg.jctech888.com.cn

[M01] 读取命令行参数
来源：http://tb.nicolike.cn

Py:   sys.argv[1:]
来源：http://bx.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://vo.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://jq.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://mo.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://qs.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://pq.hnjuh.cn

Ruby: ARGV
来源：http://xs.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://pa.wgjwhj.cn

[M02] 读取环境变量
来源：http://ww.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://pi.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://va.asd995.cn

JS:   process.env.HOME
来源：http://sj.shxzukj.cn

TS:   process.env.HOME
来源：http://jz.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://fs.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lw.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://um.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sv.bjjhwx.cn

[M03] 执行外部命令
来源：http://pm.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fa.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sx.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://il.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uc.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ec.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://at.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gn.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://fq.hahajie.cn

[M04] 获取当前工作目录
来源：http://un.jctech888.com.cn

Py:   os.getcwd()
来源：http://pf.hnjuh.cn

PHP:  getcwd();
来源：http://im.colortex.cn

JS:   process.cwd()
来源：http://fs.hahajie.cn

TS:   process.cwd()
来源：http://xe.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://gr.yuexingan06.cn

Go:   os.Getwd()
来源：http://dw.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://hl.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oz.yuntaijiaju.cn

[M05] 设置退出码
来源：http://ba.shtwfgs.cn

Py:   sys.exit(1)
来源：http://ex.huixiangedu.cn

PHP:  exit(1);
来源：http://vg.bookmarksfly.cn

JS:   process.exit(1)
来源：http://li.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://jp.wgjwhj.cn

Java: System.exit(1)
来源：http://ku.wgjwhj.cn

Go:   os.Exit(1)
来源：http://lz.huixiangedu.cn


<!-- 参考信息 -->