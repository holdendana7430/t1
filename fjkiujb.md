代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fk.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://je.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kt.panjiajie.cn

================================================================================
来源：http://ny.hnjuh.cn

J. 日期与时间
来源：http://yx.9csxet.cn

================================================================================
来源：http://ko.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://cq.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://my.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pj.asd995.cn

JS:   new Date();  Date.now()
来源：http://nl.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://ad.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wt.jianghongdianzi.cn

Go:   time.Now()
来源：http://ei.wgjwhj.cn

Ruby: Time.now
来源：http://dj.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ug.asd995.cn

[J02] 格式化输出
来源：http://ow.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ut.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://av.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://it.colortex.cn

TS:   d.toISOString()
来源：http://zd.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dv.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sz.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xl.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ro.newstarts.cn

[J03] 字符串解析为日期
来源：http://kz.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vo.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mb.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://tc.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://cj.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eq.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rb.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://hy.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kq.hahajie.cn

[J04] 时间戳与日期互转
来源：http://tw.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ky.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ca.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jx.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kb.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lr.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dh.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ze.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ts.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://ib.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://ad.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pw.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://in.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ua.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://bk.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pm.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://hv.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kq.shxzukj.cn

[J06] 计算两时间之差
来源：http://oi.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://ub.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ch.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ek.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vb.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xx.521024.cn

Go:   end.Sub(start).Hours()
来源：http://oi.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://sx.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ev.shxzukj.cn

[J07] 比较两个日期
来源：http://zf.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ay.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jw.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gi.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jm.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wv.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jx.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vx.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xk.lnxyls.cn

[J08] 提取年月日与星期
来源：http://dv.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sk.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wa.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kc.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bw.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://il.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xq.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uk.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mt.chemitech.net.cn

[J09] 时区处理
来源：http://xj.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ve.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uu.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xh.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yo.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fn.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pu.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://an.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lq.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://vs.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bd.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ok.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vj.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pk.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jp.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://be.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gt.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mj.9csxet.cn

================================================================================
来源：http://ge.lnxyls.cn

K. JSON 与序列化
来源：http://hn.shxzukj.cn

================================================================================
来源：http://vl.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://rf.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gp.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nz.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://tl.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://oh.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pj.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://qi.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://el.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dk.hahajie.cn

[K02] JSON 字符串转对象
来源：http://hw.chemitech.net.cn

Py:   json.loads(s)
来源：http://nn.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ti.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ml.hahajie.cn

TS:   JSON.parse(s)
来源：http://po.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eb.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://xd.colortex.cn

Ruby: JSON.parse(s)
来源：http://ff.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yt.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://bu.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ik.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lq.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pc.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xk.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://th.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qx.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uv.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tx.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://fm.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://md.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hh.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uf.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wf.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gy.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kq.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xu.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tm.bjjhwx.cn

[K05] 深拷贝对象
来源：http://zf.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://vs.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://gn.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://cf.asd995.cn

TS:   structuredClone(obj)
来源：http://pf.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aj.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://js.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jt.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kx.asd995.cn

[K06] 解析 URL 查询串
来源：http://jm.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wg.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xn.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mp.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uv.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://an.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zc.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nu.huixiangedu.cn

[K07] 进制转换
来源：http://fz.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sl.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jr.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://le.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dw.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jr.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qz.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ke.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jv.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://zg.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://aq.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sg.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://sj.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ug.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ht.muxihuayi.cn

Go:   encoding/gob
来源：http://ay.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://qc.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gd.colortex.cn

================================================================================
来源：http://bb.szxytkj.cn

L. 网络请求
来源：http://is.jctech888.com.cn

================================================================================
来源：http://ca.hnjuh.cn

[L01] 发送 GET 请求
来源：http://vn.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jn.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pn.hnjuh.cn

JS:   await fetch(url)
来源：http://px.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://yg.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jf.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://wr.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ko.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bt.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://xs.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ez.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fh.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zb.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rh.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yi.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pt.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aw.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://xn.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yd.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ta.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://se.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fk.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jf.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iq.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lu.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eb.gzmigu.cn

[L04] 设置超时
来源：http://ri.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://oy.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dh.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nm.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://av.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ox.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jc.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kl.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oi.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ql.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kb.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bx.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yc.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vf.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lk.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wt.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nw.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yw.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://yz.huixinmuqiang.cn

Py:   resp.json()
来源：http://yx.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://ze.panjiajie.cn

JS:   await resp.json()
来源：http://hz.shxzskj.cn

TS:   await resp.json()
来源：http://dw.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ba.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ee.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://lz.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ks.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://lm.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ls.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ob.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://mm.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ht.wgjwhj.cn

Java: resp.statusCode()
来源：http://ik.panjiajie.cn

Go:   resp.StatusCode
来源：http://gd.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://ki.colortex.cn

C#:   (int)resp.StatusCode
来源：http://hc.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://xa.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://af.521024.cn

PHP:  curl_multi_init() 系列
来源：http://xd.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fc.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sq.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ja.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wd.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pn.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wc.bookmarksfly.cn

================================================================================
来源：http://qu.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ww.muxihuayi.cn

================================================================================
来源：http://rf.szsharing.cn

[M01] 读取命令行参数
来源：http://mg.nicolike.cn

Py:   sys.argv[1:]
来源：http://mb.huanxung.cn

PHP:  $argv;  $argc;
来源：http://yd.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://fg.nszjky.cn

TS:   process.argv.slice(2)
来源：http://me.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://zq.nszjky.cn

Go:   os.Args[1:]
来源：http://gy.lnxyls.cn

Ruby: ARGV
来源：http://kg.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://zf.newstarts.cn

[M02] 读取环境变量
来源：http://al.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://zu.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hf.jctech888.com.cn

JS:   process.env.HOME
来源：http://sa.panjiajie.cn

TS:   process.env.HOME
来源：http://tx.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://uf.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://li.colortex.cn

Ruby: ENV["HOME"]
来源：http://eo.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bs.chemitech.net.cn

[M03] 执行外部命令
来源：http://ci.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tf.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vo.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ow.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ay.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oh.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ch.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fq.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://xd.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://lb.wgjwhj.cn

Py:   os.getcwd()
来源：http://dy.hnjuh.cn

PHP:  getcwd();
来源：http://mb.bjjhwx.cn

JS:   process.cwd()
来源：http://rt.panjiajie.cn

TS:   process.cwd()
来源：http://nn.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://lu.gzmigu.cn

Go:   os.Getwd()
来源：http://mf.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://kb.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://so.shxzskj.cn

[M05] 设置退出码
来源：http://is.muxihuayi.cn

Py:   sys.exit(1)
来源：http://wu.szsharing.cn

PHP:  exit(1);
来源：http://jb.wgjwhj.cn

JS:   process.exit(1)
来源：http://bi.nszjky.cn

TS:   process.exit(1)
来源：http://oc.jctech888.com.cn

Java: System.exit(1)
来源：http://xq.bjjhwx.cn

Go:   os.Exit(1)
来源：http://lg.bookmarksfly.cn

Ruby: exit 1
来源：http://bo.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kn.chemitech.net.cn

[M06] 向标准错误输出
来源：http://he.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://me.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yi.huanxung.cn

JS:   console.error("err")
来源：http://of.nszjky.cn

TS:   console.error("err")
来源：http://te.lnxyls.cn

Java: System.err.println("err")
来源：http://go.wgjwhj.cn


<!-- 参考信息 -->