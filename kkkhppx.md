代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pn.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nm.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://da.huanxung.cn

================================================================================
来源：http://jp.wgjwhj.cn

J. 日期与时间
来源：http://qz.szsharing.cn

================================================================================
来源：http://wo.huanxung.cn

[J01] 获取当前时间
来源：http://la.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pz.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://an.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://pk.colortex.cn

TS:   new Date();  Date.now()
来源：http://vl.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zz.hnjuh.cn

Go:   time.Now()
来源：http://ru.bjjhwx.cn

Ruby: Time.now
来源：http://wo.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qu.muxihuayi.cn

[J02] 格式化输出
来源：http://lp.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ne.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hq.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://af.huixiangedu.cn

TS:   d.toISOString()
来源：http://jc.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lf.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dy.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ho.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nh.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://xx.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gt.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vy.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ny.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://lx.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://du.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zy.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qx.9csxet.cn

[J04] 时间戳与日期互转
来源：http://pe.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pk.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ft.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nr.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yi.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://db.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hi.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ib.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pm.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://jz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://mr.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hb.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xv.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ji.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://xd.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fb.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://ol.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cc.gzmigu.cn

[J06] 计算两时间之差
来源：http://ow.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://wh.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ks.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nu.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ky.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qj.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://yi.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://gh.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://iy.szsharing.cn

[J07] 比较两个日期
来源：http://sk.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://yw.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://py.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lv.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ul.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rc.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ar.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cn.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ff.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://bl.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kq.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aq.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ny.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ep.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cu.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://os.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ye.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sj.shxzukj.cn

[J09] 时区处理
来源：http://ud.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://td.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bh.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://md.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ar.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wt.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sr.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yr.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zu.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://sw.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mc.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qf.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yn.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xm.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gr.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wi.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qr.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://na.gzmigu.cn

================================================================================
来源：http://cd.hahajie.cn

K. JSON 与序列化
来源：http://tn.newstarts.cn

================================================================================
来源：http://sx.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ye.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gl.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hj.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://mw.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://yr.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cy.hahajie.cn

Go:   json.Marshal(obj)
来源：http://uq.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kd.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iy.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://vz.lnxyls.cn

Py:   json.loads(s)
来源：http://hc.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cp.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ut.nicolike.cn

TS:   JSON.parse(s)
来源：http://yv.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rj.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://eb.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://jg.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cb.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://bz.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hx.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wo.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xi.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ie.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rn.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oj.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xd.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uy.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://uc.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pd.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kf.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vt.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mo.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oh.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ws.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jj.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tt.haigaiapp.cn

[K05] 深拷贝对象
来源：http://vw.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ik.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://vw.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://hs.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://dl.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://or.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ss.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bk.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rw.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://wt.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ei.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gx.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rc.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cj.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dk.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yu.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xy.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ck.chemitech.net.cn

[K07] 进制转换
来源：http://eh.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fu.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://he.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eo.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ek.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dv.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qo.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kx.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yk.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://le.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://kl.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lj.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://nt.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://jl.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pr.wgjwhj.cn

Go:   encoding/gob
来源：http://of.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://sj.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://cl.shxzskj.cn

L. 网络请求
来源：http://fi.shxzskj.cn

================================================================================
来源：http://nd.shxzskj.cn

[L01] 发送 GET 请求
来源：http://dm.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://il.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://co.nicolike.cn

JS:   await fetch(url)
来源：http://xo.huanxung.cn

TS:   await fetch(url)
来源：http://nq.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nq.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://iu.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jc.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qe.hahajie.cn

[L02] 发送 POST JSON
来源：http://gv.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vk.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xb.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wg.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ho.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zj.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://by.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ez.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ec.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://jw.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nb.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mb.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ud.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uz.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ge.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ff.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ds.panjiajie.cn

[L04] 设置超时
来源：http://kv.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://cx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kz.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nw.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://th.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ce.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ld.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ff.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qm.hahajie.cn

[L05] 上传文件（multipart）
来源：http://qi.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gc.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tx.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ox.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ct.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://by.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jh.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://hd.yuntaijiaju.cn

Py:   resp.json()
来源：http://bz.szsharing.cn

PHP:  json_decode($body, true);
来源：http://oh.huixinmuqiang.cn

JS:   await resp.json()
来源：http://pj.shtwfgs.cn

TS:   await resp.json()
来源：http://gt.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://me.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://uc.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yi.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://ye.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dh.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fq.asd995.cn

JS:   resp.ok;  resp.status
来源：http://yb.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://mk.shtwfgs.cn

Java: resp.statusCode()
来源：http://wu.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ov.hnjuh.cn

Ruby: resp.code.to_i
来源：http://ld.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://ru.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://hi.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uo.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://jd.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://na.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://im.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aq.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jf.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rw.muxihuayi.cn

================================================================================
来源：http://iu.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://rn.huanxung.cn

================================================================================
来源：http://az.huanxung.cn

[M01] 读取命令行参数
来源：http://al.szsharing.cn

Py:   sys.argv[1:]
来源：http://ae.newstarts.cn

PHP:  $argv;  $argc;
来源：http://hi.521024.cn

JS:   process.argv.slice(2)
来源：http://ku.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://ny.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://rm.shtwfgs.cn

Go:   os.Args[1:]
来源：http://mh.bjjhwx.cn

Ruby: ARGV
来源：http://ma.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://jm.nszjky.cn

[M02] 读取环境变量
来源：http://tf.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ml.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zt.lnxyls.cn

JS:   process.env.HOME
来源：http://dz.shxzskj.cn

TS:   process.env.HOME
来源：http://im.shxzukj.cn

Java: System.getenv("HOME")
来源：http://oy.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ae.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://pg.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xf.huixiangedu.cn

[M03] 执行外部命令
来源：http://am.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pe.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://no.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yk.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iw.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ep.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ls.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rj.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://jv.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://xb.lnxyls.cn

Py:   os.getcwd()
来源：http://qy.huixiangedu.cn

PHP:  getcwd();
来源：http://xz.muxihuayi.cn

JS:   process.cwd()
来源：http://rc.wgjwhj.cn

TS:   process.cwd()
来源：http://da.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://qm.bookmarksfly.cn

Go:   os.Getwd()
来源：http://hp.yuexingan06.cn

Ruby: Dir.pwd
来源：http://px.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tc.huixiangedu.cn

[M05] 设置退出码
来源：http://cb.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://kx.wgjwhj.cn

PHP:  exit(1);
来源：http://zw.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://mo.bjjhwx.cn

TS:   process.exit(1)
来源：http://zl.9csxet.cn

Java: System.exit(1)
来源：http://wj.gzmigu.cn

Go:   os.Exit(1)
来源：http://ha.newstarts.cn

Ruby: exit 1
来源：http://lr.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xs.asd995.cn

[M06] 向标准错误输出
来源：http://ms.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://xu.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xv.colortex.cn

JS:   console.error("err")
来源：http://ii.wgjwhj.cn

TS:   console.error("err")
来源：http://ev.chemitech.net.cn

Java: System.err.println("err")
来源：http://jt.shtwfgs.cn


<!-- 参考信息 -->