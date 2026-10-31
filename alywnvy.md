代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mm.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://of.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tq.521024.cn

================================================================================
来源：http://mo.shtwfgs.cn

J. 日期与时间
来源：http://ud.bjjhwx.cn

================================================================================
来源：http://ed.shxzukj.cn

[J01] 获取当前时间
来源：http://wy.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ji.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ja.hahajie.cn

JS:   new Date();  Date.now()
来源：http://xy.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://ki.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fk.panjiajie.cn

Go:   time.Now()
来源：http://ad.bjjhwx.cn

Ruby: Time.now
来源：http://pl.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xq.colortex.cn

[J02] 格式化输出
来源：http://dk.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pe.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vr.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xu.521024.cn

TS:   d.toISOString()
来源：http://fz.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kl.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hp.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uk.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ei.colortex.cn

[J03] 字符串解析为日期
来源：http://go.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lz.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xo.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://bg.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://vy.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oz.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ao.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://rr.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xs.colortex.cn

[J04] 时间戳与日期互转
来源：http://mu.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jx.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://de.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qr.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bc.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nt.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://um.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cc.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gr.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://rd.asd995.cn

Py:   now + timedelta(days=7)
来源：http://fm.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sb.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ij.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tn.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://gq.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qa.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://pp.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ar.jctech888.com.cn

[J06] 计算两时间之差
来源：http://mp.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://ss.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://zu.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yp.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sw.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aj.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://av.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://xi.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://yy.haigaiapp.cn

[J07] 比较两个日期
来源：http://um.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://an.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yd.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rf.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tc.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xa.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wm.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rh.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ep.lnxyls.cn

[J08] 提取年月日与星期
来源：http://kq.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sx.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xj.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lh.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cd.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zt.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://or.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gn.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fu.szsharing.cn

[J09] 时区处理
来源：http://pb.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mq.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gq.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pq.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kv.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zx.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kc.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nt.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ho.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://tt.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oy.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qx.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zq.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uj.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wl.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jv.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gg.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fa.wgjwhj.cn

================================================================================
来源：http://qo.szxytkj.cn

K. JSON 与序列化
来源：http://ug.bookmarksfly.cn

================================================================================
来源：http://zp.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://dq.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jo.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://vf.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://ju.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pm.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://lk.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://po.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tc.colortex.cn

[K02] JSON 字符串转对象
来源：http://ct.bjjhwx.cn

Py:   json.loads(s)
来源：http://hr.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pe.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ky.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://av.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dy.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://lf.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://gl.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fg.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://zh.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xu.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hi.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vy.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xj.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uc.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ib.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://im.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ci.szsharing.cn

[K04] 读取 JSON 文件
来源：http://mm.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uz.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bw.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nu.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wk.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ra.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ci.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ua.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://al.szsharing.cn

[K05] 深拷贝对象
来源：http://ea.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://qc.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://oa.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://vg.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://gc.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zk.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uq.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nn.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mi.newstarts.cn

[K06] 解析 URL 查询串
来源：http://fb.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iy.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zf.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gs.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wb.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dj.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kt.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rl.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uc.shxzukj.cn

[K07] 进制转换
来源：http://dj.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yn.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zs.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xi.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dp.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://re.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jm.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ka.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lo.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://we.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://ci.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pc.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://fg.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://da.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://io.hnjuh.cn

Go:   encoding/gob
来源：http://gj.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://jx.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xb.521024.cn

================================================================================
来源：http://fe.huixiangedu.cn

L. 网络请求
来源：http://ui.huixiangedu.cn

================================================================================
来源：http://an.lnxyls.cn

[L01] 发送 GET 请求
来源：http://tc.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zp.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wx.wgjwhj.cn

JS:   await fetch(url)
来源：http://ok.panjiajie.cn

TS:   await fetch(url)
来源：http://cz.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wn.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://so.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uj.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ja.gzmigu.cn

[L02] 发送 POST JSON
来源：http://qw.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://da.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lp.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cf.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nn.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pw.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nd.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bf.hnjuh.cn

[L03] 设置自定义请求头
来源：http://sn.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kl.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wa.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mu.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xg.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ds.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bo.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tm.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://du.szxytkj.cn

[L04] 设置超时
来源：http://ck.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://ku.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lv.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dp.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bm.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rv.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ma.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lh.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://su.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://fz.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cr.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://et.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uh.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hw.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qu.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nj.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oz.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wl.szsharing.cn

[L06] 解析响应为 JSON
来源：http://zy.szxytkj.cn

Py:   resp.json()
来源：http://cm.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://wl.bjjhwx.cn

JS:   await resp.json()
来源：http://ab.bjjhwx.cn

TS:   await resp.json()
来源：http://lp.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://db.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ro.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://no.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mu.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ig.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ar.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sh.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://wa.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://gi.jctech888.com.cn

Java: resp.statusCode()
来源：http://ui.nicolike.cn

Go:   resp.StatusCode
来源：http://cw.szsharing.cn

Ruby: resp.code.to_i
来源：http://hs.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://at.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://bs.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xs.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://vu.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gp.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cy.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ai.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fp.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tr.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gg.chemitech.net.cn

================================================================================
来源：http://ju.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://sx.szxytkj.cn

================================================================================
来源：http://lo.chemitech.net.cn

[M01] 读取命令行参数
来源：http://jm.colortex.cn

Py:   sys.argv[1:]
来源：http://qd.colortex.cn

PHP:  $argv;  $argc;
来源：http://ds.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://yb.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://lm.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://hd.newstarts.cn

Go:   os.Args[1:]
来源：http://kj.gzmigu.cn

Ruby: ARGV
来源：http://oj.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://xo.nicolike.cn

[M02] 读取环境变量
来源：http://yh.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ia.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zl.bookmarksfly.cn

JS:   process.env.HOME
来源：http://qh.shxzskj.cn

TS:   process.env.HOME
来源：http://hj.szxytkj.cn

Java: System.getenv("HOME")
来源：http://ox.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vy.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ic.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aq.huanxung.cn

[M03] 执行外部命令
来源：http://mg.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ys.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bg.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kn.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dq.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qo.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fb.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wc.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://nl.shxzskj.cn

[M04] 获取当前工作目录
来源：http://pj.huixiangedu.cn

Py:   os.getcwd()
来源：http://wo.asd995.cn

PHP:  getcwd();
来源：http://af.panjiajie.cn

JS:   process.cwd()
来源：http://oz.lnxyls.cn

TS:   process.cwd()
来源：http://ou.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://kw.shxzukj.cn

Go:   os.Getwd()
来源：http://uc.jctech888.com.cn

Ruby: Dir.pwd
来源：http://gi.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rt.nicolike.cn

[M05] 设置退出码
来源：http://io.lnxyls.cn

Py:   sys.exit(1)
来源：http://nx.shxzskj.cn

PHP:  exit(1);
来源：http://xa.wgjwhj.cn

JS:   process.exit(1)
来源：http://vn.chemitech.net.cn

TS:   process.exit(1)
来源：http://fv.asd995.cn

Java: System.exit(1)
来源：http://ys.lnxyls.cn

Go:   os.Exit(1)
来源：http://uj.yuntaijiaju.cn

Ruby: exit 1
来源：http://bo.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zk.wgjwhj.cn

[M06] 向标准错误输出
来源：http://nj.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://qh.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rg.jianghongdianzi.cn

JS:   console.error("err")
来源：http://kw.asd995.cn

TS:   console.error("err")
来源：http://rf.newstarts.cn

Java: System.err.println("err")
来源：http://fm.hnjuh.cn


<!-- 参考信息 -->